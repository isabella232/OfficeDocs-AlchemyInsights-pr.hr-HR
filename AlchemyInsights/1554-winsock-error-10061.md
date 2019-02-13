---
title: Pogreška Winsocka 1554 10061
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 9331a6c2b6e92a66fb97daf7dc5655ec320cba0f
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 02/12/2019
ms.locfileid: "29903088"
---
# <a name="winsock-error-10061"></a>Winsock pogreške 10061

Ta šifra pogreške znači da Office 365 nije mogao uspostaviti TCP utičnice (veza) s glavnog računala za cilj. Najvjerojatniji uzrok te pogreške je problem s konfiguracijom vatrozid. Da biste riješili problem, provjerite ove postavke:
  
- Provjerite konfiguraciju vatrozida s informacijama u [Office 365 URL i raspone IP adresa](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)
    
- Ako pogreška je specifičan za Exchange Online Protection (EOP), trebali ste primili prethodno obavijest promjenu [Exchange Online Protection IP adrese](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).
    
- Provjerite je li vaš davatelj internetskih usluga (ISP) blokira priključak.
    
- Provjerite pametne glavnog i ciljnog postavke poslužitelja u vaše poveznike.
    
Imajte na umu Office 365 ne blokiraj *dolazne* veze na ovaj način. 
  

