---
title: 902 (pogreške pri sinkronizaciji zbog duplikata objekata)
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 5/30/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: f8db233167a5e2b2ef7290438b8e6d92d0dccb1e
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 01/15/2019
ms.locfileid: "28280513"
---
# <a name="sync-errors-due-to-duplicate-objects"></a><span data-ttu-id="74968-102">Pogreške pri sinkronizaciji zbog duplikata objekata</span><span class="sxs-lookup"><span data-stu-id="74968-102">Sync errors due to duplicate objects</span></span>

<span data-ttu-id="74968-103">Možete primiti jednu od sljedećih poruka o pogrešci kada završi sinkronizacije imenika:</span><span class="sxs-lookup"><span data-stu-id="74968-103">You might receive one of the following error messages when directory synchronization finishes:</span></span>
  
- <span data-ttu-id="74968-104">Nije moguće ažurirati objekt u Microsoft Online Services jer vrijednosti koje možda već pridružen drugom objektu u lokalni direktorij imati sljedeće atribute povezane s ovom objektu.</span><span class="sxs-lookup"><span data-stu-id="74968-104">Unable to update this object in Microsoft Online Services because the following attributes associated with this object have values that may already be associated with another object in your local directory.</span></span>
    
- <span data-ttu-id="74968-105">Sinkronizirane objekt s iste adrese proxy već postoji u direktoriju Microsoft Online Services.</span><span class="sxs-lookup"><span data-stu-id="74968-105">A synchronized object with the same proxy address already exists in your Microsoft Online Services directory.</span></span>
    
- <span data-ttu-id="74968-106">Nije moguće ažurirati ovaj objekt jer sljedeće atribute povezane s ovom objektu imati vrijednosti koje možda već povezani s drugim objektom lokalni direktorij services: UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="74968-106">Unable to update this object because the following attributes associated with this object have values that may already be associated with another object in your local directory services: UserPrincipalName.</span></span>
    
<span data-ttu-id="74968-107">Prepoznajte i riješite problem, preuzmite i pokrenite [IdFix DirSync pogreška olakšava alat](https://www.microsoft.com/download/details.aspx?id=36832).</span><span class="sxs-lookup"><span data-stu-id="74968-107">To identify and fix the issue, download and run the [IdFix DirSync Error Remediation Tool](https://www.microsoft.com/download/details.aspx?id=36832).</span></span>
  
<span data-ttu-id="74968-108">Za dodatne informacije pogledajte [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span><span class="sxs-lookup"><span data-stu-id="74968-108">For more information, see [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span></span>
  

