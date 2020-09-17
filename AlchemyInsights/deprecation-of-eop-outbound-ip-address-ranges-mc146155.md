---
title: 1065 depretacija servisa za odlazne IP adrese u programu rangesMC146155
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: afd725668f906339f4b7d769bb67a4d2ee5a6ac6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806787"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a>Razdiobe neizlaznih IP adresa u rasponu

Uočili smo potencijalni problem s vašom organizacijom koja (ako nije ispravljena do 26. listopada 2018) može prekinuti tijek pošte na lokalnim ili vanjskim odredištima. Kao što je prethodno Priopćeno, da biste pojednostavnili upravljanje rasponom IP Address-a, objedinjujemo raspone IP adresa sustava Exchange Online (EOP) koji se koriste za slanje i primanje e-pošte izvan sustava Microsoft 365. Naša analiza upućuje na to da jedan ili više vanjskih izvora e-pošte ili odredišta koje ste konfigurirali u poveznicima tijeka pošte ne prihvaćaju veze iz raspona IP adresa prikazanih [ovdje](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

Act prije 26 listopada da bi se osiguralo da će ovi izvori i odredišta prihvatiti veze na sve [objavljene IP adrese](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)i iz njih.

Dodatne informacije o toj promjeni potražite u članku centar za poruke Posts [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)ili [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).

**Bilješka**: Ako ste prethodno koristili IP ili objavljivanje URL-a putem HTML-a, XML-a i RSS-a za ažuriranja krajnjih točaka, trebali biste migrirati i na nove web-servise radi automatiziranja ovih vrsta ažuriranja. Dodatne informacije potražite u odjeljku [Kategorije krajnjih točaka u sustavu microsoft 365 i web-servisu microsoft 365 IP Address i URL](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).
