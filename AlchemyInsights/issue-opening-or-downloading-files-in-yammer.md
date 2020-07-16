---
title: Problem s otvaranjem ili preuzimanjem datoteka na sustavu Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6041"
- "9003112"
ms.openlocfilehash: 6dfcbe9abfc23219a61e81785d31c11f7a0fa95c
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148184"
---
# <a name="issue-opening-or-downloading-files-in-yammer"></a><span data-ttu-id="f74fa-102">Problem s otvaranjem ili preuzimanjem datoteka na sustavu Yammer</span><span class="sxs-lookup"><span data-stu-id="f74fa-102">Issue opening or downloading files in Yammer</span></span>

<span data-ttu-id="f74fa-103">Klasični Yammer podržava više mogućnosti za prijenos datoteka u poruke i grupe.</span><span class="sxs-lookup"><span data-stu-id="f74fa-103">Classic Yammer supports multiple option for file uploads to messages and groups.</span></span> <span data-ttu-id="f74fa-104">Ovisno o konfiguraciji mreže, datoteke zadane za pohranu u sustavu SharePoint.</span><span class="sxs-lookup"><span data-stu-id="f74fa-104">Depending on network configuration, files default to storage in SharePoint.</span></span>

<span data-ttu-id="f74fa-105">Birač datoteka u novom programu Yammer još ne podržava sve mogućnosti dostupne u klasičnom programu Yammer.</span><span class="sxs-lookup"><span data-stu-id="f74fa-105">The file picker in new Yammer does not yet support all the options available in classic Yammer.</span></span> <span data-ttu-id="f74fa-106">Buduće ažuriranje dodat će dodatne značajke.</span><span class="sxs-lookup"><span data-stu-id="f74fa-106">A future update will add additional features.</span></span> <span data-ttu-id="f74fa-107">Dodatne informacije potražite u [odjeljku Prilaganje datoteke ili slike objavi razgovora na yammeru](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-conversation-post-8d2d17f7-8f37-4535-961e-518d751be7e8).</span><span class="sxs-lookup"><span data-stu-id="f74fa-107">For more info, see [Attach a file or image to a Yammer conversation post](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-conversation-post-8d2d17f7-8f37-4535-961e-518d751be7e8).</span></span>

<span data-ttu-id="f74fa-108">**Nije moguće otvoriti ili preuzeti datoteku**</span><span class="sxs-lookup"><span data-stu-id="f74fa-108">**Unable to open or download a file**</span></span>  

<span data-ttu-id="f74fa-109">Datoteka se može prenijeti na Yammer, ali se povezuje i s datotekom u sustavu SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="f74fa-109">A file might upload to Yammer but also be linking to a file in SharePoint Online.</span></span> <span data-ttu-id="f74fa-110">Da biste otklonili poteškoće, najprije morate odrediti mjesto datoteke.</span><span class="sxs-lookup"><span data-stu-id="f74fa-110">To troubleshoot, first you must determine the location of the file.</span></span> <span data-ttu-id="f74fa-111">Ako je datoteka prenesena na Yammer, imat će \*.yammer.com URL.</span><span class="sxs-lookup"><span data-stu-id="f74fa-111">If the file has been uploaded to Yammer, it will have a \*.yammer.com URL.</span></span> <span data-ttu-id="f74fa-112">Provjerite jesu li potrebni URL-ovi i IP adrese deblokirani.</span><span class="sxs-lookup"><span data-stu-id="f74fa-112">Ensure that required URLs and IP addresses are unblocked.</span></span> <span data-ttu-id="f74fa-113">Dodatne informacije potražite u članku na blogu [Korištenje tvrdih kodiranih IP adresa za Yammer ne preporučuje se](https://techcommunity.microsoft.com/t5/yammer-blog/using-hard-coded-ip-addresses-for-yammer-is-not-recommended/ba-p/276592).</span><span class="sxs-lookup"><span data-stu-id="f74fa-113">For more info, see the blog post [Using hard coded IP addresses for Yammer is not recommended](https://techcommunity.microsoft.com/t5/yammer-blog/using-hard-coded-ip-addresses-for-yammer-is-not-recommended/ba-p/276592).</span></span>

<span data-ttu-id="f74fa-114">Provjerite može li korisnik koji je također globalni administrator preuzeti datoteku.</span><span class="sxs-lookup"><span data-stu-id="f74fa-114">Check whether a user who is also a global admin can download the file.</span></span> <span data-ttu-id="f74fa-115">Ako je datoteka privatna, možda ćete morati koristiti način privatnog sadržaja.</span><span class="sxs-lookup"><span data-stu-id="f74fa-115">If the file is private, you might have to use Private Content Mode.</span></span> <span data-ttu-id="f74fa-116">Dodatne informacije potražite [u odjeljku Nadzor privatnog sadržaja na web-mjestu Yammer](https://docs.microsoft.com/yammer/manage-security-and-compliance/monitor-private-content).</span><span class="sxs-lookup"><span data-stu-id="f74fa-116">For more info, see then [Monitor private content in Yammer](https://docs.microsoft.com/yammer/manage-security-and-compliance/monitor-private-content).</span></span>  

<span data-ttu-id="f74fa-117">**Gosti i datoteke na razini mreže servisa Yammer u sustavu SharePoint Online**</span><span class="sxs-lookup"><span data-stu-id="f74fa-117">**Yammer network-level guests and files in SharePoint Online**</span></span>  

<span data-ttu-id="f74fa-118">[Gosti na razini mreže na servisu Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#invite-guests) ne koriste Azure AD B2B i interni su za servis Servisa Yammer pa ne mogu pristupiti datotekama servisa Yammer pohranjenima u sustavu SharePoint.</span><span class="sxs-lookup"><span data-stu-id="f74fa-118">[Network-level guests in Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#invite-guests) do not use Azure AD B2B and are internal to the Yammer service, so they can't access Yammer files stored in SharePoint.</span></span> <span data-ttu-id="f74fa-119">Pomoću tog identiteta stvorite vanjskog korisnika AAD B2B koji može pristupiti bibliotekama dokumenata u sustavu SharePoint Online pomoću tog identiteta.</span><span class="sxs-lookup"><span data-stu-id="f74fa-119">Create an external AAD B2B user who can access document libraries in SharePoint Online by using that identity.</span></span> <span data-ttu-id="f74fa-120">Informacije o budućoj podršci za goste za Azure AD B2B na servisu Yammer potražite u članku [Podrška za korisnike između tvrtke (B2B) u pretpregledu servisa Yammer – Uvjeti i najčešća pitanja o klijentima](https://docs.microsoft.com/yammer/get-started-with-yammer/azure-ad-b2b-guests-yammer).</span><span class="sxs-lookup"><span data-stu-id="f74fa-120">For information about future Azure AD B2B guest support in Yammer, see [Business-to-business (B2B) Guest support in Yammer Preview - Customer Terms and FAQ](https://docs.microsoft.com/yammer/get-started-with-yammer/azure-ad-b2b-guests-yammer).</span></span>