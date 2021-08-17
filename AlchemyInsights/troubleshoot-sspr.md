---
title: Otklanjanje poteškoća s SSPR-om
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
ms.openlocfilehash: 9d8184efdc60befd359059c62ea3eb1a14ad7d2a20dade921d4a71e424f52033
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54038950"
---
# <a name="troubleshoot-sspr"></a>Otklanjanje poteškoća s SSPR-om

**Imam problema s konfiguriranjem vraćanja izvorne lozinke**

- Ako ste administrator i tražite kako omogućiti samostalno ponovno postavljanje lozinke, pogledajte vodič za [omogućivanje SSPR-a](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr)da biste konfigurirali ponovno postavljanje lozinke za svoju organizaciju. Možete i pregledati preduvjete [licenciranja](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-licensing?WT.mc_id=Portal-Microsoft_Azure_Support). Morate imati barem jednu licencu dodijeljenu u tvrtki ili ustanovi.
    - **Korisnici samo u oblaku** – Office 365 (O365) plaćeni SKU ili Azure AD Basic
    - **Korisnici u oblaku i/ili** lokalnim korisnicima – Azure AD premium P1 ili P2, Enterprise Mobility + Security (EMS) ili Secure Productive Enterprise (SPE)
- Dodatna pitanja o samoposlužnom ponovnom postavljanju lozinke potražite u [najčešćim pitanjima.](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-faq?WT.mc_id=Portal-Microsoft_Azure_Support)

**Prikazuje mi se poruka o pogrešci**

Pregledajte ovaj članak da biste pronašli uobičajene pogreške i njihova rješenja: Otklanjanje poteškoća [sa samoposlužno vraćanjem lozinke](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support)

**Imam problem s pravilnikom o ponovnom postavljanju lozinke**

- Ako se pravilnik o ponovnom postavljanju lozinke ne ponaša prema očekivanom ili ako imate pitanja o pravilima za ponovno postavljanje lozinke, pregledajte ovaj članak: Pravilnik i ograničenja lozinke [u programu Azure Active Directory](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support).
- Pravila za ponovno postavljanje lozinke ne odnose se na administratore. Microsoft nametanje jakog zadanog pravilnika o ponovnom postavljanju lozinke s dva vrata za bilo koju ulogu administratora platforme Azure. Provjerite test s korisnikom koji nije administrator. Dodatne informacije o pravilniku o ponovnom postavljanju administratora potražite u ovom članku: Razlike pravilnika za [administratore.](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-reset-policy-differences)

**Ne želim da korisnici registriraju dodatne sigurnosne podatke za ponovno postavljanje lozinke**

Možete unaprijed popuniti podatke (atribute e-pošte i telefona) za korisnike pomoću API-ja, ljuske PowerShell ili azure AD Povezivanje. Da biste saznali kako čitati:

- [Implementacija vraćanja izvorne lozinke bez potrebe za registracijom korisnika](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support#set-and-read-authentication-data-using-powershell)
- [Koje podatke koristi ponovno postavljanje lozinke](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Želim da korisnici registriraju dodatne sigurnosne podatke za ponovno postavljanje lozinke**

1. Neka korisnici registriraju svoje sigurnosne podatke za samostalno ponovno postavljanje lozinke tako da ih usmjeravaju [na aka.ms/ssprsetup](https://mysignins.microsoft.com/security-info).
1. Kada se podaci popunjavaju korisniku (od strane korisnika ili administratora), usmjerite korisnika [na aka.ms/sspr](https://passwordreset.microsoftonline.com/) da bi korisnici mogli imati ovlasti za ponovno postavljanje vlastitih lozinki.
1. Ako korisnici i dalje nailazi na probleme, najvjerojatnije su **združeni** korisnici ili korisnici **sinkronizirani s** lozinkama. To znači da postoji problem sa servisom Za pisanje lozinkom.