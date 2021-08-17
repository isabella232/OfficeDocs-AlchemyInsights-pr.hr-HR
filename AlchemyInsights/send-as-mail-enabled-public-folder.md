---
title: Pošalji kao javnu mapu s omogućenom poštom u programu EXO
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.openlocfilehash: 22aa3e8f46c2ff4f62cb520b9498041dffb9d3a3eb607d788cc97b10bf32dbb5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54052558"
---
# <a name="sendas-mail-enabled-public-folder"></a>Javna mapa s omogućenim slanjem pošte

U sljedećem se primjeru korisniku Jasonu dodjeljuju dozvole "Pošalji kao" za javnu mapu NewPF1 s omogućenom poštom.

Add-RecipientPermission -Identity 'NewPF1' -Trustee "Jason" -AccessRights 'SendAs'

Detaljne informacije o sintaksi i parametrima potražite u članku Dodjela dozvola "Pošalji kao" ili "Pošalji u ime" za javne mape [s omogućenom poštom](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/assign-permissions-mail-enabled-pfs).

