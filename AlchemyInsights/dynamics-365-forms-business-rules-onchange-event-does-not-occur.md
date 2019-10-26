---
title: Dynamics 365 Forms poslovna pravila-poslovno pravilo ne ispaljivanje za obrazac
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1926"
- "6200018"
ms.openlocfilehash: cbdedd2c5fcf5517243e60e36d86479d6c3f7814
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 10/25/2019
ms.locfileid: "36529011"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a>Događaj OnChange ne pojavljuje se ako se polje programski promijeni

Događaj *onChange* ne pojavljuje se ako se polje programski mijenja pomoću *atributa.* [SetValue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) metodu. Ako želite da se Rukovatelji događajima za događaj *onChange* pokrenuti nakon što postavite vrijednost, morate koristiti *atribut formcontext. podatkovni. entiteti.* [Fireonchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) metodu u vašem kodu.

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
