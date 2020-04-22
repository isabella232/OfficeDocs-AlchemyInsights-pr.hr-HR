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
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a><span data-ttu-id="ba822-102">Ukidanje raspona izlazne IP adrese EOP-a</span><span class="sxs-lookup"><span data-stu-id="ba822-102">Deprecation of EOP outbound IP address ranges</span></span>

<span data-ttu-id="ba822-103">Otkrili smo potencijalni problem s vašom organizacijom koji (ako se ne ispravi do 26. listopada 2018.) može prekinuti tijek pošte na vaša lokalna ili vanjska odredišta.</span><span class="sxs-lookup"><span data-stu-id="ba822-103">We've detected a potential issue with your organization that (if not corrected by October 26th, 2018) might break mail flow to your on-premises or external destinations.</span></span> <span data-ttu-id="ba822-104">Kao što je prethodno priopćeno, kako bismo pojednostavili upravljanje rasponima IP adresa ip adresa, konsolidiramo raspone IP adresa exchange online zaštite (EOP) koji se koriste za slanje i primanje e-pošte izvan sustava Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="ba822-104">As previously communicated, to simplify IP address range management, we're consolidating the Exchange Online Protection (EOP) IP address ranges that are used to send and receive email outside of Microsoft 365.</span></span> <span data-ttu-id="ba822-105">Naša analiza pokazuje da jedan ili više vanjskih izvora e-pošte ili odredišta koja ste konfigurirali u konektorima tijeka pošte ne prihvaćaju veze iz raspona IP adresa koji su [ovdje](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)prikazani .</span><span class="sxs-lookup"><span data-stu-id="ba822-105">Our analysis indicates that one or more of the external email sources or destinations that you've configured in mail flow connectors aren't accepting connections from the IP address ranges shown [here](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

<span data-ttu-id="ba822-106">Zakon prije 26 [.](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)</span><span class="sxs-lookup"><span data-stu-id="ba822-106">Act before October 26th to ensure these sources and destinations will accept connections to and from all [published EOP IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

<span data-ttu-id="ba822-107">Dodatne informacije o toj promjeni potražite u članku Postovi centra za poruke [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)ili [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span><span class="sxs-lookup"><span data-stu-id="ba822-107">For more information about this change, please see Message Center posts [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620), or [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span></span>

<span data-ttu-id="ba822-108">**Napomena:** Ako ste prethodno koristili IP ili URL objavljivanje putem HTML-a, XML-a i RSS-a za ažuriranja krajnjih točaka, trebali biste migrirati i na nove web-servise za automatizaciju tih vrsta ažuriranja.</span><span class="sxs-lookup"><span data-stu-id="ba822-108">**Note**: If you previously used IP or URL publishing via HTML, XML, and RSS for endpoint updates, you also should migrate to the new web services for automating these types of updates.</span></span> <span data-ttu-id="ba822-109">Dodatne informacije potražite u članku [Kategorije krajnje točke za Microsoft 365 te IP adresa i URL web-usluga](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span><span class="sxs-lookup"><span data-stu-id="ba822-109">For more information, see [Microsoft 365 endpoint categories and Microsoft 365 IP Address and URL web service](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span></span>
