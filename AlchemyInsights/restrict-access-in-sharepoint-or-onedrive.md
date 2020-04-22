---
title: Ograničavanje pristupa u sustavu SharePoint ili OneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: ed8e97b20c96a7b46995c969074cc4cef3a787d9
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43715876"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Ograničavanje pristupa u sustavu SharePoint ili OneDrive

U sustavima SharePoint i OneDrive ograničavate pristup stavkama kao što su datoteke, mape i popisi dodjelom pristupa samo grupama ili pojedincima kojima želite pristupiti. Prema zadanim postavkama dozvole u sustavu SharePoint nasljeđuju se od višeg položaja u hijerarhiji. Dakle, datoteka nasljeđuje dozvole iz mape, koja nasljeđuje dozvole iz biblioteke, koja nasljeđuje svoje dozvole od web-mjesta.
  
Možete dijeliti na višoj razini (primjerice dijeljenjem cijelog web-mjesta), a zatim prekinuti nasljeđivanje ako ne želite dijeliti sve stavke na web-mjestu. Međutim, to ne preporučujemo jer održavanje dozvola čini složenijim i zbunjujućijima u budućnosti. Evo što možete učiniti umjesto toga:
  
- Ako, na primjer, želite zajednički koristiti sav sadržaj mape osim jedne datoteke u njoj, premjestite je na novo mjesto koje nije dijeljeno.
    
- Ako u mapi imate dvije podmape i želite zajednički koristiti jednu podmapu s grupama A i B i dopustiti samo grupni pristup drugoj podmapi, podijelite nadređenu mapu s grupom A i dodajte grupu B u prvu podmapu.
    
[Prekid zajedničkog korištenja datoteke ili mape](https://go.microsoft.com/fwlink/?linkid=2008861)
  

