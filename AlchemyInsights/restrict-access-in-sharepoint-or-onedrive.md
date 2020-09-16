---
title: Ograničavanje pristupa u sustavu SharePoint ili na servisu OneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: d8be1eb5bdcd0b5b08ddad32a45b6282c788c26a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720674"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Ograničavanje pristupa u sustavu SharePoint ili na servisu OneDrive

U sustavu SharePoint i na servisu OneDrive ograničite pristup stavkama kao što su datoteke, mape i popisi tako da pristupate samo grupama ili pojedincima kojima želite pristupiti. Dozvole u sustavu SharePoint po zadanom se nasljeđuju od viših prema gore u hijerarhiji. Tako da datoteka nasljeđuje dozvole iz mape, koja nasljeđuje dozvole iz biblioteke, koja nasljeđuje dozvole od web-mjesta.
  
Možete zajednički koristiti na višoj razini (kao što je zajedničko korištenje cijelog web-mjesta), a zatim prekinuti nasljeđivanje ako ne želite zajednički koristiti sve stavke na web-mjestu. No to ne preporučujemo jer čini održavanje dozvola složenijim i dvosmislenim u budućnosti. Evo što možete učiniti:
  
- Ako, primjerice, želite zajednički koristiti sve sadržaje mape osim jedne datoteke u njoj, premjestite je na novo mjesto koje se ne zajednički koristi.
    
- Ako u mapi imate dvije podmape, a želite zajednički koristiti jednu podmapu s grupama A i B te dopustiti samo grupu pristupa drugoj podmapi, zajednički koristite nadređenu mapu s grupom a i dodajte grupu B u prvu podmapu.
    
[Prestanak zajedničkog korištenja datoteke ili mape ](https://go.microsoft.com/fwlink/?linkid=2008861)
  

