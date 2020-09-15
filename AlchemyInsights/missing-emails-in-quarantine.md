---
title: Propuštate poruke e-pošte u karanteni
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 55ed9a92675939c05477fbf6d12bbedd6eb931d6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47673706"
---
# <a name="missing-emails-in-quarantine"></a><span data-ttu-id="f8339-102">Propuštate poruke e-pošte u karanteni "</span><span class="sxs-lookup"><span data-stu-id="f8339-102">Missing emails in quarantine"</span></span>

<span data-ttu-id="f8339-103">Administratori mogu [pregledavati, objaviti ili brisati te poruke.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="f8339-103">Administrators can [view, release, or delete these messages.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span></span>

<span data-ttu-id="f8339-104">Da biste otvorili centar za sigurnost & usklađenosti, otvorite [https://protection.office.com](https://protection.office.com/) .</span><span class="sxs-lookup"><span data-stu-id="f8339-104">To open the Security & Compliance Center, go to [https://protection.office.com](https://protection.office.com/).</span></span> <span data-ttu-id="f8339-105">Da biste izravno otvorili stranicu karantene, idite na [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .</span><span class="sxs-lookup"><span data-stu-id="f8339-105">To open the Quarantine page directly, go to [https://protection.office.com/quarantine](https://protection.office.com/quarantine).</span></span>  

<span data-ttu-id="f8339-106">Možete pretraživati po sljedećim vrijednostima:</span><span class="sxs-lookup"><span data-stu-id="f8339-106">You can search by the following values:</span></span>  

- <span data-ttu-id="f8339-107">**ID poruke**: globalno jedinstveni identifikator poruke.</span><span class="sxs-lookup"><span data-stu-id="f8339-107">**Message ID**: The globally unique identifier of the message.</span></span> <span data-ttu-id="f8339-108">Ako odaberete poruku na popisu, prikazat će se vrijednost  **ID**  -a poruke u oknu s  **detaljima**  koje će se prikazati.</span><span class="sxs-lookup"><span data-stu-id="f8339-108">If you select a message in the list, the  **Message ID**  value appears in the  **Details**  flyout pane that appears.</span></span> <span data-ttu-id="f8339-109">Administratori mogu koristiti [Praćenje poruka](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) da bi pronašli poruke i odgovarajuće ID-ove poruka.</span><span class="sxs-lookup"><span data-stu-id="f8339-109">Admins can use [message trace](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) to find messages and their corresponding Message ID values.</span></span>
- <span data-ttu-id="f8339-110">**Adresa e-pošte pošiljatelja**: adresa e-pošte jednog pošiljatelja.</span><span class="sxs-lookup"><span data-stu-id="f8339-110">**Sender email address**: A single sender's email address.</span></span>
- <span data-ttu-id="f8339-111">**Adresa e-pošte primatelja**: adresa e-pošte jednog primatelja.</span><span class="sxs-lookup"><span data-stu-id="f8339-111">**Recipient email address**: A single recipient's email address.</span></span>
- <span data-ttu-id="f8339-112">**Predmet**: koristite cijeli predmet poruke.</span><span class="sxs-lookup"><span data-stu-id="f8339-112">**Subject**: Use the entire subject of the message.</span></span> <span data-ttu-id="f8339-113">Pretraživanje ne razlikuje velika i mala slova.</span><span class="sxs-lookup"><span data-stu-id="f8339-113">The search is not case-sensitive.</span></span>

<span data-ttu-id="f8339-114">Nakon što unesete kriterij pretraživanja, kliknite Osvježi ![ gumb Osvježi ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Refresh** da biste filtrirali rezultate.  </span><span class="sxs-lookup"><span data-stu-id="f8339-114">After you've entered the search criteria, click  ![Refresh button](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide)  **Refresh**  to filter the results.</span></span>

<span data-ttu-id="f8339-115">Cmdleti koje koristite za prikaz i upravljanje porukama i datotekama u karanteni su:</span><span class="sxs-lookup"><span data-stu-id="f8339-115">The cmdlets you use to view and manages messages and files in quarantine are:</span></span>
- [<span data-ttu-id="f8339-116">Brisanje-poruka u karanteni</span><span class="sxs-lookup"><span data-stu-id="f8339-116">Delete-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [<span data-ttu-id="f8339-117">Izvoz-poruka u karanteni</span><span class="sxs-lookup"><span data-stu-id="f8339-117">Export-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [<span data-ttu-id="f8339-118">Poruka o karanteni</span><span class="sxs-lookup"><span data-stu-id="f8339-118">Get-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- <span data-ttu-id="f8339-119">[Pretpregled – poruka karantene](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Imajte na čemu da je ovaj cmdlet namijenjen samo porukama, a ne i zlonamjernim datotekama sa servisa ATP za SharePoint Online, OneDrive za tvrtke ili timove.</span><span class="sxs-lookup"><span data-stu-id="f8339-119">[Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Note that this cmdlet is only for messages, not malware files from ATP for SharePoint Online, OneDrive for Business, or Teams.</span></span>
- [<span data-ttu-id="f8339-120">Release-poruka u karanteni</span><span class="sxs-lookup"><span data-stu-id="f8339-120">Release-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)