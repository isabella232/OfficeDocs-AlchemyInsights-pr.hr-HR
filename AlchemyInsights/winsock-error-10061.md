---
title: 1554 Winsock pogreška 10061
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1554"
- "9000079"
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: e8f62d97efc937518ef766b45e1747e83b7f99c3
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766161"
---
# <a name="winsock-error-10061"></a>Winsock pogreška 10061

Ovaj kôd pogreške znači da Microsoft nije mogao uspostaviti TCP utičnicu (vezu) s ciljnim glavnim računalom. Najvjerojatniji uzrok ove pogreške je problem s konfiguracijom vatrozida. Da biste riješili problem, provjerite sljedeće postavke:

- Provjera konfiguracije vatrozida pomoću podataka u [URL-ovima i rasponima IP adresa sustava Microsoft 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

- Ako je pogreška specifična za Exchange Online Protection (EOP), trebali ste prethodno biti obaviješteni o promjeni [IP adresa exchange online protection](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

- Provjerite blokira li davatelj internetskih usluga (ISP) priključak.

- Provjerite postavke pametnog glavnog računala i ciljnog poslužitelja u konektorima.

Imajte na umu da Microsoft 365 na taj način ne blokira *dolazne* veze.
