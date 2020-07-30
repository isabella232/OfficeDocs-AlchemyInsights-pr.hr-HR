---
title: Pravila zadržavanja u sustavu Exchange Admin Center ne funkcioniraju
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 4d3ca121c8d22a0900f136f7f2a754dfb5b435f5
ms.sourcegitcommit: ffbed67c0a16ec423fa1d79b71e48ea4e2d320e1
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 07/29/2020
ms.locfileid: "46522799"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="10f85-102">Pravila zadržavanja u centru za administratore sustava Exchange</span><span class="sxs-lookup"><span data-stu-id="10f85-102">Retention Policies in Exchange Admin Center</span></span>

<span data-ttu-id="10f85-103">Ako želite da pokrenemo automatske provjere za postavke navedene u nastavku, odaberite gumb za povratak <-- pri vrhu ove stranice, a zatim unesite adresu e-pošte korisnika koji ima problema s pravilima zadržavanja.</span><span class="sxs-lookup"><span data-stu-id="10f85-103">If you want us to run automated checks for the settings mentioned below, select the back button <-- at the top of this page, and then enter the email address of the user who has problems with retention policies.</span></span>

 <span data-ttu-id="10f85-104">**Problem:** Novostvorena ili ažurirana pravila zadržavanja u centru za administratore sustava Exchange ne primjenjuju se na poštanske sandučiće ili se stavke ne premještaju u poštanski sandučić arhive ili brišu.</span><span class="sxs-lookup"><span data-stu-id="10f85-104">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="10f85-105">**Uzroci korijena:**</span><span class="sxs-lookup"><span data-stu-id="10f85-105">**Root Causes:**</span></span>
  
- <span data-ttu-id="10f85-106">To je možda zato što pomoćnik za **upravljane mape** nije obradio korisnikov poštanski sandučić.</span><span class="sxs-lookup"><span data-stu-id="10f85-106">This may be because the **Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="10f85-107">Pomoćnik za upravljane mape pokušava obraditi svaki poštanski sandučić u vašoj organizaciji utemeljenoj na oblaku svakih sedam dana.</span><span class="sxs-lookup"><span data-stu-id="10f85-107">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span> <span data-ttu-id="10f85-108">Ako promijenite oznaku zadržavanja ili primijenite drugo pravilo zadržavanja na poštanski sandučić, možete pričekati dok pomoć u upravljanim mapama ne obradi poštanski sandučić ili možete pokrenuti cmdlet Start-ManagedFolderAssistant da biste pokrenuli pomoćnika za upravljane mape za obradu određenog poštanskog sandučića.</span><span class="sxs-lookup"><span data-stu-id="10f85-108">If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox.</span></span> <span data-ttu-id="10f85-109">Pokretanje ovog cmdleta korisno je za testiranje ili otklanjanje poteškoća s pravilima zadržavanja ili postavkama oznake zadržavanja.</span><span class="sxs-lookup"><span data-stu-id="10f85-109">Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings.</span></span> <span data-ttu-id="10f85-110">Dodatne informacije [potražite u odjeljku Pokretanje pomoćnika za upravljane mape](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span><span class="sxs-lookup"><span data-stu-id="10f85-110">For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="10f85-111">**Rješenje:** Pokrenite sljedeću naredbu da biste pokrenuli pomoćnik za upravljane mape za određeni poštanski sandučić:</span><span class="sxs-lookup"><span data-stu-id="10f85-111">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="10f85-112">To se može dogoditi i ako je u poštanskom sandučiću **omogućena** **zadržavanja.**</span><span class="sxs-lookup"><span data-stu-id="10f85-112">This may also be occur if **RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="10f85-113">Ako je poštanski sandučić postavljen na zadržavanje, pravila zadržavanja na poštanskom sandučiću neće se obraditi tijekom tog vremena.</span><span class="sxs-lookup"><span data-stu-id="10f85-113">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span> <span data-ttu-id="10f85-114">Dodatne informacije o postavkama Zadržavanje potražite u odjeljku: [Zadržavanje poštanskog sandučića](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span><span class="sxs-lookup"><span data-stu-id="10f85-114">For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="10f85-115">**Rješenje:**</span><span class="sxs-lookup"><span data-stu-id="10f85-115">**Solution:**</span></span>
    
  - <span data-ttu-id="10f85-116">Provjerite status postavke Zadržavanje na određenom poštanskom sandučiću u [EXO powershellu:](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)</span><span class="sxs-lookup"><span data-stu-id="10f85-116">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="10f85-117">Pokrenite sljedeću naredbu da biste **onemogućili** zadržavanje na određenom poštanskom sandučiću:</span><span class="sxs-lookup"><span data-stu-id="10f85-117">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span>
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="10f85-118">Zatim, re- trčanje Uprava savijač Pomoćnik:</span><span class="sxs-lookup"><span data-stu-id="10f85-118">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="10f85-119">**Napomena:** Ako je poštanski sandučić manji od 10 MB, pomoćnik za upravljane mape neće automatski obraditi poštanski sandučić.</span><span class="sxs-lookup"><span data-stu-id="10f85-119">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span>
 
<span data-ttu-id="10f85-120">Dodatne informacije o pravilima zadržavanja u centru za administratore sustava Exchange potražite u članku:</span><span class="sxs-lookup"><span data-stu-id="10f85-120">For more info on retention policies in the Exchange Admin Center, see:</span></span>
- [<span data-ttu-id="10f85-121">Oznake zadržavanja i pravila zadržavanja</span><span class="sxs-lookup"><span data-stu-id="10f85-121">Retention tags and retention policies</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [<span data-ttu-id="10f85-122">Primjena pravila zadržavanja na poštanske sandučiće</span><span class="sxs-lookup"><span data-stu-id="10f85-122">Apply a retention policy to mailboxes</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [<span data-ttu-id="10f85-123">Dodavanje ili uklanjanje oznaka zadržavanja</span><span class="sxs-lookup"><span data-stu-id="10f85-123">Add or remove retention tags</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [<span data-ttu-id="10f85-124">Kako prepoznati vrstu čekanja postavljenu na poštanski sandučić</span><span class="sxs-lookup"><span data-stu-id="10f85-124">How to identify the type of hold placed on a mailbox</span></span>](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
