---
title: Pogreška Winsocka 1554 10061
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 96a9cfd11941158ddf13655c74974e3eb800e570
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29461895"
---
# <a name="winsock-error-10061"></a>Winsock pogreške 10061

Ta šifra pogreške znači da Office 365 nije mogao uspostaviti TCP utičnice (veza) s glavnog računala za cilj. Najvjerojatniji uzrok te pogreške je problem s konfiguracijom vatrozid. Da biste riješili problem, provjerite ove postavke:
  
- Provjerite konfiguraciju vatrozida s informacijama u [Office 365 URL i raspone IP adresa](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)
    
- Ako pogreška je specifičan za Exchange Online Protection (EOP), trebali ste primili prethodno obavijest promjenu [Exchange Online Protection IP adrese](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).
    
- Provjerite je li vaš davatelj internetskih usluga (ISP) blokira priključak.
    
- Provjerite pametne glavnog i ciljnog postavke poslužitelja u vaše poveznike.
    
Imajte na umu Office 365 ne blokiraj *dolazne* veze na ovaj način. 
  

