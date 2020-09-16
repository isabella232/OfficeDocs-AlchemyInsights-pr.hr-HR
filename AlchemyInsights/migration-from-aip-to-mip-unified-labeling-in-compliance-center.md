---
title: Migracija iz AIP-a na MIP/Unified označavanje u centru za usklađenost
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
- "9002278"
- "5114"
ms.openlocfilehash: 7157eada10db2443f64fb7925f408359275d75eb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47674318"
---
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a>Migracija iz AIP-a na MIP/Unified označavanje u centru za usklađenost

Da biste migrirali iz Alp naljepnica na sjedinjenje označavanja u centru za sigurnost i usklađenost, učinite sljedeće:

**Aktivacija zaštite s portala Azure**

1. Ako to već niste učinili, otvorite novi prozor preglednika i [prijavite se na portal Azure](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal). Dođite do noža za **zaštitu podataka za Azure** . Na izborniku koncentrator, primjerice, kliknite **sve servise** i počnite upisivati **podatke** u okvir Filtar. Odaberite **zaštiti informacija o Azure**. Ako prije niste pristupili oštrici zaštite za Azure, pogledajte [upute](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) za dodavanje ove oštrice na portal. Da biste otvorili nož za zaštitu informacija za Azure, morate imati [tarifu za zaštitu informacija za Azure](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) , ili plan sustava Office 365 koji obuhvaća upravljanje pravima. Ako imate neku od tih pretplata, ali pogledajte poruku da nije moguće pronaći valjanu pretplatu, obratite se [Microsoftovoj podršci](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) ili koristite standardne kanale za podršku.

2. Pronađite mogućnosti izbornika **Upravljanje** , a zatim odaberite **Zaštita**. Kliknite **Aktiviraj**, a zatim potvrdite akciju. Kada aktivacija bude dovršena, ta će se informacijska traka prilikom aktivacije prikazati **uspješno dovršena**.

**Migracija naljepnica s zaštitom servisa Azure na servisu Office 365 Security & centar za usklađenost**

1. Provjerite jeste li prijavljeni kao korisnik s dozvolom globalnog administratora.

2. Dođite do noža za **zaštitu podataka za Azure** .

3. Na **stranici Upravljanje** izbornikom odaberite **sjedinjeno označavanje**.

4. Na stranici za **zaštitu od Azure – jedinstven** okvir za označavanje kliknite **Aktiviraj** , a zatim slijedite upute na internetu.

**Pažnja**: Provjerite imate li odgovarajuće dozvole prije aktiviranja migracije centra za sigurnost &. Dodatne informacije potražite u sljedećim člancima:

1. [Morate li biti globalni administrator da biste konfigurirali zaštitu za informacije o Azure ili mogu li delegirati drugim administratorima?](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [Važne informacije o administratorskim ulogama nakon migracije u centar za sigurnost & usklađenosti.](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

Dodatne informacije o programu AIP za sjedinjenje označavanja migracije u centar za sigurnost i usklađenost potražite u članku [migracija naljepnica](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).
