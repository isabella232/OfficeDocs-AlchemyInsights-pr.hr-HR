---
title: Vraćanje pisanja lozinkom ne funkcionira
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
- "9004595"
- "8210"
ms.openlocfilehash: 23f5e5fe9e00a4bb00f96d2023c81f6413a7d8b808fd46bfc94483944bb898dc
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53999736"
---
# <a name="password-writeback-is-not-working"></a>Vraćanje pisanja lozinkom ne funkcionira

**Imam problema s konfiguriranjem povratnih pisanja lozinkom**

- Vraćanje pisanja lozinkom premium je značajka.
- Provjerite razumijete li preduvjete za licenciranje:
  - Morate imati barem jednu licencu dodijeljenu u tvrtki ili ustanovi
  - **Korisnici samo u oblaku** – Office 365 (O365) plaćeni SKU ili Azure AD Basic
  - **Korisnici u oblaku i/ili** lokalnim korisnicima – Azure AD premium P1 ili P2, Enterprise Mobility + Security (EMS) ili Secure Productive Enterprise (SPE)
    - Dodatne informacije o preduvjetima licenciranja potražite u članku Preduvjeti za licenciranje za samostalno ponovno [postavljanje lozinke za Azure AD](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)
- Imate barem jedan administratorski račun i jedan probni korisnički račun s jednom od odgovarajućih licenci.
- Morate povezati Azure AD Povezivanje primarnim emulatorom kontrolera domene da bi vraćanje pisanja lozinke funkcioniralo. Azure AD Povezivanje možete konfigurirati tako da desnom tipkom miša  kliknete svojstva poveznika za sinkronizaciju servisa Active Directory, a zatim odaberete **konfiguriranje direktorijskih particija.** Ondje potražite odjeljak s postavkama veze **kontrolera** domene i potvrdite okvir pod nazivom koristi samo **preferirane kontrolere domena**.
  > [!NOTE]
  > Ako preferirani DC nije oponašanje PDC-a, Azure AD Povezivanje i dalje će se pozivati na PDC radi povrata lozinke.
- Vraćanje izvorne lozinke konfigurirano je i omogućeno na klijentu. Dodatne informacije potražite u članku [Omogućivanje korisnicima ponovno postavljanje lozinki za Azure AD](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started).
- Provjerite je li administratorski račun koji se koristi za omogućivanje pisanja lozinke administratorski račun u oblaku (stvoren na servisu Azure AD nije lokalni AD)
- Imate lokalnu implementaciju sustava Windows Server 2008 R2, Windows Server 2012 ili Windows Server 2012 R2 s instaliranim najnovijim servisnim paketima
- Imate instaliran alat azure AD Povezivanje i pripremili ste ad okruženje za sinkronizaciju s oblakom. Prije testiranja povratnog pisanja lozinke provjerite jeste li najprije dovršili potpuni uvoz i potpunu sinkronizaciju s ad i sa servisa Azure AD u aplikaciji Azure AD Povezivanje.
- Dodatne informacije potražite u članku Potpuna sinkronizacija i [potpuni uvoz na servisu Azure AD Povezivanje](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)

**Imam problem s vezom za vraćanje pisanja lozinkom**

1. Preuzimanje i omogućivanje najnovije verzije servisa [Azure AD Povezivanje](https://www.microsoft.com/download/details.aspx?id=47594)
2. Konfiguracija vatrozida: alat azure AD Povezivanje (1.1.443 i više) morat **će odlazni HTTPS** pristup:
    - passwordreset.microsoftonline.com
    - servicebus.windows.networks
3. Dopusti da se neaktivne veze zadržavaju najmanje 2 do 3 minute

**I dalje imam problema s vraćanjem pisanja lozinke**

- Ako i dalje imate poteškoća, pokušajte onemogućiti i ponovno omogućiti servis za vraćanje pisanja lozinke u alatu azure AD Povezivanje.
- Da biste saznali više, pogledajte kako [onemogućiti i ponovno omogućiti vraćanje pisanja lozinke](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)
