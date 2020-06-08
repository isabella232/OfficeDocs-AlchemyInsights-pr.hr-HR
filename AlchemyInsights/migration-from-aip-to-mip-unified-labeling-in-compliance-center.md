---
title: Migracija iz AIP-a u MIP/objedinjeno označavanje u centru za usklađenost
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5114"
ms.openlocfilehash: 7ce9c387fc94f59674a922c5fe071fc0fb030344
ms.sourcegitcommit: e6d73d240669342fde9d4d25b0ee2838b7e43965
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 05/14/2020
ms.locfileid: "44236362"
---
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a>Migracija iz AIP-a u MIP/objedinjeno označavanje u centru za usklađenost

Da biste migrirali s AIP oznaka u objedinjeno označavanje u centru za sigurnost i usklađenost, učinite sljedeće:

**Aktiviranje zaštite s portala Azure**

1. Ako to još niste učinili, otvorite novi prozor preglednika i [prijavite se na portal Azure](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal). Idite na oštricu **Azure Information Protection.** Na primjer, na izborniku koncentratora kliknite **Svi servisi** i počnite upisivati **informacije** u okvir Filtar. Odaberite **Azure information protection**. Ako još niste pristupili oštrici Azure Information Protection, pogledajte [jednokratne dodatne korake](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) za dodavanje ove oštrice na portal. Da biste otvorili oštricu Azure Information Protection, morate imati [tarifu Azure Information Protection Premium](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) ili tarifu za Office 365 koja uključuje upravljanje pravima. Ako imate jednu od tih pretplata, ali vidite poruku da nije moguće pronaći valjanu pretplatu, [obratite se Microsoftovoj podršci](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) ili koristite standardne kanale podrške.

2. Pronađite mogućnosti izbornika **Upravljanje** i odaberite **Aktivacija zaštite**. Kliknite **Aktiviraj**, a zatim potvrdite akciju. Kada se aktivacija dovrši, informativna traka prikazuje **aktivaciju uspješno dovršenu**.

**Migracija oznaka zaštite podataka za Azure u Centar za usklađenost sa sigurnosnim & sustava Office 365**

1. Provjerite jeste li prijavljeni kao korisnik s dozvolom globalnog administratora.

2. Idite na oštricu **Azure Information Protection.**

3. Na izborniku **Upravljanje** odaberite **Objedinjena oznaka**.

4. Na oštrici **Azure Information Protection - Unified labeling** kliknite **Aktiviraj** i slijedite mrežne upute.

**Napomena**: Provjerite imate li odgovarajuće dozvole prije aktivacije migracije centra za & sigurnosti & usklađenosti. Pogledajte ove članke za više informacija:

1. [Trebate li globalni administrator konfigurirati zaštitu podataka za Azure ili mogu delegirati drugim administratorima?](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [Važne informacije o administrativnim ulogama nakon migracije u centar za usklađenost & sigurnosti.](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

Dodatne informacije o AIP-u objedinjenoj migraciji označavanja u centar za sigurnost i usklađenost potražite u odjeljku [Migracija oznaka](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).
