---
title: Ograničavanje pristupa u sustavu SharePoint ili servisu OneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: e5458226fe33bd5cb3da1f608fb113b888fbfd16
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 10/18/2019
ms.locfileid: "36551443"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Ograničavanje pristupa u sustavu SharePoint ili servisu OneDrive

U sustavu SharePoint i servisu OneDrive ograničite pristup stavkama kao što su datoteke, mape i popisi dodjeljivanju pristupa samo grupama ili pojedincima kojima želite pristupiti. Prema zadanim postavkama, dozvole u sustavu SharePoint nasljeđuju se iz viših vrijednosti u hijerarhiji. Dakle, datoteka nasljeće svoje dozvole iz mape, koja nasljeće svoje dozvole iz biblioteke, koja nasljeće svoje dozvole od web-mjesta.
  
Možete dijeliti na višoj razini (kao što je dijeljenje cijelog web-mjesta), a zatim prekinuti nasljedstvo ako ne želite dijeliti sve stavke na web-mjestu. Međutim, to ne preporučujemo jer to čini održavanje dozvole složenijim i zbunjujućim u budućnosti. Evo što možete učiniti umjesto toga:
  
- Ako, na primjer, želite podijeliti sav sadržaj mape osim jedne datoteke u njoj, premjestite tu datoteku na novo mjesto koje se ne dijeli.
    
- Ako imate dvije podmape u mapi i želite podijeliti jednu podmapu s grupama A i B i dopustiti samo grupi pristup drugoj podmapi, podijelite nadređenu mapu s grupom A i dodajte grupu B u prvu podmapu.
    
[Zaustavljanje dijeljenja datoteke ili mape](https://go.microsoft.com/fwlink/?linkid=2008861)
  

