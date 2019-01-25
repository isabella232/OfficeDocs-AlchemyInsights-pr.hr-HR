---
title: Premještanje poruka e-pošte arhiva poštanskog sandučića
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 41d6825b568263fb7b09066b65235aa348415bae
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29461811"
---
<span data-ttu-id="64aa5-p101">Problematična arhiviranje stavki u arhivu poštanski sandučić. Provjerite je li obavite sljedeće korake:</span><span class="sxs-lookup"><span data-stu-id="64aa5-p101">Having problems archiving items to the Archive mailbox. Make sure you have performed the following steps:</span></span>
  
1. <span data-ttu-id="64aa5-p102">Potvrdite da je **arhiviranje poštanski sandučić** je omogućeno. Ako nije, koristite korake u [ovom članku](https://docs.microsoft.com/en-us/office365/securitycompliance/enable-archive-mailboxes) da biste omogućili arhiva poštanskog sandučića.</span><span class="sxs-lookup"><span data-stu-id="64aa5-p102">Confirm that an **Archive mailbox** has been enabled. If not, use steps in [this article](https://docs.microsoft.com/en-us/office365/securitycompliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span> 
    
2. <span data-ttu-id="64aa5-106">U centru za administraciju Exchange odaberite **Zadržavanja oznake** pod **Usklađenost upravljanja**, stvaranje **zadržavanja oznaka** s **Premještanje arhiva** akciju koja sadrži željenu **Zadržavanja dob**.</span><span class="sxs-lookup"><span data-stu-id="64aa5-106">In the Exchange Admin Center, select **Retention Tags** under **Compliance Management**, create a **Retention tag** with the **Move to Archive** action containing the desired **Retention Age**.</span></span>
    
3. <span data-ttu-id="64aa5-107">U centru za administraciju sustava Exchange odaberite **Pravila zadržavanja**, stvaranje **Pravila zadržavanja** i dodati to pravilo zadržavanja oznaka **Premjesti u arhivu** .</span><span class="sxs-lookup"><span data-stu-id="64aa5-107">In the Exchange Admin Center, select **Retention Policies**, create a **Retention Policy** and add your **Move to Archive** retention tag to that policy.</span></span> 
    
4. <span data-ttu-id="64aa5-p103">[Dodjeljivanje pravila zadržavanja](https://docs.microsoft.com/en-us/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) poštanski sandučić određenog korisnika. Ista pravila primijenit će se na **primarni** i poštanski sandučić **arhiva** .</span><span class="sxs-lookup"><span data-stu-id="64aa5-p103">[Assign the Retention Policy](https://docs.microsoft.com/en-us/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox. The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span> 
    
<span data-ttu-id="64aa5-p104">Korisnikov poštanski sandučić trebala bi pravila arhiviranja za premještanje stavki poštanskog sandučića arhiva. Možda će biti potrebno da biste prisilili na upravljana mapa pomoćnika (MFA) za pokretanje i primijeniti nove postavke u korisnički poštanski sandučić. Pokrenite sljedeću naredbu tijekom [povezani EXO PowerShell](https://docs.microsoft.com/en-us/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) za pokretanje upravljanih Pomoćnik za mape za određene poštanski sandučić:</span><span class="sxs-lookup"><span data-stu-id="64aa5-p104">The user's mailbox should now have an Archive policy to move items to the Archive mailbox. It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox. Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/en-us/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span> 
  
```
Start-ManagedFolderAssistant -Identity <name of the mailbox>
```

<span data-ttu-id="64aa5-113">Dodatne informacije o postavljanju pravila arhiviranja potražite u odjeljku [Postavljanje arhiva i brisanje pravila za poštanske sandučiće](https://docs.microsoft.com/en-us/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span><span class="sxs-lookup"><span data-stu-id="64aa5-113">Want more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/en-us/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  

