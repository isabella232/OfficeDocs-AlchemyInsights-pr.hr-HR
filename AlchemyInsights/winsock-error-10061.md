---
title: 1554 Winsock pogreška 10061
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
ms.openlocfilehash: 4f8007bd8ccb4666260c75fdca15dd0b14eb4e96
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47698854"
---
# <a name="winsock-error-10061"></a>Poruka o pogrešci za Winsock 10061

Ovaj kod pogreške znači da Microsoft ne može uspostaviti TCP utičnicu (veza) s odredišnim domaćinom. Najvjerojatnije je uzrok te pogreške problem s konfiguracijom vatrozida. Da biste riješili problem, provjerite sljedeće postavke:

- Provjera konfiguracije vatrozida pomoću podataka u [URL-ovima programa Microsoft 365 i RASPONIMA IP adresa](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

- Ako je pogreška specifična za Exchange Online Protection (AOP), trebali ste prethodno biti obaviješteni o promjeni [IP adresa zaštite sustava Exchange Online](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

- Provjerite nije li davatelj internetskih usluga (ISP) blokirao priključak.

- Provjerite postavke pametnog glavnog računala i odredišnog poslužitelja u poveznicima.

Imajte na čemu da Microsoft 365 ne blokira *dolazne* veze na taj način.
