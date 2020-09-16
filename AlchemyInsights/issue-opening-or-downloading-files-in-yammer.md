---
title: Otvaranje i preuzimanje datoteka u servisu Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6041"
- "9003112"
ms.openlocfilehash: de335e27624caf5a91bdc2913570eba92f627282
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695641"
---
# <a name="issue-opening-or-downloading-files-in-yammer"></a><span data-ttu-id="512f4-102">Otvaranje i preuzimanje datoteka u servisu Yammer</span><span class="sxs-lookup"><span data-stu-id="512f4-102">Issue opening or downloading files in Yammer</span></span>

<span data-ttu-id="512f4-103">Klasični Yammer podržava više mogućnosti za prijenos datoteka na poruke i grupe.</span><span class="sxs-lookup"><span data-stu-id="512f4-103">Classic Yammer supports multiple option for file uploads to messages and groups.</span></span> <span data-ttu-id="512f4-104">Ovisno o konfiguraciji mreže, datoteke će biti zadane za pohranu u sustavu SharePoint.</span><span class="sxs-lookup"><span data-stu-id="512f4-104">Depending on network configuration, files default to storage in SharePoint.</span></span>

<span data-ttu-id="512f4-105">Birač datoteka u novom Yammeru još ne podržava sve mogućnosti dostupne u klasičnom Yammeru.</span><span class="sxs-lookup"><span data-stu-id="512f4-105">The file picker in new Yammer does not yet support all the options available in classic Yammer.</span></span> <span data-ttu-id="512f4-106">Ubuduće će se ažurirati dodavanjem dodatnih značajki.</span><span class="sxs-lookup"><span data-stu-id="512f4-106">A future update will add additional features.</span></span> <span data-ttu-id="512f4-107">Dodatne informacije potražite u članku [prilaganje datoteke ili slike u objavu razgovora u servisu Yammer](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-conversation-post-8d2d17f7-8f37-4535-961e-518d751be7e8).</span><span class="sxs-lookup"><span data-stu-id="512f4-107">For more info, see [Attach a file or image to a Yammer conversation post](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-conversation-post-8d2d17f7-8f37-4535-961e-518d751be7e8).</span></span>

<span data-ttu-id="512f4-108">**Nije moguće otvoriti ili preuzeti datoteku**</span><span class="sxs-lookup"><span data-stu-id="512f4-108">**Unable to open or download a file**</span></span>  

<span data-ttu-id="512f4-109">Datoteka se može prenijeti na Yammer, ali i povezati se s datotekom u sustavu SharePoint online.</span><span class="sxs-lookup"><span data-stu-id="512f4-109">A file might upload to Yammer but also be linking to a file in SharePoint Online.</span></span> <span data-ttu-id="512f4-110">Da biste otklonili poteškoće, najprije morate odrediti mjesto datoteke.</span><span class="sxs-lookup"><span data-stu-id="512f4-110">To troubleshoot, first you must determine the location of the file.</span></span> <span data-ttu-id="512f4-111">Ako je datoteka prenesena na Yammer, imat će URL \*. yammer.com.</span><span class="sxs-lookup"><span data-stu-id="512f4-111">If the file has been uploaded to Yammer, it will have a \*.yammer.com URL.</span></span> <span data-ttu-id="512f4-112">Provjerite jesu li obavezni URL-ovi i IP adrese neblokirani.</span><span class="sxs-lookup"><span data-stu-id="512f4-112">Ensure that required URLs and IP addresses are unblocked.</span></span> <span data-ttu-id="512f4-113">Dodatne informacije potražite u članku objava bloga [pomoću tvrdih kodirane IP adrese za Yammer](https://techcommunity.microsoft.com/t5/yammer-blog/using-hard-coded-ip-addresses-for-yammer-is-not-recommended/ba-p/276592).</span><span class="sxs-lookup"><span data-stu-id="512f4-113">For more info, see the blog post [Using hard coded IP addresses for Yammer is not recommended](https://techcommunity.microsoft.com/t5/yammer-blog/using-hard-coded-ip-addresses-for-yammer-is-not-recommended/ba-p/276592).</span></span>

<span data-ttu-id="512f4-114">Provjerite je li korisnik koji je također globalni administrator mogao preuzeti datoteku.</span><span class="sxs-lookup"><span data-stu-id="512f4-114">Check whether a user who is also a global admin can download the file.</span></span> <span data-ttu-id="512f4-115">Ako je datoteka privatna, možda ćete morati koristiti način osobnog sadržaja.</span><span class="sxs-lookup"><span data-stu-id="512f4-115">If the file is private, you might have to use Private Content Mode.</span></span> <span data-ttu-id="512f4-116">Dodatne informacije potražite [u članku praćenje privatnog sadržaja u servisu Yammer](https://docs.microsoft.com/yammer/manage-security-and-compliance/monitor-private-content).</span><span class="sxs-lookup"><span data-stu-id="512f4-116">For more info, see then [Monitor private content in Yammer](https://docs.microsoft.com/yammer/manage-security-and-compliance/monitor-private-content).</span></span>  

<span data-ttu-id="512f4-117">**Gosti i datoteke na razini servisa Yammer u sustavu SharePoint Online**</span><span class="sxs-lookup"><span data-stu-id="512f4-117">**Yammer network-level guests and files in SharePoint Online**</span></span>  

<span data-ttu-id="512f4-118">[Gosti na razini mreže u servisu Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#invite-guests) ne koriste tvrtke Azure ad B2B i interni su za servis servisa Yammer, tako da ne mogu pristupiti datotekama servisa Yammer pohranjenima u sustavu SharePoint.</span><span class="sxs-lookup"><span data-stu-id="512f4-118">[Network-level guests in Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#invite-guests) do not use Azure AD B2B and are internal to the Yammer service, so they can't access Yammer files stored in SharePoint.</span></span> <span data-ttu-id="512f4-119">Stvaranje vanjskog servisa AAD B2B korisnika koji može pristupati bibliotekama dokumenata u sustavu SharePoint Online pomoću tog identiteta.</span><span class="sxs-lookup"><span data-stu-id="512f4-119">Create an external AAD B2B user who can access document libraries in SharePoint Online by using that identity.</span></span> <span data-ttu-id="512f4-120">Informacije o budućoj podršci za podršku za Azure AD B2B u servisu Yammer potražite [u članku Podrška za tvrtke – poslovno (B2B) u pretpregledu servisa Yammer – uvjeti kupaca i najčešća pitanja](https://docs.microsoft.com/yammer/get-started-with-yammer/azure-ad-b2b-guests-yammer).</span><span class="sxs-lookup"><span data-stu-id="512f4-120">For information about future Azure AD B2B guest support in Yammer, see [Business-to-business (B2B) Guest support in Yammer Preview - Customer Terms and FAQ](https://docs.microsoft.com/yammer/get-started-with-yammer/azure-ad-b2b-guests-yammer).</span></span>