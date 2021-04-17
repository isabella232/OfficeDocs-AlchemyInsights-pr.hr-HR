---
title: Nedostaje poruka e-pošte u karanteni
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 43f9a1f03084bf9adab706b3f77eff1d1db888ca
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51831726"
---
# <a name="missing-emails-in-quarantine"></a><span data-ttu-id="0f9d2-102">Nedostaje poruka e-pošte u karanteni"</span><span class="sxs-lookup"><span data-stu-id="0f9d2-102">Missing emails in quarantine"</span></span>

<span data-ttu-id="0f9d2-103">Administratori mogu [pregledavati, objavu i brisati te poruke.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="0f9d2-103">Administrators can [view, release, or delete these messages.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span></span>

<span data-ttu-id="0f9d2-104">Da biste otvorili centar za & usklađenosti, idite na [https://protection.office.com](https://protection.office.com/) .</span><span class="sxs-lookup"><span data-stu-id="0f9d2-104">To open the Security & Compliance Center, go to [https://protection.office.com](https://protection.office.com/).</span></span> <span data-ttu-id="0f9d2-105">Da biste izravno otvorili stranicu Karantena, idite na [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .</span><span class="sxs-lookup"><span data-stu-id="0f9d2-105">To open the Quarantine page directly, go to [https://protection.office.com/quarantine](https://protection.office.com/quarantine).</span></span>  

<span data-ttu-id="0f9d2-106">Možete pretraživati prema sljedećim vrijednostima:</span><span class="sxs-lookup"><span data-stu-id="0f9d2-106">You can search by the following values:</span></span>  

- <span data-ttu-id="0f9d2-107">**ID poruke:** globalno jedinstveni identifikator poruke.</span><span class="sxs-lookup"><span data-stu-id="0f9d2-107">**Message ID**: The globally unique identifier of the message.</span></span> <span data-ttu-id="0f9d2-108">Ako na popisu odaberete poruku, u oknu  s detaljima koja će se prikazati prikazat će se vrijednost **ID** poruke.</span><span class="sxs-lookup"><span data-stu-id="0f9d2-108">If you select a message in the list, the  **Message ID**  value appears in the  **Details**  flyout pane that appears.</span></span> <span data-ttu-id="0f9d2-109">Administratori mogu koristiti [praćenje poruka da bi](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) pronašli poruke i njihove odgovarajuće vrijednosti ID-a poruke.</span><span class="sxs-lookup"><span data-stu-id="0f9d2-109">Admins can use [message trace](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) to find messages and their corresponding Message ID values.</span></span>
- <span data-ttu-id="0f9d2-110">**Adresa e-pošte** pošiljatelja: adresa e-pošte jednog pošiljatelja.</span><span class="sxs-lookup"><span data-stu-id="0f9d2-110">**Sender email address**: A single sender's email address.</span></span>
- <span data-ttu-id="0f9d2-111">**Adresa e-pošte** primatelja: adresa e-pošte jednog primatelja.</span><span class="sxs-lookup"><span data-stu-id="0f9d2-111">**Recipient email address**: A single recipient's email address.</span></span>
- <span data-ttu-id="0f9d2-112">**Predmet:** koristite cijeli predmet poruke.</span><span class="sxs-lookup"><span data-stu-id="0f9d2-112">**Subject**: Use the entire subject of the message.</span></span> <span data-ttu-id="0f9d2-113">Pretraživanje ne može umašati velika i mala slova.</span><span class="sxs-lookup"><span data-stu-id="0f9d2-113">The search is not case-sensitive.</span></span>

<span data-ttu-id="0f9d2-114">Kada unesete kriterije pretraživanja, kliknite Osvježi gumb ![ ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Osvježi da** biste filtrirali rezultate.  </span><span class="sxs-lookup"><span data-stu-id="0f9d2-114">After you've entered the search criteria, click  ![Refresh button](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide)  **Refresh**  to filter the results.</span></span>

<span data-ttu-id="0f9d2-115">Cmdleti koje koristite za prikaz poruka i datoteka u karanteni i upravljanje njima:</span><span class="sxs-lookup"><span data-stu-id="0f9d2-115">The cmdlets you use to view and manages messages and files in quarantine are:</span></span>
- [<span data-ttu-id="0f9d2-116">Delete-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="0f9d2-116">Delete-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [<span data-ttu-id="0f9d2-117">Export-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="0f9d2-117">Export-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [<span data-ttu-id="0f9d2-118">Get-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="0f9d2-118">Get-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- <span data-ttu-id="0f9d2-119">[Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Imajte na umu da je ovaj cmdlet samo za poruke, a ne i za datoteke zlonamjernog softvera iz sustava ATP za SharePoint Online, OneDrive za tvrtke ili Teams.</span><span class="sxs-lookup"><span data-stu-id="0f9d2-119">[Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Note that this cmdlet is only for messages, not malware files from ATP for SharePoint Online, OneDrive for Business, or Teams.</span></span>
- [<span data-ttu-id="0f9d2-120">Release-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="0f9d2-120">Release-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)