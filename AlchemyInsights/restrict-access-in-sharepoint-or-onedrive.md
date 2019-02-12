---
title: Ograničiti pristup u SharePoint ili OneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: e0fbec6eb269a173664e2b9a1efe6eefb527b96f
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 02/12/2019
ms.locfileid: "29905140"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Ograničiti pristup u SharePoint ili OneDrive

U SharePoint i OneDrive, ograničiti pristup stavki kao što su datoteke, mape i popisa tako da pristup dozvolite samo grupe ili pojedinci želite imati pristup. Po zadanom, dozvole u SharePoint nasljeđuju od gore viši u hijerarhiji. Stoga datoteku svoje dozvole nasljeđuju od mapa nasljeđuje dozvole iz biblioteke koji svoje dozvole nasljeđuju od web-mjesta.
  
Možete zajednički koristiti na višoj razini (kao što su po zajedničko korištenje cijelo web-mjesto) i ukinuti nasljeđivanje ako želite zajednički koristiti stavke na web-mjestu. Međutim, ne preporučujemo ovo jer olakšava održavanje dozvola kompleksne i zbunjujuće u budućnosti. Evo što nije moguće učiniti umjesto toga:
  
- Ako, na primjer, želite zajednički koristiti sadržaj mape osim jedne datoteke u njoj, premještanje te datoteke na novo mjesto nije zajednički.
    
- Ako imate dva podmape u mapi i želite dijeliti jednu podmapu s grupama A i B i dopustiti samo pristup grupi A drugi podmapu, dijeliti nadređene mape s grupom A i dodavanje grupe B prvu podmapu.
    
[Prekid zajedničkog korištenja datoteke ili mape](https://go.microsoft.com/fwlink/?linkid=2008861)
  

