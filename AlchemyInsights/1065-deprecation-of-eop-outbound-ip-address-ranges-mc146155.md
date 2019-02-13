---
title: 1065 postupku EOP izlaznog IP adresa rangesMC146155
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 9/28/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: 2b4b2e2341f45e2d37713d72a2e0d34fa1a9a7cc
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 02/12/2019
ms.locfileid: "29934876"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a>Postupku EOP izlaznog IP adresu raspona

Možemo ste otkrio mogući problem s vaše organizacije (Ako ne ispravlja po listopad 26th, 2018) možda prijeloma Protok e-pošte za lokalno ili vanjska odredišta. Kao prethodno communicated da biste pojednostavili upravljanje raspon IP adresa, možemo konsolidirate raspone Exchange Online Protection (EOP) IP adresa koji se koriste za slanje i primanje e-pošte izvan Office 365. Naše analiza pokazuje da jedan ili više e-pošte vanjskog izvora ili odredišta koji ste konfigurirali u poveznici protok pošte nisu prihvaća veze iz u IP adresu raspone prikazana [ovdje](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).
  
Djelovati prije listopad 26th da biste osigurali tih izvora i odredišta će prihvatiti veze i iz sve [objavljene EOP IP adrese](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).
  
Dodatne informacije o ovom promjenom pogledajte poruku centar knjiži [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)ili [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).
  
 **Napomena**: Ako prethodno koristili IP ili URL objavljivanje putem HTML, XML i RSS krajnje točke ažuriranja, možete također treba migrirati u novu web-usluge za automatiziranje te vrste ažuriranja. Dodatne informacije potražite u [Office 365 krajnje točke kategorije i Office 365 IP adresu i URL web-usluge](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).
  

