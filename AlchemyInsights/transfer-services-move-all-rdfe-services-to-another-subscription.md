---
title: Transfer Services - Move all RDFE services to another subscription
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004116"
- "7196"
ms.openlocfilehash: 89217922b8b51f2548f9fff53bf80364c0e897b1d9b34bfb7016f0b0f197cf17
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53940029"
---
# <a name="transfer-services---move-all-rdfe-services-to-another-subscription"></a>Transfer Services - Move all RDFE services to another subscription

**Premještanje resursa**

Resursi platforme Azure mogu se premjestiti u neku drugu pretplatu na Azure ili grupu resursa u istoj pretplati pomoću portala Azure, komponente Azure PowerShell, Azure CLI ili REST API-ja za premještanje resursa.

Da biste mogli premještati resurse, pogledajte sljedeće:

- [Kontrolni popis prije premještanja resursa](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#checklist-before-moving-resources)
- [Servisi koje je moguće premjestiti](https://docs.microsoft.com/azure/azure-resource-manager/move-support-resources?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Provjera valjanosti poteza](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#validate-move)
- [Premještanje smjernica za servise](https://docs.microsoft.com/azure/azure-resource-manager/move-limitations/app-service-move-limitations?WT.mc_id=Portal-Microsoft_Azure_Support)

Da biste postojeće resurse premjestili u drugu grupu resursa ili pretplatu, možete koristiti sljedeće:

- [Portal Azure](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-the-portal)
- [Azure PowerShell](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-powershell)
- [Azure CLI](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-cli)
- [REST API](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-rest-api)

Vodič: [Premještanje resursa servisa Azure u drugu grupu resursa ili pretplatu](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)

**Otklanjanje poteškoća s upraviteljem resursa za Azure**

Pogledajte članke u nastavku da biste saznali više o nekim uobičajenim pogreškama prilikom implementacije servisa Azure i primili informacije da biste ih riješili. Ako ne možete pronaći kod pogreške za pogrešku prilikom implementacije, pogledajte traženje [koda pogreške](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code).

- [Otklanjanje poteškoća s implementacijom](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors)
- [Otklanjanje poteškoća s premještanjem resursa servisa Azure u novu grupu resursa ili pretplatu](https://docs.microsoft.com/azure/azure-resource-manager/troubleshoot-move)

Imajte na umu da ako želite nadograditi pretplatu na Azure, kao što je prijelaz s besplatne na pay-as-you-go, morat ćete pretvoriti pretplatu.

- Da biste nadogradili besplatnu probnu verziju, pogledajte članak Nadogradnja besplatne probne verzije ili pretplate na Microsoft Imagine Azure na [Pay-As-You-Go](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription).
- Da biste promijenili račun za plaćanje po nalogu, pogledajte promjena pretplate na [Azure Pay-As-You-Go u drugu ponudu](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer).

**Da biste dodali ili povezali pretplatu na Azure Azure Active Directory klijentu:**

1. Prijavite se i odaberite pretplatu koju želite koristiti na [stranici Pretplate na portalu Azure](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade).
2. Odaberite **Promijeni direktorij**.
3. Pregledajte sva upozorenja koja se prikazuju, a zatim odaberite **Promijeni**.
4. Direktorij će se promijeniti za pretplatu i dobiti ćete poruku o uspjehu.
5. Pomoću *prekidača direktorija* idite na novi direktorij. Da bi se sve pravilno prikazilo, može potrajati i do 10 minuta.

**Preporučeni dokumenti**

- [Prijenos vlasništva nad pretplatom na Azure](https://docs.microsoft.com/azure/billing-subscription-transfer)
- [Premještanje resursa u novu grupu resursa ili pretplatu](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources)
- [Upravljanje resursima pomoću portala Azure](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-portal)
