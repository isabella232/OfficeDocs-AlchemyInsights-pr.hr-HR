---
title: Omogućivanje povratnog pisanja lozinke u aplikaciji Azure AD Povezivanje
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002933"
- "5615"
ms.openlocfilehash: 63304667cce67c48fd8bbeee52ff6d61d033ea38fd8d4c4d96c240847dab2cab
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54118196"
---
# <a name="enable-password-writeback-in-azure-ad-connect"></a>Omogućivanje povratnog pisanja lozinke u aplikaciji Azure AD Povezivanje

Da biste omogućili samoposlužno vraćanje izvorne lozinke, najprije omogućite mogućnost povratnog pisanja na servisu Azure AD Povezivanje. Na poslužitelju servisa Azure AD Povezivanje učinite sljedeće:

1. Prijavite se na poslužitelj servisa Azure AD Povezivanje pokrenite čarobnjak za konfiguriranje **servisa Azure AD Povezivanje** Azure AD.
2. Na **stranici Dobro** došli kliknite **Konfiguriraj**.
3. Na **stranici Dodatni zadaci** odaberite **Prilagodba mogućnosti sinkronizacije**, a zatim **kliknite Dalje**.
4. Na **stranici Povezivanje Azure AD** unesite vjerodajnicu globalnog administratora za klijent azure, a zatim kliknite **Dalje**.
5. Na stranicama Povezivanje **domena/OU** filtriranja kliknite **Dalje**. 
6. Na **stranici Neobavezne** značajke odaberite okvir pokraj mogućnosti **Vraćanje pisanja lozinkom pa** kliknite **Dalje**.
7. Na **stranici Spremno za** konfiguriranje kliknite **Konfiguriraj** i pričekajte da postupak završi.
8. Kada vidite završetak konfiguracije, kliknite **Izlaz**.

Ako je u aplikaciji Azure AD Povezivanje omogućeno vraćanje pisanja lozinkom, konfigurirajte Azure AD SSPR za povrat pisanja.  Da biste omogućili vraćanje pisanja lozinke u SSPR-u, učinite sljedeće:

1. Prijavite se na portal Azure pomoću globalnog administratorskog računa.
2. Potražite i odaberite **Azure Active Directory**, kliknite Ponovno **postavljanje lozinke**, a zatim **kliknite Lokalne integracije**.
3. Postavite mogućnost za pisanje lozinki u **lokalni direktorij? na** **Da**.
4. Postavite mogućnost Dopusti **korisnicima otključavanje računa bez ponovnog postavljanja lozinke?** na **Da**.
5. Kada budete spremni, kliknite **Spremi**.

Dodatne informacije potražite u članku [Omogućivanje Azure Active Directory samoposlužnog](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback)vraćanja izvorne lozinke u lokalno okruženje .

> [!NOTE]
>  Kada administrator ponovno postavi korisničku lozinku na portalu Azure, ako je taj korisnik združen ili se sinkronizira s lozinkama, lozinka se ponovno zapisi na lokalno. Za tu je funkciju potrebna licenca za Azure premium (P1 ili P2) i trenutno nije podržana na portalu Office administratora.
