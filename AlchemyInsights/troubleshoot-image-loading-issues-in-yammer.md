---
title: Otklanjanje problema s učitavanjem slike u servisu Yammer
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
- "6000"
- "9003112"
ms.openlocfilehash: cf330adbf3f3a92d4b90768c7dd8bada6333db80
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690235"
---
# <a name="troubleshoot-image-loading-issues-in-yammer"></a><span data-ttu-id="6a588-102">Otklanjanje problema s učitavanjem slike u servisu Yammer</span><span class="sxs-lookup"><span data-stu-id="6a588-102">Troubleshoot image loading issues in Yammer</span></span>

<span data-ttu-id="6a588-103">Kada se pojave problemi s fotografijama i pretpregledima datoteka u servisu Yammer, riješite poteškoće ako se pojavi problem za sve korisnike, bez obzira na to događa li se na mobilnim uređajima, a ako se prilikom učitavanja privitka može reproducirati.</span><span class="sxs-lookup"><span data-stu-id="6a588-103">When issues occur with photos and file previews in Yammer, troubleshoot by checking whether the issue occurs for all users, whether it occurs on mobile devices, and if it is reproducible when uploading the attachment.</span></span>  

<span data-ttu-id="6a588-104">**Problemi s fotografijom profila**</span><span class="sxs-lookup"><span data-stu-id="6a588-104">**Profile photo issues**</span></span>  

<span data-ttu-id="6a588-105">Ako se krajnji korisnici prijavljuju na Yammer putem programa Microsoft 365, moraju promijeniti svoj profil, uključujući fotografiju profila.</span><span class="sxs-lookup"><span data-stu-id="6a588-105">If end users sign into Yammer via Microsoft 365, they must change their profile, including their profile photo.</span></span> <span data-ttu-id="6a588-106">Ako korisnicima nije dopušteno stvaranje ažuriranja profila, administrator može izvršiti ažuriranje korisnika.</span><span class="sxs-lookup"><span data-stu-id="6a588-106">If users are not permitted to make profile updates, an admin can make the update for the user.</span></span> <span data-ttu-id="6a588-107">Dodatne informacije potražite u članku [Prikaz i ažuriranje profila u sustavu Office delve](https://support.microsoft.com/office/view-and-update-your-profile-in-office-delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba).</span><span class="sxs-lookup"><span data-stu-id="6a588-107">For more info, see [View and update your profile in Office Delve](https://support.microsoft.com/office/view-and-update-your-profile-in-office-delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba).</span></span>

<span data-ttu-id="6a588-108">Informacije o uređivanju profila, uključujući fotografije profila, potražite u članku [Promjena profila i postavki servisa Yammer](https://support.microsoft.com/office/classic-yammer-change-my-yammer-profile-and-settings-a3aeca0e-de34-4897-9b59-de6516542851).</span><span class="sxs-lookup"><span data-stu-id="6a588-108">For info about profile editing, including profile photos, see [Change my Yammer profile and settings](https://support.microsoft.com/office/classic-yammer-change-my-yammer-profile-and-settings-a3aeca0e-de34-4897-9b59-de6516542851).</span></span> 

<span data-ttu-id="6a588-109">Ažurirane fotografije profila sinkroniziraju se drugačije od atributa profila.</span><span class="sxs-lookup"><span data-stu-id="6a588-109">Updated profile photos are synced differently than profile attributes.</span></span> <span data-ttu-id="6a588-110">Korisnici se moraju prijaviti da bi pokrenuli sinkronizaciju fotografije na profilu.</span><span class="sxs-lookup"><span data-stu-id="6a588-110">Users must sign in to initiate a sync of their profile photo.</span></span> <span data-ttu-id="6a588-111">Informacije potražite u članku [slike korisničkog profila ažuriranih iz sustava Office 365 na Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle#q-are-user-profile-pictures-updated-from-office-365-to-yammer).</span><span class="sxs-lookup"><span data-stu-id="6a588-111">For info, see [are user profile pictures updated from Office 365 to Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle#q-are-user-profile-pictures-updated-from-office-365-to-yammer).</span></span>

<span data-ttu-id="6a588-112">Informacije o korisničkom životnom ciklusu za Yammer potražite u članku [Upravljanje korisnicima servisa Yammer u cijelom svom životnom ciklusu iz sustava Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle).</span><span class="sxs-lookup"><span data-stu-id="6a588-112">For info about the user lifecycle for Yammer, see [Manage Yammer users across their lifecycle from Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle).</span></span>  

<span data-ttu-id="6a588-113">Pojedinosti o načinu sinkronizacije profila slika u programu Microsoft 365 potražite u članku [informacije o sinkronizaciji slika profila u programu microsoft 365](https://support.microsoft.com/office/information-about-profile-picture-synchronization-in-microsoft-365-20594d76-d054-4af4-a660-401133e3d48a).</span><span class="sxs-lookup"><span data-stu-id="6a588-113">For details on how profile picture sync works in Microsoft 365, see [Information about profile picture synchronization in Microsoft 365](https://support.microsoft.com/office/information-about-profile-picture-synchronization-in-microsoft-365-20594d76-d054-4af4-a660-401133e3d48a).</span></span>  

<span data-ttu-id="6a588-114">**Problemi s pretpregledima dokumenata i minijaturama slike**</span><span class="sxs-lookup"><span data-stu-id="6a588-114">**Document previews and image thumbnail issues**</span></span>  

<span data-ttu-id="6a588-115">Kada su datoteke ili slike objavljene na servisu Yammer, pretpregled se možda neće prikazivati jer:</span><span class="sxs-lookup"><span data-stu-id="6a588-115">When files or images are posted to Yammer, previews might not appear because:</span></span> 

- <span data-ttu-id="6a588-116">Datoteka je oštećena i nije je moguće obraditi.</span><span class="sxs-lookup"><span data-stu-id="6a588-116">The file is corrupt and cannot be processed.</span></span>
- <span data-ttu-id="6a588-117">Datoteka nije nedavno otpremljena u SharePoint Online ili Yammer sadrži metapodatke koji nisu valjani iz drugih razloga.</span><span class="sxs-lookup"><span data-stu-id="6a588-117">The file has not been recently uploaded to SharePoint Online, or Yammer has invalid metadata for other reasons.</span></span>
- <span data-ttu-id="6a588-118">URL-ovi potrebni za učitavanje slika pretpregleda blokiraju se.</span><span class="sxs-lookup"><span data-stu-id="6a588-118">URLs required for loading the preview images are blocked.</span></span>
- <span data-ttu-id="6a588-119">Korisnik je prije knjiženja uklonio pretpregled datoteke.</span><span class="sxs-lookup"><span data-stu-id="6a588-119">The file preview was removed by the user before posting.</span></span>
- <span data-ttu-id="6a588-120">Problem s servisom spriječio je Pretpregled prikaza.</span><span class="sxs-lookup"><span data-stu-id="6a588-120">A service issue prevented a preview being generated.</span></span>

<span data-ttu-id="6a588-121">**Notes** Pretpregled veza i učitavanja datoteka mogu se ponašati drugačije.</span><span class="sxs-lookup"><span data-stu-id="6a588-121">**Note** Previews for links and file uploads might behave differently.</span></span> <span data-ttu-id="6a588-122">Veze na datoteke na internetu ili veze koje zahtijevaju dodatnu provjeru autentičnosti možda se neće ispravno prikazivati.</span><span class="sxs-lookup"><span data-stu-id="6a588-122">Links to files on the internet or links that require additional authentication might not display correctly.</span></span>

<span data-ttu-id="6a588-123">Dodatne informacije potražite u članku [prilaganje datoteke ili slike poruci servisa Yammer](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-message-f576d4d1-ad66-4ce4-9c43-46cf75978dbf).</span><span class="sxs-lookup"><span data-stu-id="6a588-123">For more info, see [Attach a file or image to a Yammer message](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-message-f576d4d1-ad66-4ce4-9c43-46cf75978dbf).</span></span> 