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
ms.openlocfilehash: f70b43a8b914b0d2dda9db61606b8ae24523f869
ms.sourcegitcommit: 097a8cabe0d2280af489159789988a0ab532dabb
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 12/11/2020
ms.locfileid: "49677137"
---
# <a name="device-in-pending-state"></a>Uređaj u stanju na čekanju

**Preduvjeti**

1. Ako prvi put postavljate registracije uređaja, provjerite jeste li pregledali [Uvod u upravljanje uređajima u servisu Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) koji će vas voditi na način na koji možete nabaviti uređaje u odjeljku kontrola Azure AD.
2. Ako izravno registrirate uređaje u Azure AD i postavite ih u Intune, morat ćete se pobrinuti da ste [konfigurirali Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) i da prvo imate [licenciranje](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) .
3. Provjerite jeste li ovlašteni za izvršavanje operacija u Azure AD i lokalnom AD-u. Samo globalni administrator u servisu Azure AD može upravljati postavkama za registraciju uređaja. Osim toga, ako postavljate automatske registracije u lokalnom servisu Active Directory, morat ćete biti administrator servisa Active Directory i AD FS (ako je primjenjivo).

Postupak registracije za hibridnu verziju Azure AD Join zahtijeva uređaje za korporacijsku mrežu. Internet isto tako utvrde na VPN, ali ima neki opomena to taj. Čuli smo da kupci trebaju pomoć pri otklanjanju poteškoća s postupkom registracije hibridne Azure AD Join u odjeljku udaljeni uvjeti rada.

**Okruženje za provjeru autentičnosti u oblaku (korištenje značajke korištenja lozinke za Azure AD i provjera autentičnosti)**

Ovaj tijek registracije poznat je i kao "Sinkronizacija pridruživanja".

Ovdje se nalazi kvar u tijeku postupka registracije:

1. Windows 10 otkriva točku povezivanja servisa (SCP) kada se korisnik prijavljuje na uređaj.

    1. Uređaj najprije pokuša dohvatiti informacije o klijentu s klijentskog SCP-a u registru [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]. Dodatne informacije potražite u članku [dokument](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).
    1. Ako ne uspije, uređaj komunicira s lokalnim programom Active Directory radi nabavljanje informacija o klijentu iz programa SCP. Da biste potvrdili SCP, obratite se ovom [dokumentu](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).

    > [!NOTE]
    > Preporučujemo da u aktivnom direktoriju omogućite SCP, a za početnu provjeru valjanosti koristite samo SKP za klijentski dio.

2. Windows 10 pokušava razgovarati s Azure AD u odjeljku sistemski kontekst radi provjere autentičnosti za Azure AD.

    Možete potvrditi može li uređaj pristupati Microsoftovim resursima u odjeljku sistemski račun pomoću skripte za povezivanje s [registriranjem testnog uređaja](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0).

3. Windows 10 generira samopotpisani certifikat i pohranjuje ga u objekt računala u lokalnom servisu Active Directory. Za to je potreban kontrolor domene.

4. Objekt uređaja s certifikatom može se sinkronizirati s programom Azure AD putem servisa Azure AD Connect. Ciklus sinkronizacije svaki je 30 minuta po zadanom, ali ovisi o konfiguraciji servisa Azure AD Connect. Dodatne informacije potražite u ovom [dokumentu](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).

5. U ovoj će fazi biti moguće vidjeti predmet uređaja u odjeljku "u **tijeku**" u odjeljku sprava Blade of Azure portal.

6. Kada se sljedeći korisnik prijavi na Windows 10, registracija će biti dovršena.

    > [!NOTE]
    > Ako ste na VPN-u i odjava/prijava prestaje s povezivanjem domene, registraciju možete aktivirati ručno. Da biste to učinili, učinite sljedeće:
    >
    > Problem `dsregcmd /join` lokalno na administratorskom upitu ili na daljinu putem Psexez-a na PC.
    >
    > Na primjer: `PsExec -s \\win10client01 cmd, dsregcmd /join`

Za česte probleme s registracijom uređaja Azure Active Directory, pročitajte članak [Najčešća pitanja o uređajima](https://docs.microsoft.com/azure/active-directory/devices/faq).
