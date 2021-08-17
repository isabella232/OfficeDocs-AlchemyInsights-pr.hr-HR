---
title: Pogreška 1554 Winsock 10061
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
- "1554"
- "9000079"
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 7991f83a0b4791eaa7eb3246f7e61f781e4c7430931fbf920d7fd9e44c018d13
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54083222"
---
# <a name="winsock-error-10061"></a>Pogreška Winsock 10061

Taj kod pogreške znači da Microsoft nije mogao uspostaviti TCP utičnicu (vezu) s ciljnim hostom. Uzrok te pogreške najvjerojatnije je problem s konfiguracijom vatrozida. Da biste riješili problem, provjerite sljedeće postavke:

- Provjerite konfiguraciju vatrozida pomoću podataka u [Microsoft 365 URL-ova i raspona IP adresa](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

- Ako je pogreška specifična za Exchange Online Protection (EOP), trebali ste prethodno biti obaviješteni o promjeni [IP adresa Exchange Online Protection ip adresa](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

- Provjerite blokira li vaš davatelj internetskih usluga (ISP) priključak.

- Provjerite postavke pametnog glavnog računala i ciljnog poslužitelja u poveznikima.

Imajte Microsoft 365 ne blokira *dolazne* veze na taj način.
