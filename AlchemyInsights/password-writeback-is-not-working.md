---
title: Lozinka writeback ne funkcionira
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
ms.openlocfilehash: d7766f908f025b5db8299aa45d01dc5389b321ec
ms.sourcegitcommit: 2f39850ac0fba9fbeba9b8b7939ae79b505d3b67
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 02/12/2021
ms.locfileid: "50243247"
---
# <a name="password-writeback-is-not-working"></a>Lozinka writeback ne funkcionira

**Imam problema s konfiguriranjem lozinke za nepotvrđenim**

- Lozinka nepotvrđenim je Premium značajka.
- Provjerite jeste li razumjeli preduvjete za licenciranje:
  - U vašoj tvrtki ili ustanovi mora biti dodijeljena najmanje jedna licenca
  - **Samo oblak korisnici** -bilo koji Office 365 (O365) Paid SKU ili Azure ad Basic
  - **Cloud i/ili lokalni korisnici** -Azure ad Premium P1 ili P2, Enterprise Mobility + Security (EMS) ili Secure produktivnost Enterprise (SPE)
    - Dodatne informacije o preduvjetima za licenciranje potražite u članku [Licencne preduvjete za ponovno postavljanje lozinke za Azure ad samoservisiranja](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)
- Imate najmanje jedan administratorski račun i jedan test korisnički račun s jednom od odgovarajućih licenci.
- Morate povezati Azure ad Connect s primarnom kontrolorom domene na kojoj je lozinka nepotvrđenim na posao. Možete konfigurirati Azure AD Connect da biste koristili primarni kontroler domene tako da desnom tipkom miša kliknete **Svojstva** sinkronizacijskog konektora servisa Active Directory, a zatim odaberete **Konfiguriranje particija direktorija**. Odatle potražite odjeljak **Postavke veze s kontrolerom domene** , a zatim potvrdite okvir **samo koristi preferirani kontroleri domena**.
  > [!NOTE]
  > Ako preferirani DC nije PDC emulator, Azure AD Connect i dalje će doći do PDC-a za lozinku writeback.
- Ponovno postavljanje lozinke konfigurirano je i omogućeno u vašem zakupcu. Dodatne informacije potražite u članku [Omogućivanje ponovnog vraćanja lozinki za Azure ad](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started).
- Provjerite je li administratorski račun koji se koristi za omogućivanje lozinke writeback račun administratora oblaka (stvoren u servisu Azure AD nije lokalni oglas)
- Imate jednu ili više-šumsku web-lokalnu implementaciju sa sustavom Windows Server 2008 R2, Windows Server 2012 ili Windows Server 2012 R2 s instaliranim najnovijim servisnim paketima
- Imate instaliran alat Azure AD Connect i pripremili ste svoj oglasni ambijent za sinkronizaciju u oblak. Prije testiranja lozinke writeback, provjerite jeste li prvi put dovršili kompletnu uvoz i potpunu sinkronizaciju iz oglasa i Azure ad u servisu Azure AD Connect.
- Dodatne informacije potražite u članku [potpuna sinkronizacija i puni uvoz u servisu Azure ad Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)

**Imam problema s vezom za lozinku nepotvrđenim**

1. Preuzimanje i Omogućivanje najnovije verzije servisa [Azure ad Connect](https://www.microsoft.com/download/details.aspx?id=47594)
2. Konfiguracija vatrozida: alat za Azure AD Connect (1.1.443 i noviji) Trebat će **Izlazni https** pristup:
    - passwordreset.microsoftonline.com
    - servicebus. Windows. Networks
3. Dopuštanje mirovanja veza koje traju najmanje 2-3 minuta

**I dalje imam problema s lozinkom nepotvrđenim**

- Ako i dalje imate poteškoća, pokušajte onemogućiti i ponovno omogućiti servis za lozinku nepotvrđenim u alatu za Azure ad Connect
- Dodatne informacije potražite u članku [onemogućivanje i ponovno omogućivanje lozinke za nepotvrđenim](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)
