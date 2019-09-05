---
title: Stvaranje web-mjesta u SharePoint Online
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: 42430c8dadc17b87dc7741f3fa045ba7c25fab84
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36755300"
---
# <a name="create-sharepoint-sites-using-templates"></a><span data-ttu-id="71b6d-102">Stvaranje SharePoint web-mjesta pomoću predložaka</span><span class="sxs-lookup"><span data-stu-id="71b6d-102">Create SharePoint sites using templates</span></span>

<span data-ttu-id="71b6d-103">Predlošci web-mjesta SharePoint su unaprijed ugrađenih definicije dizajniran oko poslovnih potreba.</span><span class="sxs-lookup"><span data-stu-id="71b6d-103">SharePoint site templates are prebuilt definitions designed around a particular business need.</span></span> <span data-ttu-id="71b6d-104">Za dodatne informacije pogledajte [koristeći predloške za stvaranje različitih vrsta SharePoint web-mjesta](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span><span class="sxs-lookup"><span data-stu-id="71b6d-104">For more information, see [Using templates to create different kinds of SharePoint sites](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span></span>

<span data-ttu-id="71b6d-105">Ovdje su neki uobičajeni problemi/rješenja vezi spremanja na web-mjesto ili popis kao predložak u Sharepoint Online.</span><span class="sxs-lookup"><span data-stu-id="71b6d-105">Here are some common issues/solutions regarding Saving a Site or List as a template in Sharepoint Online.</span></span> 

<span data-ttu-id="71b6d-106">**Gumb Spremi web-mjesta popisu predložak nije dostupan ili nedostaje**</span><span class="sxs-lookup"><span data-stu-id="71b6d-106">**Save site/list template button is not available or missing**</span></span>

<span data-ttu-id="71b6d-107">Administratori morat ćete dopustiti Prilagođena skripta za omogućavanje značajki predloška.</span><span class="sxs-lookup"><span data-stu-id="71b6d-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="71b6d-108">Za detaljne korake Primjeri i razmatranja pogledajte</span><span class="sxs-lookup"><span data-stu-id="71b6d-108">For detailed steps, examples and considerations see</span></span> 

- [<span data-ttu-id="71b6d-109">Omogućavanje ili onemogućavanje prilagođene skripte</span><span class="sxs-lookup"><span data-stu-id="71b6d-109">Allow or prevent custom script</span></span>](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- <span data-ttu-id="71b6d-110">Spremanje web-mjesta kao predloška naredba nije podržana i može uzrokovati probleme na mjestima koja koriste Infrastruktura objavljivanja programa SharePoint Server.</span><span class="sxs-lookup"><span data-stu-id="71b6d-110">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>

<span data-ttu-id="71b6d-111">**Predložak web-mjesta ne može se stvoriti ili ne funkcionira ispravno**</span><span class="sxs-lookup"><span data-stu-id="71b6d-111">**The site template cannot be created or does not work correctly**</span></span>

<span data-ttu-id="71b6d-112">Predložak nedostaje [značajka](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) i nećete aktivirati.</span><span class="sxs-lookup"><span data-stu-id="71b6d-112">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won't activate.</span></span> <span data-ttu-id="71b6d-113">Ako značajka nije dostupna za aktiviranje u trenutnoj zbirci web-mjesta, ne možete koristiti predložak web-mjesta za stvaranje web-mjesta.</span><span class="sxs-lookup"><span data-stu-id="71b6d-113">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>

- <span data-ttu-id="71b6d-114">Provjerite ako popise ili biblioteke premašuju [Prag prikaza popisa ograničenje](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) 5000 stavke kao to možete blokirati stvaranja predloška web-mjesta.</span><span class="sxs-lookup"><span data-stu-id="71b6d-114">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>

- <span data-ttu-id="71b6d-115">Web-mjesto pomoću previše resursa i stoga predložak web-mjesta premašuje ograničenje 50 MB.</span><span class="sxs-lookup"><span data-stu-id="71b6d-115">The site may be using too many resources and therefore the site template exceeds the 50 MB limit.</span></span>


- <span data-ttu-id="71b6d-116">Postoje problemi prikaz podataka s popisa koji koristi stupac za pretraživanje.</span><span class="sxs-lookup"><span data-stu-id="71b6d-116">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="71b6d-117">Dodatne informacije potražite u [popisu predložak generira ne prikazuju podatke iz popis ispravan pretraživanja u SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span><span class="sxs-lookup"><span data-stu-id="71b6d-117">For more information, see [Template-generated list doesn't display data from the correct lookup list in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span></span>

<span data-ttu-id="71b6d-118">Detaljnije informacije o uobičajenih problema i rešenja provjerite [Stvaranje i korištenje predložaka web-mjesta](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span><span class="sxs-lookup"><span data-stu-id="71b6d-118">For more detailed information on common problems and solutions, please check [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>



