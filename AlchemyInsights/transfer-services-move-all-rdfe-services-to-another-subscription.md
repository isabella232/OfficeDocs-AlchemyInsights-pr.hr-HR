---
title: Prijenos servisa – Premještanje svih servisa RDFE na drugu pretplatu
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
ms.openlocfilehash: d6744484fe42f09f03de562a00fd56712607d418
ms.sourcegitcommit: ec88047d550006a1df4b6f10a3f513218113b9a5
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 12/15/2020
ms.locfileid: "49691945"
---
# <a name="transfer-services---move-all-rdfe-services-to-another-subscription"></a>Prijenos servisa – Premještanje svih servisa RDFE na drugu pretplatu

**Premještanje resursa**

Resursi za Azure mogu se premjestiti u neku drugu pretplatu na Azure ili grupu resursa u istoj pretplati pomoću portala Azure, Azure PowerShell, Azure CLI ili ostatka API-ja za premještanje resursa.

Da biste mogli premještati resurse, pročitajte sljedeće:

- [Kontrolni popis prije preseljenja resursa](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#checklist-before-moving-resources)
- [Servisi koje je moguće premjestiti](https://docs.microsoft.com/azure/azure-resource-manager/move-support-resources?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Provjera valjanosti premještanja](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#validate-move)
- [Premještanje smjernica za servise](https://docs.microsoft.com/azure/azure-resource-manager/move-limitations/app-service-move-limitations?WT.mc_id=Portal-Microsoft_Azure_Support)

Da biste postojeće resurse premjestili u neku drugu grupu resursa ili pretplatu, možete koristiti sljedeće:

- [Portal Azure](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-the-portal)
- [Azure PowerShell](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-powershell)
- [Azure CLI](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-cli)
- [REST API](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-rest-api)

Udžbenik: [Premještanje resursa za Azure u neku drugu grupu resursa ili pretplatu](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)

**Otklanjanje pogrešaka s programom Azure Resource Manager**

Pogledajte članke u nastavku da biste saznali više o nekim uobičajenim pogreškama implementacije Azura i primili informacije da biste ih riješili. Ako ne možete pronaći kôd pogreške za vašu pogrešku pri implementaciji, pročitajte članak [Traženje koda pogreške](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code).

- [Otklanjanje poteškoća s pogreškama prilikom implementacije](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors)
- [Otklanjanje poteškoća s premještanjem resursa Azure na novu grupu resursa ili pretplatu](https://docs.microsoft.com/azure/azure-resource-manager/troubleshoot-move)

Imajte na glavi da ako želite nadograditi pretplatu na Azure, kao što je prebacivanje s besplatnog na plaćanje-kao-te-go, morat ćete pretvoriti pretplatu.

- Da biste nadogradili besplatnu probnu verziju, pročitajte članak [Nadogradnja besplatne probne ili Microsoftove pretplate na Azure da plati-kao-ti-ići](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription).
- Da biste promijenili račun Pay-It-te-go, pročitajte članak [Promjena pretplate na Azure Pay-kao-te-go u neku drugu ponudu](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer).

**Da biste dodali ili povezali pretplatu na Azure u servisu Azure Active Directory, učinite sljedeće:**

1. Prijavite se i odaberite pretplatu koju želite koristiti na [stranici pretplate na portalu Azure](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade).
2. Odaberite **Promijeni direktorij**.
3. Pregledajte sva upozorenja koja se prikazuju, a zatim odaberite **Promijeni**.
4. Direktorij se mijenja za pretplatu i prikazat će vam se poruka o uspjehu.
5. Otvorite *direktorij* mjenjač da biste otvorili novi direktorij. Da bi se sve ispravno prikazalo, može potrajati i do 10 minuta.

**Preporučeni dokumenti**

- [Prijenos vlasništva nad pretplatom na Azure](https://docs.microsoft.com/azure/billing-subscription-transfer)
- [Premještanje resursa u novu grupu resursa ili pretplatu](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources)
- [Upravljanje resursima pomoću portala Azure](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-portal)
