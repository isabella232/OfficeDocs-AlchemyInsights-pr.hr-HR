---
title: Nedostaju poruke e-pošte u karanteni
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 61a926c363c62bc7acb5efefe42b834f33c78eb6
ms.sourcegitcommit: 8fdcd2acd31e8a4b9a8a0b91674f397d2f7889c1
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44568964"
---
# <a name="missing-emails-in-quarantine"></a><span data-ttu-id="738b4-102">Nedostaju poruke e-pošte u karanteni"</span><span class="sxs-lookup"><span data-stu-id="738b4-102">Missing emails in quarantine"</span></span>

<span data-ttu-id="738b4-103">Administratori mogu [pregledavati, objavljivati ili brisati te poruke.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="738b4-103">Administrators can [view, release, or delete these messages.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span></span>

<span data-ttu-id="738b4-104">Da biste otvorili Centar za usklađenost sa sigurnosnim &, idite na [https://protection.office.com](https://protection.office.com/) .</span><span class="sxs-lookup"><span data-stu-id="738b4-104">To open the Security & Compliance Center, go to [https://protection.office.com](https://protection.office.com/).</span></span> <span data-ttu-id="738b4-105">Da biste izravno otvorili stranicu Karantena, idite na [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .</span><span class="sxs-lookup"><span data-stu-id="738b4-105">To open the Quarantine page directly, go to [https://protection.office.com/quarantine](https://protection.office.com/quarantine).</span></span>  

<span data-ttu-id="738b4-106">Možete pretraživati prema sljedećim vrijednostima:</span><span class="sxs-lookup"><span data-stu-id="738b4-106">You can search by the following values:</span></span>  

- <span data-ttu-id="738b4-107">**ID poruke**: globalno jedinstveni identifikator poruke.</span><span class="sxs-lookup"><span data-stu-id="738b4-107">**Message ID**: The globally unique identifier of the message.</span></span> <span data-ttu-id="738b4-108">Ako odaberete poruku na popisu, vrijednost **ID poruke** pojavljuje se u oknu potpalete **detalji** koje će se pojaviti.</span><span class="sxs-lookup"><span data-stu-id="738b4-108">If you select a message in the list, the  **Message ID**  value appears in the  **Details**  flyout pane that appears.</span></span> <span data-ttu-id="738b4-109">Administratori mogu koristiti [praćenje poruka](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) da bi pronašli poruke i njihove odgovarajuće vrijednosti ID-a poruka.</span><span class="sxs-lookup"><span data-stu-id="738b4-109">Admins can use [message trace](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) to find messages and their corresponding Message ID values.</span></span>
- <span data-ttu-id="738b4-110">**Adresa e-pošte pošiljatelja**: adresa e-pošte jednog pošiljatelja.</span><span class="sxs-lookup"><span data-stu-id="738b4-110">**Sender email address**: A single sender's email address.</span></span>
- <span data-ttu-id="738b4-111">**Adresa e-pošte primatelja**: E-adresa jednog primatelja.</span><span class="sxs-lookup"><span data-stu-id="738b4-111">**Recipient email address**: A single recipient's email address.</span></span>
- <span data-ttu-id="738b4-112">**Predmet**: Koristite cijeli predmet poruke.</span><span class="sxs-lookup"><span data-stu-id="738b4-112">**Subject**: Use the entire subject of the message.</span></span> <span data-ttu-id="738b4-113">Pretraživanje ne razlikuje velika i mala slova.</span><span class="sxs-lookup"><span data-stu-id="738b4-113">The search is not case-sensitive.</span></span>

<span data-ttu-id="738b4-114">Kada unesete kriterije pretraživanja, kliknite ![ Osvježi gumb ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Osvježi** da biste filtrirali rezultate.  </span><span class="sxs-lookup"><span data-stu-id="738b4-114">After you've entered the search criteria, click  ![Refresh button](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide)  **Refresh**  to filter the results.</span></span>

<span data-ttu-id="738b4-115">Cmdleti koje koristite za prikaz i upravljanje porukama i datotekama u karanteni su:</span><span class="sxs-lookup"><span data-stu-id="738b4-115">The cmdlets you use to view and manages messages and files in quarantine are:</span></span>
- [<span data-ttu-id="738b4-116">Brisanje karanteneMessage</span><span class="sxs-lookup"><span data-stu-id="738b4-116">Delete-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [<span data-ttu-id="738b4-117">Izvoz-KarantenaMessage</span><span class="sxs-lookup"><span data-stu-id="738b4-117">Export-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [<span data-ttu-id="738b4-118">Get-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="738b4-118">Get-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- <span data-ttu-id="738b4-119">[Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Imajte na umu da je ovaj cmdlet namijenjen samo porukama, a ne za datoteke zlonamjernog softvera iz ATP-a za SharePoint Online, OneDrive za tvrtke ili timove.</span><span class="sxs-lookup"><span data-stu-id="738b4-119">[Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Note that this cmdlet is only for messages, not malware files from ATP for SharePoint Online, OneDrive for Business, or Teams.</span></span>
- [<span data-ttu-id="738b4-120">Izdanje-KarantenaMessage</span><span class="sxs-lookup"><span data-stu-id="738b4-120">Release-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)