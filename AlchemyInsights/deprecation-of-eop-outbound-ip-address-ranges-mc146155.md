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
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a><span data-ttu-id="7c160-102">Razdiobe neizlaznih IP adresa u rasponu</span><span class="sxs-lookup"><span data-stu-id="7c160-102">Deprecation of EOP outbound IP address ranges</span></span>

<span data-ttu-id="7c160-103">Uočili smo potencijalni problem s vašom organizacijom koja (ako nije ispravljena do 26. listopada 2018) može prekinuti tijek pošte na lokalnim ili vanjskim odredištima.</span><span class="sxs-lookup"><span data-stu-id="7c160-103">We've detected a potential issue with your organization that (if not corrected by October 26th, 2018) might break mail flow to your on-premises or external destinations.</span></span> <span data-ttu-id="7c160-104">Kao što je prethodno Priopćeno, da biste pojednostavnili upravljanje rasponom IP Address-a, objedinjujemo raspone IP adresa sustava Exchange Online (EOP) koji se koriste za slanje i primanje e-pošte izvan sustava Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="7c160-104">As previously communicated, to simplify IP address range management, we're consolidating the Exchange Online Protection (EOP) IP address ranges that are used to send and receive email outside of Microsoft 365.</span></span> <span data-ttu-id="7c160-105">Naša analiza upućuje na to da jedan ili više vanjskih izvora e-pošte ili odredišta koje ste konfigurirali u poveznicima tijeka pošte ne prihvaćaju veze iz raspona IP adresa prikazanih [ovdje](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="7c160-105">Our analysis indicates that one or more of the external email sources or destinations that you've configured in mail flow connectors aren't accepting connections from the IP address ranges shown [here](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

<span data-ttu-id="7c160-106">Act prije 26 listopada da bi se osiguralo da će ovi izvori i odredišta prihvatiti veze na sve [objavljene IP adrese](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)i iz njih.</span><span class="sxs-lookup"><span data-stu-id="7c160-106">Act before October 26th to ensure these sources and destinations will accept connections to and from all [published EOP IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

<span data-ttu-id="7c160-107">Dodatne informacije o toj promjeni potražite u članku centar za poruke Posts [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)ili [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span><span class="sxs-lookup"><span data-stu-id="7c160-107">For more information about this change, please see Message Center posts [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620), or [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span></span>

<span data-ttu-id="7c160-108">**Bilješka**: Ako ste prethodno koristili IP ili objavljivanje URL-a putem HTML-a, XML-a i RSS-a za ažuriranja krajnjih točaka, trebali biste migrirati i na nove web-servise radi automatiziranja ovih vrsta ažuriranja.</span><span class="sxs-lookup"><span data-stu-id="7c160-108">**Note**: If you previously used IP or URL publishing via HTML, XML, and RSS for endpoint updates, you also should migrate to the new web services for automating these types of updates.</span></span> <span data-ttu-id="7c160-109">Dodatne informacije potražite u odjeljku [Kategorije krajnjih točaka u sustavu microsoft 365 i web-servisu microsoft 365 IP Address i URL](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span><span class="sxs-lookup"><span data-stu-id="7c160-109">For more information, see [Microsoft 365 endpoint categories and Microsoft 365 IP Address and URL web service](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span></span>
