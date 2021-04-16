---
title: Omogućivanje povratnog pisanja lozinke na servisu Azure AD Connect
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
ms.openlocfilehash: 2ad7568bded3c8e4832e0e433a2d715e6307e4bb
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814004"
---
# <a name="enable-password-writeback-in-azure-ad-connect"></a>Omogućivanje povratnog pisanja lozinke na servisu Azure AD Connect

Da biste omogućili samoposlužno vraćanje izvorne lozinke, najprije omogućite mogućnost povratnog pisanja na servisu Azure AD Connect. Na poslužitelju azure AD Connect učinite sljedeće:

1. Prijavite se na poslužitelj servisa Azure AD Connect i pokrenite čarobnjak za **konfiguraciju servisa Azure AD Connect.**
2. Na **stranici Dobro** došli kliknite **Konfiguriraj**.
3. Na **stranici Dodatni zadaci** odaberite **Prilagodba mogućnosti sinkronizacije**, a zatim **kliknite Dalje**.
4. Na **stranici Povezivanje sa servisom Azure AD** unesite vjerodajnicu globalnog administratora za klijent azure, a zatim kliknite **Dalje**.
5. Na stranicama **Za povezivanje direktorija** **i Filtriranje domene/OU** kliknite **Dalje.**
6. Na **stranici Neobavezne** značajke odaberite okvir pokraj mogućnosti **Vraćanje pisanja lozinkom pa** kliknite **Dalje**.
7. Na **stranici Spremno za** konfiguriranje kliknite **Konfiguriraj** i pričekajte da postupak završi.
8. Kada vidite završetak konfiguracije, kliknite **Izlaz**.

Kada je omogućeno vraćanje pisanja lozinkom na servisu Azure AD Connect, konfigurirajte Azure AD SSPR za povrat pisanja.  Da biste omogućili vraćanje pisanja lozinke u SSPR-u, učinite sljedeće:

1. Prijavite se na portal Azure pomoću globalnog administratorskog računa.
2. Potražite i odaberite **Azure Active Directory**, kliknite Ponovno postavljanje **lozinke**, a zatim **lokalnu integraciju**.
3. Postavite mogućnost za pisanje lozinki u **lokalni direktorij? na** **Da**.
4. Postavite mogućnost Dopusti **korisnicima otključavanje računa bez ponovnog postavljanja lozinke?** na **Da**.
5. Kada budete spremni, kliknite **Spremi**.

Dodatne informacije potražite u članku [Omogućivanje samoposlužnog](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback)vraćanja izvorne lozinke servisa Azure Active Directory u lokalno okruženje .

> [!NOTE]
>  Kada administrator ponovno postavi korisničku lozinku na portalu Azure, ako je taj korisnik združen ili se sinkronizira s lozinkama, lozinka se ponovno zapisi na lokalno. Za tu je funkciju potrebna licenca za Azure Premium (P1 ili P2) i trenutno nije podržana na portalu za administratore sustava Office.
