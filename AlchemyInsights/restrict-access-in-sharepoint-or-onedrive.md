---
title: Ograničavanje pristupa u SharePoint ili OneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: b7b68df2ae24b09fe9b01bd67c31a89e37f284a512bc1ecb097ef52fae5ae7d6
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54075032"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Ograničavanje pristupa u SharePoint ili OneDrive

U SharePoint i OneDrive možete ograničiti pristup stavkama kao što su datoteke, mape i popisi davanjem pristupa samo grupama ili pojedincima kojima želite pristupiti. Dozvole u aplikaciji SharePoint prema zadanim postavkama nasljeđuju se od višeg prema gore u hijerarhiji. Datoteka nasljeđuje dozvole od mape, koja nasljeđuje dozvole iz biblioteke, što nasljeđuje dozvole od web-mjesta.
  
Zajedničko korištenje možete zajednički koristiti na višoj razini (npr. zajedničkim korištenjem cijelog web-mjesta), a zatim prekinuti nasljeđivanje ako ne želite zajednički koristiti sve stavke na web-mjestu. No to ne preporučujemo jer održavanje dozvola u budućnosti čini složenijima i zbunjujućima. Evo što biste mogli učiniti:
  
- Ako, primjerice, želite zajednički koristiti sav sadržaj mape, osim jedne datoteke u njemu, premjestite tu datoteku na novo mjesto koje se ne zajednički koristi.
    
- Ako u mapi imate dvije podmape i želite zajednički koristiti jednu podmapu s grupama A i B i omogućiti samo grupi A pristup drugoj podmapa, zajedničko korištenje nadređene mape s grupom A i dodavanje grupe B u prvu podmapu.
    
[Zaustavljanje zajedničkog korištenja datoteke ili mape ](https://go.microsoft.com/fwlink/?linkid=2008861)
  

