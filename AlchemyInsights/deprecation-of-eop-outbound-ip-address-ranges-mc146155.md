---
title: 1065 Ukidanje raspona izlazne IP adrese EOP-aMC146155
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: f4854c32d970d84f3a0664a9e384dc6e3cd0bfa7
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704589"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a>Ukidanje raspona izlazne IP adrese EOP-a

Otkrili smo potencijalni problem s vašom organizacijom koji (ako se ne ispravi do 26. listopada 2018.) može prekinuti tijek pošte na vaša lokalna ili vanjska odredišta. Kao što je prethodno priopćeno, kako bismo pojednostavili upravljanje rasponima IP adresa ip adresa, konsolidiramo raspone IP adresa exchange online zaštite (EOP) koji se koriste za slanje i primanje e-pošte izvan sustava Microsoft 365. Naša analiza pokazuje da jedan ili više vanjskih izvora e-pošte ili odredišta koja ste konfigurirali u konektorima tijeka pošte ne prihvaćaju veze iz raspona IP adresa koji su [ovdje](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)prikazani .

Zakon prije 26 [.](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)

Dodatne informacije o toj promjeni potražite u članku Postovi centra za poruke [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)ili [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).

**Napomena:** Ako ste prethodno koristili IP ili URL objavljivanje putem HTML-a, XML-a i RSS-a za ažuriranja krajnjih točaka, trebali biste migrirati i na nove web-servise za automatizaciju tih vrsta ažuriranja. Dodatne informacije potražite u članku [Kategorije krajnje točke za Microsoft 365 te IP adresa i URL web-usluga](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).
