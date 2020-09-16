---
title: Spremanje web-mjesta ili popisa kao predloška
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: 37ae727aa6dd6af94d0d833ce972aec413d90194
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727523"
---
# <a name="save-site-or-list-as-a-template"></a><span data-ttu-id="9427a-102">Spremanje web-mjesta ili popisa kao predloška</span><span class="sxs-lookup"><span data-stu-id="9427a-102">Save site or list as a template</span></span>

<span data-ttu-id="9427a-103">Predlošci web-mjesta sustava SharePoint pretizgrađene su definicije dizajnirane oko određene poslovne potrebe.</span><span class="sxs-lookup"><span data-stu-id="9427a-103">SharePoint site templates are prebuilt definitions designed around a particular business need.</span></span> <span data-ttu-id="9427a-104">Dodatne informacije potražite u članku [Korištenje predložaka za stvaranje različitih vrsta web-mjesta sustava SharePoint](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span><span class="sxs-lookup"><span data-stu-id="9427a-104">For more information, see [Using templates to create different kinds of SharePoint sites](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span></span>

<span data-ttu-id="9427a-105">Slijede neki Česti problemi/rješenja vezana uz spremanje web-mjesta ili popisa kao predloška u sustavu SharePoint online.</span><span class="sxs-lookup"><span data-stu-id="9427a-105">Here are some common issues/solutions regarding Saving a Site or List as a template in SharePoint Online.</span></span>

<span data-ttu-id="9427a-106">**Gumb Spremi predložak web-mjesta/popisa nije dostupan ili nedostaje**.</span><span class="sxs-lookup"><span data-stu-id="9427a-106">**Save site/list template button is not available or missing**.</span></span> 

- <span data-ttu-id="9427a-107">Administratorima će biti potrebno omogućiti prilagođenu skriptu za omogućivanje značajki predložaka.</span><span class="sxs-lookup"><span data-stu-id="9427a-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="9427a-108">Detaljne upute, primjeri i razmatranja potražite u članku [Omogućivanje i onemogućivanje prilagođene skripte](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="9427a-108">For detailed steps, examples and considerations see [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>


- <span data-ttu-id="9427a-109">Naredba Spremi web-mjesto kao predložak nije podržana i može uzrokovati probleme na web-mjestima koja koriste infrastrukturu za objavljivanje sustava SharePoint Server.</span><span class="sxs-lookup"><span data-stu-id="9427a-109">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>


<span data-ttu-id="9427a-110">**Predložak web-mjesta nije moguće stvoriti ili ne funkcionira pravilno**</span><span class="sxs-lookup"><span data-stu-id="9427a-110">**The site template cannot be created or does not work correctly**</span></span>

- <span data-ttu-id="9427a-111">Predložak možda nema [značajku](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) i neće se aktivirati.</span><span class="sxs-lookup"><span data-stu-id="9427a-111">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won’t activate.</span></span> <span data-ttu-id="9427a-112">Ako značajka nije dostupna za aktivaciju u aktualnoj zbirci web-mjesta, ne možete stvoriti web-mjesto pomoću predloška web-mjesta.</span><span class="sxs-lookup"><span data-stu-id="9427a-112">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>


- <span data-ttu-id="9427a-113">Provjerite prelazi li neki popisi ili biblioteke iznad [praga ograničenja prikaza popisa](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) od 5000 stavki jer to može blokirati stvaranje predloška web-mjesta.</span><span class="sxs-lookup"><span data-stu-id="9427a-113">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>


- <span data-ttu-id="9427a-114">Web-mjesto možda koristi previše resursa, a predložak web-mjesta premašuje ograničenje od 50 megabajta (MB).</span><span class="sxs-lookup"><span data-stu-id="9427a-114">The site may be using too many resources and therefore the site template exceeds the 50 megabyte (MB) limit.</span></span>


- <span data-ttu-id="9427a-115">Postoje problemi s prikazom podataka s popisa koji koristi stupac za pretraživanje.</span><span class="sxs-lookup"><span data-stu-id="9427a-115">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="9427a-116">Dodatne informacije potražite u članku [popis generirani predložak ne prikazuje podatke s odgovarajućeg popisa pretraživanja u sustavu SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span><span class="sxs-lookup"><span data-stu-id="9427a-116">For more information, see [Template-generated list doesn’t display data from the correct lookup list in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span></span>


<span data-ttu-id="9427a-117">Detaljne informacije o uobičajenim problemima i rješenjima potražite u odjeljku [Stvaranje i korištenje predložaka web-mjesta](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span><span class="sxs-lookup"><span data-stu-id="9427a-117">For more detailed information on common problems and solutions please reference, [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>

