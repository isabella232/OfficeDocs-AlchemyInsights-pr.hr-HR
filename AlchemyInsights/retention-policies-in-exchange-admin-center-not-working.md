---
title: Pravila zadržavanja u centru za administraciju sustava Exchange ne radi
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 6c69511f6bcdad5793cd2473a20a2d168d2ac260
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 01/30/2019
ms.locfileid: "29660699"
---
 <span data-ttu-id="1dd90-102">**Problem:** Novostvoreni ili pravila zadržavanja ažurirani u centru za administraciju sustava Exchange ne primjenjivanje na poštanske sandučiće ili stavke su premještene u poštanski sandučić arhive ili izbrisane.</span><span class="sxs-lookup"><span data-stu-id="1dd90-102">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="1dd90-103">**Korijenski uzrok:**</span><span class="sxs-lookup"><span data-stu-id="1dd90-103">**Root Causes:**</span></span>
  
- <span data-ttu-id="1dd90-p101">Možda na **Upravljana pomoćnika za mape** nije obrađen korisnikov poštanski sandučić. Upravljani Pomoćnik za mape pokušava obraditi svakih poštanskog sandučića u organizaciji oblak temelji svakih sedam dana. Ako promijenite oznaku zadržavanja ili primijenite neko drugo pravilo zadržavanja poštanski sandučić, možete pričekati dok na upravljana mapa pomoći obrađuje poštanski sandučić ili pokrenite cmdlet Start ManagedFolderAssistant za pokretanje upravljanih Pomoćnik za mape za određenu obradu poštanski sandučić. Ovaj cmdlet pokrenut je korisna za testiranje ili postavke zadržavanja oznaka ili pravila zadržavanja za otklanjanje poteškoća. Za dodatne informacije posjetite [pokrenuti upravljanih Pomoćnik za mape](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span><span class="sxs-lookup"><span data-stu-id="1dd90-p101">This may be because the **Managed Folder Assistant** has not processed the user's mailbox. The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days. If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox. Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings. For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="1dd90-109">**Rješenja:** Pokrenite sljedeću naredbu za pokretanje upravljanih Pomoćnik za mape za određene poštanski sandučić:</span><span class="sxs-lookup"><span data-stu-id="1dd90-109">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span> 
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="1dd90-p102">To može se pojaviti i ako je **omogućeno** u poštanskom sandučiću **RetentionHold** . Ako poštanski sandučić stavljen na RetentionHold, pravila zadržavanja na poštanski sandučić nije obrađena tijekom vremena. Za više informaton na RetentionHold postavku pogledajte: [Poštanski sandučić držite zadržavanja](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span><span class="sxs-lookup"><span data-stu-id="1dd90-p102">This may also be occur if **RetentionHold** has been **enabled** on the mailbox. If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time. For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="1dd90-113">**Rješenje:**</span><span class="sxs-lookup"><span data-stu-id="1dd90-113">**Solution:**</span></span>
    
  - <span data-ttu-id="1dd90-114">Provjera stanja RetentionHold postavku na određenom poštanskom sandučiću u [PowerShellu EXO](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span><span class="sxs-lookup"><span data-stu-id="1dd90-114">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="1dd90-115">Pokrenite sljedeću naredbu da biste **onemogućili** RetentionHold na određene poštanski sandučić:</span><span class="sxs-lookup"><span data-stu-id="1dd90-115">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span> 
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="1dd90-116">Sada, ponovno pokrenite mapi upravljani pomoćnika:</span><span class="sxs-lookup"><span data-stu-id="1dd90-116">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="1dd90-117">**Napomena:** Ako poštanski sandučić je manja od 10 MB, upravljana Pomoćnik za mape neće automatski obraditi poštanski sandučić.</span><span class="sxs-lookup"><span data-stu-id="1dd90-117">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span> 
  

