---
title: Poslovna pravila - poslovna pravila koja se ne odnosi na obrazac za obrasce Dynamics 365
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1926"
- "6200018"
ms.openlocfilehash: 4ade8d2f68b465298e2d6efff3eef4f04f25c3bf
ms.sourcegitcommit: a413a0e27ef4ab8c484fa9fccff8bbef381c8b96
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35747153"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a>Događaj OnChange pojaviti ako programski promijeniti polje

Događaj *OnChange* pojaviti ako polje promijenjeno programski pomoću u *atribut.* Metoda [setValue](https://docs.microsoft.com/en-us/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) . Ako želite rukovatelja događajima za događaj *OnChange* za pokretanje nakon što postavite vrijednost mora koristiti u *atribut formContext.data.entity.* Metoda [fireOnchange](https://docs.microsoft.com/en-us/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) u kodu.

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/en-us/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
