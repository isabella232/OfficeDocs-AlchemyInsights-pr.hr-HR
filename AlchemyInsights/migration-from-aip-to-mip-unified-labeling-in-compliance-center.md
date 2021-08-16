---
title: Migracija iz AIP-a u MIP/Sjedinjeno označavanje u centru za usklađenost
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
- "9002278"
- "5114"
ms.openlocfilehash: 378c3f58f77db8b23682432c942cd4f9c3a392651ca6564528a635724ad66a25
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54000348"
---
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a>Migracija iz AIP-a u MIP/Sjedinjeno označavanje u centru za usklađenost

Da biste migrirati s AIP naljepnica na sjedinjeno označavanje u centru za sigurnost i usklađenost, učinite sljedeće:

**Aktivacija zaštite s portala Azure**

1. Ako to još niste učinili, otvorite novi prozor preglednika i [prijavite se na portal Azure](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal). Pomaknite se do **oštrice Azure Information Protection.** Na izborniku središte, primjerice, kliknite **Svi servisi i** počnite **upisivati informacije** u okvir Filtar. Odaberite **Azure Information Protection**. Ako još niste pristupili oštrici Azure Information Protection, [](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) pogledajte dodatne korake za dodavanje ove oštrice na portal. Da biste otvorili oštricu Azure Information Protection, morate imati plan [Azure Information Protection premium ili](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) plan Office 365 koji obuhvaća upravljanje pravima. Ako imate jednu od tih pretplata, ali vidite poruku da nije moguće pronaći valjanu pretplatu, obratite se [Microsoftovoj](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) podršci ili koristite standardne kanale podrške.

2. Pronađite mogućnosti **izbornika Upravljanje** i odaberite **Aktivacija zaštite**. Kliknite **Aktiviraj**, a zatim potvrdite akciju. Kada aktivacija završi, informativna traka prikazuje uspješno **dovršenu aktivaciju.**

**Migriranje naljepnica za Azure Information Protection u centar za Office 365 sigurnost & usklađenost**

1. Provjerite jeste li prijavljeni kao korisnik s dozvolom globalnog administratora.

2. Pomaknite se do **oštrice Azure Information Protection.**

3. Na **izborniku Upravljanje** odaberite **Sjedinjeno označavanje**.

4. Na **alatu Azure Information Protection - Unified labeling** blade (Sjedinjeno **označavanje) kliknite Aktiviraj** i slijedite mrežne upute.

**Napomena:** provjerite imate li odgovarajuće dozvole prije aktivacije migracije centra za & usklađenosti. Dodatne informacije potražite u ovim člancima:

1. [Morate li biti globalni administrator da biste konfigurirali Azure Information Protection ili mogu delegirati drugim administratorima?](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [Važne informacije o administrativnim ulogama nakon migracije u centar za & usklađenost.](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

Dodatne informacije o migraciji AIP-a u sjedinjeno označavanje u centar za sigurnost i usklađenost potražite u [članku Migracija naljepnica](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).
