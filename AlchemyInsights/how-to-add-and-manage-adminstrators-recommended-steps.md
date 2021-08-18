---
title: Dodavanje administratora i upravljanje njima – preporučeni koraci
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/07/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004114"
- "7194"
ms.openlocfilehash: 48a06fde215e007b6b81b32ab751ca8e4bba522d
ms.sourcegitcommit: 46e24d65cffd37b6988447c6738b3315303bbe13
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58339024"
---
# <a name="how-to-add-and-manage-administrators---recommended-steps"></a>Dodavanje administratora i upravljanje njima – preporučeni koraci

Na temelju opisa problema pronašli smo rješenje za vas. Većina korisnika uspjela je sami riješiti problem nakon što su slijedili našu dokumentaciju.

**Uređivanje administratora pretplate ili su administratora pretplate**

- Administrator računa može uređivati obje uloge, a administrator pretplate može mijenjati samo su administratore na [portalu Azure](https://ms.portal.azure.com/#home).
- [Dodavanje ili promjena administratora pretplate na Azure](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator)

**Ažuriranje pretplate administratora ili Co-Administrator za interne (AIRS) pretplate**

Administrator servisa ili su administrator mogu samostalno poslužiti ovu akciju pomoću sljedećih koraka:

1. Prijavite se na [portal Azure i](https://ms.portal.azure.com/#home) kliknite Upravljanje **troškovima + Naplata na** lijevoj oštrici.
2. Kliknite stavku retka s pretplatom. Time se otvara pregled pretplate.
3. Na **oštrici Pretplata** kliknite **Svojstva**. 
4. Kliknite gumb **Administrator servisa.**
5. Unesite e-poštu korisnika kojeg želite postaviti kao administratora servisa i kliknite U **redu**.

**Dodavanje/promjena/uklanjanje su administratora**

1. Prijavite se na [portal Azure kao administrator](https://ms.portal.azure.com/#home) servisa.
2. Otvorite [Pretplate](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) i odaberite pretplatu. (Su adminstratori se mogu dodijeliti samo u opsegu pretplate.)
3. Otvorite klasični administratori kontrole programa **Access (IAM)** Dodavanje su administratora za dodavanje da biste otvorili okno Dodavanje su  >    >    >   **administratora** (ako je mogućnost Dodaj su administratora onemogućena, označava da nema dozvola).
4. Odaberite korisnika kojeg želite dodati, a zatim kliknite **Dodaj**.

**uči više:**
- [Dodavanje su administratora](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Uklanjanje su administratora](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Promjena administratora servisa](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Prikaz administratora računa](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Upravljanje pristupom pomoću portala RBAC i Azure](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal)

**Dodavanje/brisanje korisnika pomoću Azure Active Directory (AD)**

Možete dodati nove korisnike ili izbrisati postojeće korisnike iz svoje Azure Active Directory (Azure AD) tvrtke ili ustanove:

1. Da biste dodali novog korisnika, prijavite se na [portal Azure](https://ms.portal.azure.com/#home) kao korisnik-administrator tvrtke ili ustanove.
2. Odaberite **Azure Active Directory**, **odaberite Korisnici,** a zatim **Kliknite Novi korisnik**.
3. Na **stranici** Korisnik ispunite potrebne podatke. Kliknite **Stvori**. Korisnik se stvara i dodaje u klijent azure AD.

**Saznajte više:**

- [Dodavanje novog korisnika](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [Brisanje korisnika](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [Dodavanje ili ažuriranje podataka o profilu korisnika pomoću Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)

**Preporučeni dokumenti**

- [Što je kontrola pristupa utemeljena na ulogama (RBAC)?](https://docs.microsoft.com/azure/role-based-access-control/overview)
- [Razumijevanje različitih uloga na servisu Azure](https://docs.microsoft.com/azure/role-based-access-control/rbac-and-directory-admin-roles)
- [Administratorske dozvole uloga u programu Azure Active Directory](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)
- [Vodič: Dodjela pristupa korisniku pomoću aplikacije RBAC i portala Azure](https://docs.microsoft.com/azure/role-based-access-control/quickstart-assign-role-user-portal)
- [Otklanjanje poteškoća s RBAC-om na servisu Azure](https://docs.microsoft.com/azure/role-based-access-control/troubleshooting)
- [Organiziranje resursa pomoću grupa za upravljanje servisom Azure](https://docs.microsoft.com/azure/governance/management-groups/overview)
- [Kako zatražiti kopiju fakture za Azure putem e-pošte](https://azure.microsoft.com/blog/azure-email-invoices/)
- [Dodavanje, ažuriranje ili uklanjanje kreditne ili debitne kartice sa servisa Azure](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card)
- [Upravljanje pretplatom (Ponovna aktivacija/otkazivanje/prebacivanje)](https://docs.microsoft.com/azure/cost-management-billing/manage/subscription-disabled)



