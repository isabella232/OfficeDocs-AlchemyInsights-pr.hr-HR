---
title: Pravilnik za lozinke
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/11/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "9277"
ms.openlocfilehash: 12751288d04a2ec5993bf4a546b7d0c862f8f171f5bfd7a337cb79cb95792056
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54040822"
---
# <a name="password-policies"></a>Pravilnik za lozinke

**Imam problema s pravilnikom o lozinkama za korisnika**

- Pravilnik za lozinke za korisnika ovisi o tome je li korisnik samo u oblaku ili lokalno.
- Samo korisnici u oblaku moraju odabrati lozinku koja zadovoljava preduvjete u ovom članku: pravilnike za lozinke [koji se odnose samo na korisničke](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#password-policies-that-only-apply-to-cloud-user-accounts) račune u oblaku
- Lokalni korisnici moraju odabrati lozinku koja zadovoljava lokalne preduvjete. Ako lokalni korisnik ne može postaviti lozinku, provjerite lokalne preduvjete.

**Ne znam kako postaviti ili provjeriti pravilnike o isteku lozinke**

- Pomoću komponente PowerShell možete postaviti i provjeriti pravilnik o isteku za korisnike u oblaku na klijentu. Slijedite upute u ovom članku: [Postavljanje ili provjera pravilnika za lozinke pomoću komponente PowerShell](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)
- Pravilnik o isteku lozinke za lokalne korisnike postavljen je u lokalnom AD-u.

**Ostale korisne veze:**
- [Početak rada s vraćanjem izvorne lozinke](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)
- [Otklanjanje poteškoća s vraćanjem izvorne lozinke koju je pokrenuo administrator](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshoot-the-password-reset-portal)
