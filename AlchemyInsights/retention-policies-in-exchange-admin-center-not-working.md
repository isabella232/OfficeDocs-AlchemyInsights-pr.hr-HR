---
title: Pravila zadržavanja u centru za administraciju sustava Exchange ne radi
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 5d7b62546397c13b37540e8797b31123b2880280
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36551335"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="a92f2-102">Pravila zadržavanja u centru za administraciju sustava Exchange</span><span class="sxs-lookup"><span data-stu-id="a92f2-102">Retention Policies in Exchange Admin Center</span></span>

 <span data-ttu-id="a92f2-103">**Problem:** Novostvoreni ili pravila zadržavanja ažurirani u centru za administraciju sustava Exchange ne primjenjivanje na poštanske sandučiće ili stavke su premještene u poštanski sandučić arhive ili izbrisane.</span><span class="sxs-lookup"><span data-stu-id="a92f2-103">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="a92f2-104">**Korijenski uzrok:**</span><span class="sxs-lookup"><span data-stu-id="a92f2-104">**Root Causes:**</span></span>
  
- <span data-ttu-id="a92f2-105">Možda na **Upravljana pomoćnika za mape** nije obrađen korisnikov poštanski sandučić.</span><span class="sxs-lookup"><span data-stu-id="a92f2-105">This may be because the **Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="a92f2-106">Upravljani Pomoćnik za mape pokušava obraditi svakih poštanskog sandučića u organizaciji oblak temelji svakih sedam dana.</span><span class="sxs-lookup"><span data-stu-id="a92f2-106">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span> <span data-ttu-id="a92f2-107">Ako promijenite oznaku zadržavanja ili primijenite neko drugo pravilo zadržavanja poštanski sandučić, možete pričekati dok na upravljana mapa pomoći obrađuje poštanski sandučić ili pokrenite cmdlet Start ManagedFolderAssistant za pokretanje upravljanih Pomoćnik za mape za određenu obradu poštanski sandučić.</span><span class="sxs-lookup"><span data-stu-id="a92f2-107">If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox.</span></span> <span data-ttu-id="a92f2-108">Ovaj cmdlet pokrenut je korisna za testiranje ili postavke zadržavanja oznaka ili pravila zadržavanja za otklanjanje poteškoća.</span><span class="sxs-lookup"><span data-stu-id="a92f2-108">Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings.</span></span> <span data-ttu-id="a92f2-109">Za dodatne informacije posjetite [pokrenuti upravljanih Pomoćnik za mape](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span><span class="sxs-lookup"><span data-stu-id="a92f2-109">For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="a92f2-110">**Rješenja:** Pokrenite sljedeću naredbu za pokretanje upravljanih Pomoćnik za mape za određene poštanski sandučić:</span><span class="sxs-lookup"><span data-stu-id="a92f2-110">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="a92f2-111">To može se pojaviti i ako je **omogućeno** u poštanskom sandučiću **RetentionHold** .</span><span class="sxs-lookup"><span data-stu-id="a92f2-111">This may also be occur if **RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="a92f2-112">Ako poštanski sandučić stavljen na RetentionHold, pravila zadržavanja na poštanski sandučić nije obrađena tijekom vremena.</span><span class="sxs-lookup"><span data-stu-id="a92f2-112">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span> <span data-ttu-id="a92f2-113">Za više informaton na RetentionHold postavku pogledajte: [Poštanski sandučić držite zadržavanja](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span><span class="sxs-lookup"><span data-stu-id="a92f2-113">For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="a92f2-114">**Rješenje:**</span><span class="sxs-lookup"><span data-stu-id="a92f2-114">**Solution:**</span></span>
    
  - <span data-ttu-id="a92f2-115">Provjera stanja RetentionHold postavku na određenom poštanskom sandučiću u [PowerShellu EXO](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span><span class="sxs-lookup"><span data-stu-id="a92f2-115">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="a92f2-116">Pokrenite sljedeću naredbu da biste **onemogućili** RetentionHold na određene poštanski sandučić:</span><span class="sxs-lookup"><span data-stu-id="a92f2-116">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span>
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="a92f2-117">Sada, ponovno pokrenite mapi upravljani pomoćnika:</span><span class="sxs-lookup"><span data-stu-id="a92f2-117">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="a92f2-118">**Napomena:** Ako poštanski sandučić je manja od 10 MB, upravljana Pomoćnik za mape neće automatski obraditi poštanski sandučić.</span><span class="sxs-lookup"><span data-stu-id="a92f2-118">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span>
 
<span data-ttu-id="a92f2-119">Dodatne informacije o pravilima zadržavanja u centru za administraciju Exchange potražite:</span><span class="sxs-lookup"><span data-stu-id="a92f2-119">For more info on retention policies in the Exchange Admin Center, see:</span></span>
- [<span data-ttu-id="a92f2-120">Oznake zadržavanja i pravila zadržavanja</span><span class="sxs-lookup"><span data-stu-id="a92f2-120">Retention tags and retention policies</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [<span data-ttu-id="a92f2-121">Primijeni pravila zadržavanja poštanski sandučići</span><span class="sxs-lookup"><span data-stu-id="a92f2-121">Apply a retention policy to mailboxes</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [<span data-ttu-id="a92f2-122">Dodavanje ili uklanjanje oznake zadržavanja</span><span class="sxs-lookup"><span data-stu-id="a92f2-122">Add or remove retention tags</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [<span data-ttu-id="a92f2-123">Kako prepoznati vrstu čekanje smjestiti na poštanski sandučić</span><span class="sxs-lookup"><span data-stu-id="a92f2-123">How to identify the type of hold placed on a mailbox</span></span>](https://docs.microsoft.com/office365/securitycompliance/identify-a-hold-on-an-exchange-online-mailbox)
