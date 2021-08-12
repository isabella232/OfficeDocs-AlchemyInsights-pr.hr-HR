---
title: Uređaj u stanju na čekanju
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003244"
- "7319"
ms.openlocfilehash: 224e6e613c306b50e354930bcbe6f43f1c08528766cb6e681b0e9826b2d55a4d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53913995"
---
# <a name="device-in-pending-state"></a>Uređaj u stanju na čekanju

**Preduvjeti:**

1. Ako prvi put postavljate registracije uređaja, provjerite jeste li pregledali uvod u upravljanje uređajima [u sustavu Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) koji će vas voditi o tome kako nabaviti uređaje pod kontrolom servisa Azure AD.
2. Ako izravno registrirate uređaje na Azure AD i registrirate ih u Intune, morat [](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) ćete biti sigurni da ste [konfigurirali Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) i da ste prvo registrirali licencu.
3. Provjerite imate li ovlasti za izvođenje operacija na servisu Azure AD i lokalnom servisu AD. Samo globalni administrator na servisu Azure AD može upravljati postavkama za registracije uređaja. Osim toga, ako postavljate automatske registracije u lokalnom servisu Active Directory, morat ćete biti administrator servisa Active Directory i AD FS (ako je primjenjivo).

Hibridni postupak registracije pridruživanja servisa Azure AD zahtijeva da uređaji moraju biti na korporacijskoj mreži. Funkcionira i nad VPN-om, ali postoje neke upozorenje o tome. Čuli smo da korisnicima treba pomoć pri otklanjanju poteškoća s hibridnim postupkom registracije za Azure AD u udaljenim radnim okolnostima.

**Okruženje za provjeru autentičnosti u oblaku (pomoću sinkronizacije i provjere autentičnosti lozinke za Azure AD)**

Taj je tijek registracije poznat i kao "Sinkronizacija spoja".

Evo raščlamba onoga što se događa tijekom postupka registracije:

1. Windows 10 otkriva zapis točke povezivanja servisa (SCP) kada se korisnik prijavi na uređaj.

    1. Uređaj najprije pokušava dohvatiti podatke klijenta iz klijentskog SCP-a u registru [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]. Dodatne informacije potražite u članku [Dokument](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).
    1. Ako ne uspije, uređaj komunicira s lokalnim servisom Active Directory radi primanja podataka o klijentu od SCP-a. Da biste potvrdili SCP, pogledajte [ovaj dokument](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).

    > [!NOTE]
    > Preporučujemo da omogućite SCP u servisu Active Directory i koristite samo klijentski SCP za početnu provjeru valjanosti.

2. Windows 10 pokušava komunicirati sa servisom Azure AD u kontekstu sustava da bi se provjerila autentičnost u odnosu na Azure AD.

    Možete provjeriti može li uređaj pristupiti Microsoftovim resursima putem računa sustava pomoću skripte [Test Device Registration Connectivity](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0).

3. Windows 10 generira samoispravke certifikata i pohranjuje ga ispod objekta računala u lokalnom servisu Active Directory. Za to je potreban linijski kontroler domene.

4. Objekt uređaja s certifikatom sinkronizira se sa servisom Azure AD putem servisa Azure AD Povezivanje. Ciklus sinkronizacije po zadanom je svakih 30 minuta, ali ovisi o konfiguraciji servisa Azure AD Povezivanje. Dodatne informacije potražite u ovom [dokumentu](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).

5. U ovoj fazi trebali biste moći vidjeti predmet uređaja u stanju **"Na** čekanju" ispod oštrice uređaja portala Azure.

6. Prilikom sljedeće prijave korisnika na Windows 10 registracija će biti dovršena.

    > [!NOTE]
    > Ako ste na VPN-u, a prijava/e-prijava prekida vezu s domenom, registraciju možete pokrenuti ručno. Da biste to učiniti, učinite sljedeće:
    >
    > `dsregcmd /join`Izlajte lokalno administratorski upit ili daljinski putem servisa PSExec na PC.
    >
    > Na primjer: `PsExec -s \\win10client01 cmd, dsregcmd /join`

Uobičajene probleme s registracijom Azure Active Directory uređaja potražite u članku [Najčešća pitanja o uređajima](https://docs.microsoft.com/azure/active-directory/devices/faq).
