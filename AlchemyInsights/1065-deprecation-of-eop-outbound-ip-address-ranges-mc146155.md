---
title: 1065 postupku EOP izlaznog IP adresa rangesMC146155
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 9/28/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: ec87141ffaa2fa3484620a9b52851e3e92f20b6b
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29462072"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a><span data-ttu-id="0e347-102">Postupku EOP izlaznog IP adresu raspona</span><span class="sxs-lookup"><span data-stu-id="0e347-102">Deprecation of EOP outbound IP address ranges</span></span>

<span data-ttu-id="0e347-p101">Možemo ste otkrio mogući problem s vaše organizacije (Ako ne ispravlja po listopad 26th, 2018) možda prijeloma Protok e-pošte za lokalno ili vanjska odredišta. Kao prethodno communicated da biste pojednostavili upravljanje raspon IP adresa, možemo konsolidirate raspone Exchange Online Protection (EOP) IP adresa koji se koriste za slanje i primanje e-pošte izvan Office 365. Naše analiza pokazuje da jedan ili više e-pošte vanjskog izvora ili odredišta koji ste konfigurirali u poveznici protok pošte nisu prihvaća veze iz u IP adresu raspone prikazana [ovdje](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="0e347-p101">We've detected a potential issue with your organization that (if not corrected by October 26th, 2018) might break mail flow to your on-premises or external destinations. As previously communicated, to simplify IP address range management, we're consolidating the Exchange Online Protection (EOP) IP address ranges that are used to send and receive email outside of Office 365. Our analysis indicates that one or more of the external email sources or destinations that you've configured in mail flow connectors aren't accepting connections from the IP address ranges shown [here](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>
  
<span data-ttu-id="0e347-106">Djelovati prije listopad 26th da biste osigurali tih izvora i odredišta će prihvatiti veze i iz sve [objavljene EOP IP adrese](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="0e347-106">Act before October 26th to ensure these sources and destinations will accept connections to and from all [published EOP IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>
  
<span data-ttu-id="0e347-107">Dodatne informacije o ovom promjenom pogledajte poruku centar knjiži [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)ili [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span><span class="sxs-lookup"><span data-stu-id="0e347-107">For more information about this change, please see Message Center posts [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620), or [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span></span>
  
 <span data-ttu-id="0e347-p102">**Napomena**: Ako prethodno koristili IP ili URL objavljivanje putem HTML, XML i RSS krajnje točke ažuriranja, možete također treba migrirati u novu web-usluge za automatiziranje te vrste ažuriranja. Dodatne informacije potražite u [Office 365 krajnje točke kategorije i Office 365 IP adresu i URL web-usluge](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span><span class="sxs-lookup"><span data-stu-id="0e347-p102">**Note**: If you previously used IP or URL publishing via HTML, XML, and RSS for endpoint updates, you also should migrate to the new web services for automating these types of updates. For more information, see [Office 365 endpoint categories and Office 365 IP Address and URL web service](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span></span>
  

