---
title: Otklanjanje poteškoća sa sustavom SSPR
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/04/2021
ms.topic: article
ms.audience: Admin
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003259"
- "6128"
ms.openlocfilehash: 85bfc812dcffce008a6fa5394a6069bd64c514d6
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50429470"
---
# <a name="troubleshoot-sspr"></a>Otklanjanje poteškoća sa sustavom SSPR

**Imam problema s konfiguriranjem izvorne postavke lozinke**

- Ako ste administrator i tražite vraćanje izvorne lozinke za samoposluživanje, pročitajte članak [Vodič za omogućivanje SSPR](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr)-a da biste konfigurirali ponovno postavljanje lozinke za svoju tvrtku ili ustanovu. Možda ćete htjeti i pregledati [preduvjete za licenciranje](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-licensing?WT.mc_id=Portal-Microsoft_Azure_Support). U vašoj tvrtki ili ustanovi mora biti dodijeljena najmanje jedna licenca.
    - **Samo oblak korisnici** -bilo koji Office 365 (O365) Paid SKU ili Azure ad Basic
    - **Cloud i/ili lokalni korisnici** -Azure ad Premium P1 ili P2, Enterprise Mobility + Security (EMS) ili Secure produktivnost Enterprise (SPE)
- Dodatne informacije o ponovnom postavljanju lozinke potražite u članku [Najčešća](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-faq?WT.mc_id=Portal-Microsoft_Azure_Support)pitanja.

**Prikazuje mi se poruka o pogrešci**

Pregledajte ovaj članak da biste pronašli česte pogreške i njihova rješenja: [Otklanjanje poteškoća s resetom samoservisiranja lozinke](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support)

**Imam problema s pravilima za ponovno postavljanje lozinke**

- Ako se pravilo za ponovno postavljanje lozinke ne ponaša kao što je očekivano ili ako imate pitanja o pravilima za ponovno postavljanje lozinki, pregledajte ovaj članak: [pravila i ograničenja lozinke u servisu Azure Active Directory](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support).
- Pravila za ponovno postavljanje lozinke ne primjenjuju se na administratore. Microsoft nameće snažan zadani pravilnik o ponovnom postavljanju lozinki za bilo koju ulogu Azure administratora. Provjerite jeste li testirali s korisnikom koji nije administrator. Dodatne informacije o pravilniku o ponovnom postavljanju administratora potražite u ovom članku: [Vraćanje izvornih razlika pravilnika za administratore](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-reset-policy-differences).

**Ne želim da moji korisnici registriraju dodatne sigurnosne podatke za ponovno postavljanje lozinke**

Možete unaprijed popuniti podatke (adrese e-pošte i telefona) za korisnike pomoću API-ja, komponente PowerShell ili Azure AD Connect. Da biste saznali kako čitati:

- [Implementacija ponovnog postavljanja lozinke bez zahtjeva korisnika za registraciju](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support#set-and-read-authentication-data-using-powershell)
- [Koje podatke koristi ponovno postavljanje lozinke](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Želim da moji korisnici registriraju svoje dodatne sigurnosne podatke za ponovno postavljanje lozinki**

1. Neka vaši korisnici registriraju svoje sigurnosne podatke za ponovno postavljanje lozinke za samostalno posluživanje tako da ih usmjerite na [aka.MS/ssprsetup](https://mysignins.microsoft.com/security-info).
1. Nakon što podaci budu naseljeni korisniku (od korisnika ili administratora), usmjerite korisnika na [aka.MS/sspr](https://passwordreset.microsoftonline.com/) da bi korisnici mogli biti ovlašteni za ponovno postavljanje vlastitih lozinki.
1. Ako korisnici i dalje nailazite na probleme s kojima su najvjerojatnije **udružen** ili **zaporni sinkronizirani** korisnici. To znači da je vjerojatno došlo do problema s servisom lozinke za writeback.