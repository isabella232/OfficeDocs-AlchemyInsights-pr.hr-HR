---
title: Spremanje web-mjesta ili popisa kao predloška
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: 73a32536995a604c734393c2300b4c9bb507e2b2
ms.sourcegitcommit: 136b8209c52c2a05d0f2fdaab93b2cd92253fa2c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/07/2019
ms.locfileid: "34770520"
---
# <a name="save-site-or-list-as-a-template"></a><span data-ttu-id="28636-102">Spremanje web-mjesta ili popisa kao predloška</span><span class="sxs-lookup"><span data-stu-id="28636-102">Save site or list as a template</span></span>

<span data-ttu-id="28636-103">Predlošci web-mjesta SharePoint su unaprijed ugrađenih definicije dizajniran oko poslovnih potreba.</span><span class="sxs-lookup"><span data-stu-id="28636-103">SharePoint site templates are prebuilt definitions designed around a particular business need.</span></span> <span data-ttu-id="28636-104">Za dodatne informacije pogledajte [koristeći predloške za stvaranje različitih vrsta SharePoint web-mjesta](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span><span class="sxs-lookup"><span data-stu-id="28636-104">For more information, see [Using templates to create different kinds of SharePoint sites](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span></span>

<span data-ttu-id="28636-105">Ovdje su neki uobičajeni problemi/rješenja vezi spremanja na web-mjesto ili popis kao predložak u SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="28636-105">Here are some common issues/solutions regarding Saving a Site or List as a template in SharePoint Online.</span></span>

<span data-ttu-id="28636-106">**Spremanje web-mjesta popisu predložak je gumb nije dostupan ili nedostaje**.</span><span class="sxs-lookup"><span data-stu-id="28636-106">**Save site/list template button is not available or missing**.</span></span> 

- <span data-ttu-id="28636-107">Administratori morat ćete dopustiti Prilagođena skripta za omogućavanje značajki predloška.</span><span class="sxs-lookup"><span data-stu-id="28636-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="28636-108">Za detaljne korake, Primjeri i razmatranja pogledajte [Dopusti ili spriječiti prilagođene skripte](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="28636-108">For detailed steps, examples and considerations see [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>


- <span data-ttu-id="28636-109">Spremanje web-mjesta kao predloška naredba nije podržana i može uzrokovati probleme na mjestima koja koriste Infrastruktura objavljivanja programa SharePoint Server.</span><span class="sxs-lookup"><span data-stu-id="28636-109">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>


<span data-ttu-id="28636-110">**Predložak web-mjesta ne može se stvoriti ili ne funkcionira ispravno**</span><span class="sxs-lookup"><span data-stu-id="28636-110">**The site template cannot be created or does not work correctly**</span></span>

- <span data-ttu-id="28636-111">Predložak nedostaje [značajka](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) i nećete aktivirati.</span><span class="sxs-lookup"><span data-stu-id="28636-111">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won’t activate.</span></span> <span data-ttu-id="28636-112">Ako značajka nije dostupna za aktiviranje u trenutnoj zbirci web-mjesta, ne možete koristiti predložak web-mjesta za stvaranje web-mjesta.</span><span class="sxs-lookup"><span data-stu-id="28636-112">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>


- <span data-ttu-id="28636-113">Provjerite ako popise ili biblioteke premašuju [Prag prikaza popisa ograničenje](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) 5000 stavke kao to možete blokirati stvaranja predloška web-mjesta.</span><span class="sxs-lookup"><span data-stu-id="28636-113">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>


- <span data-ttu-id="28636-114">Web-mjesto pomoću previše resursa i stoga predložak web-mjesta prelazi ograničenje od 50 megabajta (MB).</span><span class="sxs-lookup"><span data-stu-id="28636-114">The site may be using too many resources and therefore the site template exceeds the 50 megabyte (MB) limit.</span></span>


- <span data-ttu-id="28636-115">Postoje problemi prikaz podataka s popisa koji koristi stupac za pretraživanje.</span><span class="sxs-lookup"><span data-stu-id="28636-115">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="28636-116">Dodatne informacije potražite u [popisu predložak generira ne prikazuju podatke iz popis ispravan pretraživanja u SharePoint Online](https://support.office.com/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a).</span><span class="sxs-lookup"><span data-stu-id="28636-116">For more information, see [Template-generated list doesn’t display data from the correct lookup list in SharePoint Online](https://support.office.com/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a).</span></span>


<span data-ttu-id="28636-117">Za detaljnije informacije o uobičajene probleme i rješenja Molim referenca, [Stvaranje i korištenje predložaka web-mjesta](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span><span class="sxs-lookup"><span data-stu-id="28636-117">For more detailed information on common problems and solutions please reference, [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>

