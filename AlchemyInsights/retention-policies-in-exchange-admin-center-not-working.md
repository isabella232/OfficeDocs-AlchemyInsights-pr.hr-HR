---
title: Pravila zadržavanja u centru za administratore sustava Exchange ne funkcioniraju
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
ms.openlocfilehash: e2fb22f872be0eefc3b4b78b18cd09baffa66cda
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43742425"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="0c9d7-102">Pravila zadržavanja u centru za administratore sustava Exchange</span><span class="sxs-lookup"><span data-stu-id="0c9d7-102">Retention Policies in Exchange Admin Center</span></span>

 <span data-ttu-id="0c9d7-103">**Broj izdanja:** Novostvorena ili ažurirana pravila zadržavanja u centru za administratore sustava Exchange ne primjenjuju se na poštanske sandučiće ili stavke ne premještaju se u poštanski sandučić arhive ili se ne brišu.</span><span class="sxs-lookup"><span data-stu-id="0c9d7-103">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="0c9d7-104">**Glavni uzroci:**</span><span class="sxs-lookup"><span data-stu-id="0c9d7-104">**Root Causes:**</span></span>
  
- <span data-ttu-id="0c9d7-105">To je možda zato što **pomoćnik za upravljane mape** nije obradio korisnički poštanski sandučić.</span><span class="sxs-lookup"><span data-stu-id="0c9d7-105">This may be because the **Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="0c9d7-106">Pomoćnik za upravljane mape pokušava obraditi svaki poštanski sandučić u vašoj organizaciji utemeljenoj na oblaku svakih sedam dana.</span><span class="sxs-lookup"><span data-stu-id="0c9d7-106">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span> <span data-ttu-id="0c9d7-107">Ako promijenite oznaku zadržavanja ili primijenite drugo pravilo zadržavanja na poštanski sandučić, možete pričekati dok pomoć upravljane mape ne obradi poštanski sandučić ili možete pokrenuti cmdlet Start-ManagedFolderAssistant da biste pokrenuli pomoćnika za upravljane mape da biste obradili određeni poštanski sandučić.</span><span class="sxs-lookup"><span data-stu-id="0c9d7-107">If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox.</span></span> <span data-ttu-id="0c9d7-108">Pokretanje ovog cmdleta korisno je za testiranje ili otklanjanje poteškoća s pravilima zadržavanja ili postavkama oznake zadržavanja.</span><span class="sxs-lookup"><span data-stu-id="0c9d7-108">Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings.</span></span> <span data-ttu-id="0c9d7-109">Dodatne informacije [potražite u odjeljku Pokrenite pomoćnika za upravljane mape](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span><span class="sxs-lookup"><span data-stu-id="0c9d7-109">For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="0c9d7-110">**Rješenje:** Pokrenite sljedeću naredbu da biste pokrenuli pomoćnika za upravljane mape za određeni poštanski sandučić:</span><span class="sxs-lookup"><span data-stu-id="0c9d7-110">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="0c9d7-111">To se može dogoditi i ako je na poštanskom sandučiću **omogućena** **čuvanje vremena zadržavanja.**</span><span class="sxs-lookup"><span data-stu-id="0c9d7-111">This may also be occur if **RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="0c9d7-112">Ako je poštanski sandučić smješten na čuvanje zadržavanja, pravila zadržavanja poštanskog sandučića neće se obraditi tijekom tog vremena.</span><span class="sxs-lookup"><span data-stu-id="0c9d7-112">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span> <span data-ttu-id="0c9d7-113">Za više informaton na postavku ZadržavanjeHold pogledajte: [Zadržavanje poštanskog sandučića Čekanje](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span><span class="sxs-lookup"><span data-stu-id="0c9d7-113">For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="0c9d7-114">**Rješenje:**</span><span class="sxs-lookup"><span data-stu-id="0c9d7-114">**Solution:**</span></span>
    
  - <span data-ttu-id="0c9d7-115">Provjerite status postavke ZadržavanjaDržite na određenom poštanskom sandučiću u [EXO powershell:](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)</span><span class="sxs-lookup"><span data-stu-id="0c9d7-115">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="0c9d7-116">Pokrenite sljedeću naredbu da biste **onemogućili** zadržavanjeDržite na određenom poštanskom sandučiću:</span><span class="sxs-lookup"><span data-stu-id="0c9d7-116">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span>
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="0c9d7-117">Sada ponovno pokrenite Pomoćnik za upravljane mape:</span><span class="sxs-lookup"><span data-stu-id="0c9d7-117">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="0c9d7-118">**Napomena:** Ako je poštanski sandučić manji od 10 MB, pomoćnik za upravljane mape neće automatski obraditi poštanski sandučić.</span><span class="sxs-lookup"><span data-stu-id="0c9d7-118">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span>
 
<span data-ttu-id="0c9d7-119">Dodatne informacije o pravilima zadržavanja u centru za administratore sustava Exchange potražite u članku Sljedeće:</span><span class="sxs-lookup"><span data-stu-id="0c9d7-119">For more info on retention policies in the Exchange Admin Center, see:</span></span>
- [<span data-ttu-id="0c9d7-120">Oznake zadržavanja i pravila zadržavanja</span><span class="sxs-lookup"><span data-stu-id="0c9d7-120">Retention tags and retention policies</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [<span data-ttu-id="0c9d7-121">Primjena pravila zadržavanja na poštanske sandučiće</span><span class="sxs-lookup"><span data-stu-id="0c9d7-121">Apply a retention policy to mailboxes</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [<span data-ttu-id="0c9d7-122">Dodavanje ili uklanjanje oznaka zadržavanja</span><span class="sxs-lookup"><span data-stu-id="0c9d7-122">Add or remove retention tags</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [<span data-ttu-id="0c9d7-123">Kako prepoznati vrstu čekanja postavljenog na poštanski sandučić</span><span class="sxs-lookup"><span data-stu-id="0c9d7-123">How to identify the type of hold placed on a mailbox</span></span>](https://docs.microsoft.com/office365/securitycompliance/identify-a-hold-on-an-exchange-online-mailbox)
