---
title: Premještanje poruka e-pošte arhiva poštanskog sandučića
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: fb5745b60d42e1f7d7bb9b7a336a51b62c2ff92a
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/07/2019
ms.locfileid: "34762357"
---
# <a name="move-email-to-the-archive-mailbox"></a><span data-ttu-id="eec7b-102">Premjesti e-pošta poštanski sandučić arhiva</span><span class="sxs-lookup"><span data-stu-id="eec7b-102">Move email to the archive mailbox</span></span>
 
1. <span data-ttu-id="eec7b-103">Potvrdite da je **arhiviranje poštanski sandučić** je omogućeno.</span><span class="sxs-lookup"><span data-stu-id="eec7b-103">Confirm that an **Archive mailbox** has been enabled.</span></span> <span data-ttu-id="eec7b-104">Ako nije, slijedite korake u [ovom članku](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) da biste omogućili arhiva poštanski sandučić.</span><span class="sxs-lookup"><span data-stu-id="eec7b-104">If not, use the steps in [this article](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span>

2. <span data-ttu-id="eec7b-105">Za arhiviranje poruka automatski u poštanski sandučić arhiva zadržavanja oznaka s akcijom **premjestiti za arhiviranje** mora biti postavljen da **automatski primijeniti oznaka cijeli sandučić (zadano)**.</span><span class="sxs-lookup"><span data-stu-id="eec7b-105">To archive messages automatically to the archive mailbox, a retention tag with the **Move to archive** action must be set to **applied automatically to entire mailbox (default) tag**.</span></span> <span data-ttu-id="eec7b-106">Ovdje koristite korake za stvaranje oznaka: [arhiva zadana oznaka](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fdocs.microsoft.com%2Fen-us%2Foffice365%2Fsecuritycompliance%2Fset-up-an-archive-and-deletion-policy-for-mailboxes%23create-a-custom-archive-default-policy-tag&data=04%7C01%7Cstephow%40microsoft.com%7C89934e16dbd84ebdef6708d6b319b348%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636893320296576506%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C-1&sdata=UibWi%2BtrO3ITZ6iF%2FtKQj5JyxzEb9Mu9frBJPT6FNFI%3D&reserved=0).</span><span class="sxs-lookup"><span data-stu-id="eec7b-106">Use the steps here to create the tag: [Archive Default tag](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fdocs.microsoft.com%2Fen-us%2Foffice365%2Fsecuritycompliance%2Fset-up-an-archive-and-deletion-policy-for-mailboxes%23create-a-custom-archive-default-policy-tag&data=04%7C01%7Cstephow%40microsoft.com%7C89934e16dbd84ebdef6708d6b319b348%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636893320296576506%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C-1&sdata=UibWi%2BtrO3ITZ6iF%2FtKQj5JyxzEb9Mu9frBJPT6FNFI%3D&reserved=0).</span></span>
    
3. <span data-ttu-id="eec7b-107">Dalje, dodajte oznaku **arhiva** pravila zadržavanja.</span><span class="sxs-lookup"><span data-stu-id="eec7b-107">Next, add the **Archive** tag to your retention policy.</span></span> <span data-ttu-id="eec7b-108">U centru za administraciju Exchange odaberite **Pravila zadržavanja** > dodavanje **Premještanje arhiva oznaku** > pravila **spremiti**.</span><span class="sxs-lookup"><span data-stu-id="eec7b-108">In the Exchange admin center, choose **Retention Policies** > add the **Move to Archive tag** to the policy > **Save**.</span></span> 
    
4. <span data-ttu-id="eec7b-109">Sada [dodijeliti pravila zadržavanja](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) poštanski sandučić određenog korisnika.</span><span class="sxs-lookup"><span data-stu-id="eec7b-109">Now [Assign the Retention Policy](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox.</span></span> <span data-ttu-id="eec7b-110">Ista pravila primijenit će se na **primarni** i poštanski sandučić **arhiva** .</span><span class="sxs-lookup"><span data-stu-id="eec7b-110">The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span> 
    
<span data-ttu-id="eec7b-111">Možda će biti potrebno da biste prisilili na upravljana mapa pomoćnika (MFA) za pokretanje i primijeniti nove postavke u korisnički poštanski sandučić.</span><span class="sxs-lookup"><span data-stu-id="eec7b-111">It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox.</span></span> <span data-ttu-id="eec7b-112">Pokrenite sljedeću naredbu tijekom [povezani EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) za pokretanje upravljanih Pomoćnik za mape za određene poštanski sandučić:</span><span class="sxs-lookup"><span data-stu-id="eec7b-112">Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span> 
  
```
Start-ManagedFolderAssistant -Identity <name of the mailbox>
```

<span data-ttu-id="eec7b-113">Za dodatne informacije o postavljanju pravila arhiviranja pogledajte [Postavljanje arhiva i brisanje pravila za poštanske sandučiće](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span><span class="sxs-lookup"><span data-stu-id="eec7b-113">For more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  

