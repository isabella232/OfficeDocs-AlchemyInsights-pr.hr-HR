---
title: Pravila zadržavanja u centru za administratore sustava Exchange ne funkcioniraju
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 1fee2361b2dd6e0989d430a17aebb13bd5948578
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47740502"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="8426c-102">Pravila zadržavanja u centru za administratore sustava Exchange</span><span class="sxs-lookup"><span data-stu-id="8426c-102">Retention Policies in Exchange Admin Center</span></span>

<span data-ttu-id="8426c-103">Ako želite da pokrenete automatske provjere za navedene postavke, odaberite gumb natrag < – pri vrhu ove stranice, a zatim unesite adresu e-pošte korisnika koji ima problema s pravilima zadržavanja.</span><span class="sxs-lookup"><span data-stu-id="8426c-103">If you want us to run automated checks for the settings mentioned below, select the back button <-- at the top of this page, and then enter the email address of the user who has problems with retention policies.</span></span>

 <span data-ttu-id="8426c-104">**Problem:** Novo stvorene ili ažurirane pravilnika o zadržavanju u centru za administratore sustava Exchange ne primjenjuju se na poštanske sandučiće ili se stavke ne premještaju u arhivski poštanski sandučić ili izbrisane.</span><span class="sxs-lookup"><span data-stu-id="8426c-104">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="8426c-105">**Korijenski uzroci:**</span><span class="sxs-lookup"><span data-stu-id="8426c-105">**Root Causes:**</span></span>
  
- <span data-ttu-id="8426c-106">To je možda zato što **Pomoćnik za upravljane mape** nije procesira korisnikov poštanski sandučić.</span><span class="sxs-lookup"><span data-stu-id="8426c-106">This may be because the **Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="8426c-107">Pomoćnik za upravljane mape pokušava obraditi svaki poštanski sandučić u tvrtki ili ustanovi utemeljenoj na oblaku jednom svakih sedam dana.</span><span class="sxs-lookup"><span data-stu-id="8426c-107">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span> <span data-ttu-id="8426c-108">Ako promijenite oznaku zadržavanja ili primijenite drugo pravilo zadržavanja na poštanski sandučić, možete pričekati dok upravna mapa ne obradi poštanski sandučić, a možete i pokrenuti cmdlet Start-ManagedFolderAssistant da biste pokrenuli pomoćnik za upravljane mape da bi obradio određeni poštanski sandučić.</span><span class="sxs-lookup"><span data-stu-id="8426c-108">If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox.</span></span> <span data-ttu-id="8426c-109">Pokretanjem tog cmdleta korisna je provjera i otklanjanje poteškoća s pravilima zadržavanja ili oznakama zadržavanja.</span><span class="sxs-lookup"><span data-stu-id="8426c-109">Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings.</span></span> <span data-ttu-id="8426c-110">Dodatne informacije potražite u odjeljku [pokretanje pomoćnika za upravljanu mapu](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span><span class="sxs-lookup"><span data-stu-id="8426c-110">For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="8426c-111">**Rješenje:** Pokrenite sljedeću naredbu da biste pokrenuli pomoćnik za upravljane mape za određeni poštanski sandučić:</span><span class="sxs-lookup"><span data-stu-id="8426c-111">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="8426c-112">To se može dogoditi i ako je na poštanskom sandučiću **omogućena** mogućnost **Retentionhold** .</span><span class="sxs-lookup"><span data-stu-id="8426c-112">This may also be occur if **RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="8426c-113">Ako je poštanski sandučić stavljen na nastavak, pravilnik o zadržavanju na poštanskom sandučiću neće biti obrađen tijekom tog vremena.</span><span class="sxs-lookup"><span data-stu-id="8426c-113">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span> <span data-ttu-id="8426c-114">Dodatne informacije o postavljanju programa RetentionHold potražite u članku [zadržavanje poštanskog sandučića na čekanju](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span><span class="sxs-lookup"><span data-stu-id="8426c-114">For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="8426c-115">**Rješenje**</span><span class="sxs-lookup"><span data-stu-id="8426c-115">**Solution:**</span></span>
    
  - <span data-ttu-id="8426c-116">Provjerite status postavke RetentionHold na određenom poštanskom sandučiću u programu [Exo PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span><span class="sxs-lookup"><span data-stu-id="8426c-116">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="8426c-117">Pokrenite sljedeću naredbu da biste **onemogućili** retentionhold na određenom poštanskom sandučiću:</span><span class="sxs-lookup"><span data-stu-id="8426c-117">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span>
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="8426c-118">Zatim ponovno pokrenite pomoćnik za upravljane mape:</span><span class="sxs-lookup"><span data-stu-id="8426c-118">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="8426c-119">**Upozorenje:** Ako je poštanski sandučić manji od 10 MB, pomoćnik za upravljanu mapu neće automatski obraditi poštanski sandučić.</span><span class="sxs-lookup"><span data-stu-id="8426c-119">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span>
 
<span data-ttu-id="8426c-120">Dodatne informacije o pravilima zadržavanja u centru za administratore sustava Exchange potražite u članku:</span><span class="sxs-lookup"><span data-stu-id="8426c-120">For more info on retention policies in the Exchange Admin Center, see:</span></span>
- [<span data-ttu-id="8426c-121">Oznake zadržavanja i pravila zadržavanja</span><span class="sxs-lookup"><span data-stu-id="8426c-121">Retention tags and retention policies</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [<span data-ttu-id="8426c-122">Primjena pravilnika o zadržavanju na poštanske sandučiće</span><span class="sxs-lookup"><span data-stu-id="8426c-122">Apply a retention policy to mailboxes</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [<span data-ttu-id="8426c-123">Dodavanje i uklanjanje oznaka zadržavanja</span><span class="sxs-lookup"><span data-stu-id="8426c-123">Add or remove retention tags</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [<span data-ttu-id="8426c-124">Prepoznavanje vrste držite smještenih na poštanskom sandučiću</span><span class="sxs-lookup"><span data-stu-id="8426c-124">How to identify the type of hold placed on a mailbox</span></span>](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
