---
title: Omogućivanje lozinke za nepotvrđenim u servisu Azure ad Connect
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002933"
- "5615"
ms.openlocfilehash: 1e90aedab20c8abaa021ed980e868cea0503b7b1
ms.sourcegitcommit: db95fd628c45d9810e5af5c5a4e6388c793339ac
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 02/03/2021
ms.locfileid: "50093347"
---
# <a name="enable-password-writeback-in-azure-ad-connect"></a>Omogućivanje lozinke za nepotvrđenim u servisu Azure ad Connect

Da biste omogućili samoposlužnu lozinku za vraćanje izvornih postavki, najprije omogućite mogućnost nepotvrđenim u servisu Azure ad Connect. Na servisu Azure AD Connect Server dovršite sljedeće korake:

1. Prijavite se na poslužitelj za Azure AD Connect i pokrenite čarobnjak za konfiguraciju **Azure ad Connect** .
2. Na stranici **dobrodošlice** kliknite **Konfiguriraj**.
3. Na stranici **dodatni zadaci** odaberite **Prilagodi mogućnosti sinkronizacije**, a zatim kliknite **dalje**.
4. Na stranici **Povezivanje sa servisom Azure** Unesite korisničku vjerodajnicu za Azure, a zatim kliknite **dalje**.
5. Na stranicama **Connect direktorije** i **domene/ou** filtriranje kliknite **dalje**.
6. Na stranici **neobavezne značajke** odaberite okvir pokraj stavke **Lozinka nepotvrđenim** i kliknite **dalje**.
7. Na stranici **spremni za konfiguriranje** kliknite **Konfiguriraj** i pričekajte da se postupak završi.
8. Kada se prikaže kraj konfiguracije, kliknite **izlaz**.

Ako je u servisu Azure ad Connect omogućeno lozinka nepotvrđenim, konfigurirajte Azure ad sspr za nepotvrđenim.  Da biste omogućili lozinku nepotvrđenim u sspr-u, dovršite sljedeće korake:

1. Prijavite se na portal Azure pomoću globalnog administratorskog računa.
2. Potražite i odaberite **Azure Active Directory**, kliknite **ponovno postavljanje lozinke**, a zatim **lokalne integracije**.
3. Postavite mogućnost za **unos lozinki za vraćanje u lokalni direktorij?** **u da**.
4. Postavite mogućnost **Dopusti korisnicima da otključaju račune bez ponovnog postavljanja lozinke?** u **da**.
5. Kada ste spremni, kliknite **Spremi**.

Dodatne informacije potražite u članku [Omogućivanje izvorne lozinke za samoposluživanje u servisu Azure Active Directory ponovno postavljanje programa nepotvrđenim u lokalno okruženje](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).

> [!NOTE]
>  Ako administrator ponovno postavi korisnikovu lozinku na portalu Azure, ako je taj korisnik sinkroniziran ili je postavljen za lozinku, lozinka će biti napisana natrag na lokalno. Za tu je funkcionalnost potrebna licenca za Azure Premium (P1 ili P2) i trenutno nije podržana na portalu za administratore sustava Office.
