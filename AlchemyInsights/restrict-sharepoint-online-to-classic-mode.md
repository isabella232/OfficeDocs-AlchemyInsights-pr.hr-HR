---
title: Ograničavanje sustava SharePoint online na klasičan način rada
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.custom:
- "1835"
- "1889"
- "9000225"
ms.openlocfilehash: 1887bf64df98bf90a1902250633d5774178dfa2f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47751414"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a>Ograničavanje sustava SharePoint online na klasičan način rada

Neke ustanove i dalje zahtijevaju klasično iskustvo načina rada. Iako nema planova za uklanjanje klasičnog načina rada na granulacijskom nivou, više nije moguće ograničiti cijelu organizaciju (korisnika) na klasični način za popise i biblioteke.

Administrator će imati sljedeće mogućnosti za upravljanje pojedinačnim popisima i bibliotekama u klasičnom načinu rada uz Granularne parametre isključivanja koje dajemo na sljedećim razinama:

- Zbirka web-mjesta
- stranice
- popis
- biblioteka

Osim toga, popisi koji koriste određene značajke i prilagodbe koje moderni neće podržavati i dalje će se automatski prebaciti u klasični način rada.

Počevši od travnja 1, 2019, postupak za onemogućivanje izuzeća iz modernog popisa i biblioteka započet će i nastavit će se kroz Svibanj 31, 2019.  Popisi i biblioteke koji su u klasičnom načinu rada kao rezultat izuzećih korisnika automatski će se pomaknuti na moderno.

Ako vam je potreban klasičan način rada, Pogledajte dodatne informacije [ovdje](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) i upute za PNP PowerShell [ovdje](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) koje opisuju mogućnosti i alate koje danas možete koristiti da biste koristili klasičan način rada.
