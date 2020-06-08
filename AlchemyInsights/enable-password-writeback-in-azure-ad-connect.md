---
title: Omogući vraćanje lozinkom u servisu Azure AD Connect
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002933"
- "5615"
ms.openlocfilehash: ab4b8692799d08363e1d726f72a3b80dcb598797
ms.sourcegitcommit: 0cf8d133d6feade6df8b1082444ce73faa91e145
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 05/13/2020
ms.locfileid: "44204617"
---
# <a name="enable-password-writeback-in-azure-ad-connect"></a>Omogući vraćanje lozinkom u servisu Azure AD Connect

Da biste omogućili ponovno pisanje samoposlužne lozinke, najprije omogućite mogućnost vraćanja na otpis u usluzi Azure AD Connect. Na poslužitelju Azure AD Connect učinite sljedeće:

1. Prijavite se na poslužitelj Azure AD Connect i pokrenite čarobnjak za konfiguraciju **usluge Azure AD Connect.**
2. Na stranici **Dobrodošlice** kliknite **Konfiguriraj**.
3. Na stranici **Dodatni zadaci** odaberite Prilagodi **mogućnosti sinkronizacije**, a zatim kliknite **Dalje**.
4. Na **stranici Povezivanje s Azure AD** unesite vjerodajnice globalnog administratora za klijenta azure, a zatim kliknite Dalje.
5. Na stranicama **povezivanje direktorija** i **domena/OU** filtriranja kliknite **Dalje**.
6. Na stranici **Neobavezne značajke** potvrdite okvir pokraj stavke **Povratni zapis lozinke** i kliknite **Dalje**.
7. Na **stranici Spremno za konfiguriranje** kliknite **Konfiguriraj** i pričekajte da se postupak završi.
8. Kada vidite da je konfiguracija dovršena, kliknite **Izlaz**.

Uz omogućen povratni unos lozinke u servisu Azure AD Connect, sada konfigurirajte Azure AD SSPR za povratni zapis.  Da biste omogućili vraćanje lozinke u SSPR-u, poduzmite sljedeće korake:

1. Prijavite se na portal Azure pomoću globalnog administratorskog računa.
2. Potražite i odaberite **Azure Active Directory**, kliknite Ponovno postavljanje **lozinke**, a zatim odaberite **Lokalna integracija**.
3. Postavite opciju za **Vraćanje lozinki u lokalni direktorij?** **Yes**
4. Postavite opciju za **Dopusti korisnicima otključavanje računa bez ponovnog postavljanja lozinke?** **Yes**
5. Kada ste spremni, kliknite **Spremi**.

Dodatne informacije [potražite u odjeljku Omogućivanje ponovnog vraćanja ponovnog postavljanja samoposlužne lozinke servisa Azure Active Directory u lokalno okruženje](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).
