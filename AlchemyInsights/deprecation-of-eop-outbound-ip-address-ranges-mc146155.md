---
title: 1065 Deprecation of EOP outbound IP address rangesMC146155
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
ms.openlocfilehash: 214abc57a99c70a02a7d159441713e007f6ad980f67e373780d4ca297f69f764
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54031254"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a>Deprecation of EOP outbound IP address ranges

Otkrili smo potencijalni problem s vašom organizacijom koji (ako se ne ispravi do 26. listopada 2018.) može prekinuti tijek pošte na lokalno ili vanjsko odredište. Kao što smo prethodno komunicirali, da bismo pojednostavnili upravljanje rasponom IP adresa, konsolidiramo raspone IP adresa sustava Exchange Online Protection (EOP) koji se koriste za slanje i primanje e-pošte izvan Microsoft 365. Naša analiza upućuje na to da jedan ili više vanjskih izvora e-pošte ili odredišta koje ste konfigurirali u poveznikima tijeka pošte ne prihvaća veze iz ovdje prikazanih raspona IP [adresa](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

Djeluj prije 26. listopada da bi ti izvori i odredišta prihvaćali veze sa svim objavljenim IP adresama [EOP-a](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)i s njih .

Dodatne informacije o ovoj promjeni potražite u člancima Centar za poruke [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)ili [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).

**Napomena:** ako ste prethodno koristili objavljivanje IP-a ili URL-a putem HTML-a, XML-a i RSS-a za ažuriranja krajnjih točaka, trebali biste migrirati i na nove web-servise radi automatizacije tih vrsta ažuriranja. Dodatne informacije potražite u članku [Microsoft 365 krajnje točke i ip Microsoft 365 i URL web-servisa](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).
