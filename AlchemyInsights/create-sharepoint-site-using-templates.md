---
title: Stvaranje web-mjesta u sustavu SharePoint Online
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: b9009fdbdc2a5e7443151446daade1685d2f5d45
ms.sourcegitcommit: 317eeed39c7777a922442992d67733726c41d9e1
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 02/04/2020
ms.locfileid: "41770415"
---
# <a name="create-sharepoint-sites-using-templates"></a><span data-ttu-id="fed0b-102">Stvaranje SharePoint web-mjesta pomoću predložaka</span><span class="sxs-lookup"><span data-stu-id="fed0b-102">Create SharePoint sites using templates</span></span>

<span data-ttu-id="fed0b-103">Mogućnost spremanja web-mjesta kao predloška nije podržana s modernom komunikacijom ili tim web-lokacijama.</span><span class="sxs-lookup"><span data-stu-id="fed0b-103">The ability to save a site as a template is not supported with modern Communication or Team Sites.</span></span> <span data-ttu-id="fed0b-104">Dodatne informacije o korištenju predložaka potražite u okviru [Spremi, Preuzmite i prenesite SharePoint web-mjesto kao predložak](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).</span><span class="sxs-lookup"><span data-stu-id="fed0b-104">For more information about using templates see [Save, download and upload a SharePoint site as a template](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).</span></span>

<span data-ttu-id="fed0b-105">Evo nekih uobičajenih problema/rješenja vezanih uz spremanje web-mjesta ili popisa kao predloška u sustavu SharePoint online.</span><span class="sxs-lookup"><span data-stu-id="fed0b-105">Here are some common issues/solutions regarding Saving a Site or List as a template in Sharepoint Online.</span></span> 

<span data-ttu-id="fed0b-106">**Spremanje gumba predloška web-mjesta/popisa nije dostupno ili nedostaje**</span><span class="sxs-lookup"><span data-stu-id="fed0b-106">**Save site/list template button is not available or missing**</span></span>

<span data-ttu-id="fed0b-107">Administratori će morati dopustiti prilagođenoj skripti da omogući značajke predloška.</span><span class="sxs-lookup"><span data-stu-id="fed0b-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="fed0b-108">Za detaljne korake, primjeri i razmatranja vide</span><span class="sxs-lookup"><span data-stu-id="fed0b-108">For detailed steps, examples and considerations see</span></span> 

- [<span data-ttu-id="fed0b-109">Dopusti ili spriječi prilagođenu skriptu</span><span class="sxs-lookup"><span data-stu-id="fed0b-109">Allow or prevent custom script</span></span>](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- <span data-ttu-id="fed0b-110">Naredba Spremi web-mjesto kao predložak nije podržana i može uzrokovati probleme na web-lokacijama koje koriste SharePoint Server Publishing je infrastruktura.</span><span class="sxs-lookup"><span data-stu-id="fed0b-110">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>

<span data-ttu-id="fed0b-111">**Predložak web-mjesta nije moguće stvoriti ili ne radi ispravno**</span><span class="sxs-lookup"><span data-stu-id="fed0b-111">**The site template cannot be created or does not work correctly**</span></span>

<span data-ttu-id="fed0b-112">Predlošku možda nedostaje [značajka](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) i neće se aktivirati.</span><span class="sxs-lookup"><span data-stu-id="fed0b-112">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won't activate.</span></span> <span data-ttu-id="fed0b-113">Ako značajka nije dostupna za aktivaciju u trenutnoj zbirci web-mjesta, ne možete koristiti predložak web-mjesta za stvaranje web-mjesta.</span><span class="sxs-lookup"><span data-stu-id="fed0b-113">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>

- <span data-ttu-id="fed0b-114">Provjerite prelazi li neki popisi ili biblioteke prekoračiti [prag ograničenja prikaza popisa](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) od 5000 artikala jer to može blokirati stvaranje predloška web-mjesta.</span><span class="sxs-lookup"><span data-stu-id="fed0b-114">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>

- <span data-ttu-id="fed0b-115">Web-mjesto možda koristi previše resursa i stoga predložak web-mjesta premašuje ograničenje od 50 MB.</span><span class="sxs-lookup"><span data-stu-id="fed0b-115">The site may be using too many resources and therefore the site template exceeds the 50 MB limit.</span></span>


- <span data-ttu-id="fed0b-116">Postoje problemi s prikazom podataka s popisa koji koristi stupac za pretraživanje.</span><span class="sxs-lookup"><span data-stu-id="fed0b-116">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="fed0b-117">Dodatne informacije potražite [u prikazu popisa koji se generiraju predlošcima ne prikazuju se podaci s ispravnog popisa pretraživanja u sustavu SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span><span class="sxs-lookup"><span data-stu-id="fed0b-117">For more information, see [Template-generated list doesn't display data from the correct lookup list in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span></span>

<span data-ttu-id="fed0b-118">Za detaljnije informacije o zajedničkim problemima i rješenjima, provjerite [stvorite i koristite predloške web-mjesta](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span><span class="sxs-lookup"><span data-stu-id="fed0b-118">For more detailed information on common problems and solutions, please check [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>



