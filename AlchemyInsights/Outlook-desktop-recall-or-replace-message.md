---
title: Outlook radne površine opoziv ili zamjena poruke e-pošte
ms.author: daeite
author: daeite
manager: joallard
ms.date: 3/13/2019
ms.audience: Admin
ms.topic: article
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: aced684777ef82860b969aea8825699b78b04c5a
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32389664"
---
# <a name="recall-or-replace-an-email-message"></a><span data-ttu-id="d60a9-102">Opozvati ili zamijeniti poruku e-pošte</span><span class="sxs-lookup"><span data-stu-id="d60a9-102">Recall or replace an email message</span></span>

- <span data-ttu-id="d60a9-103">Kao administrator, možete **opoziv poruke u ime korisnika pomoću PowerShell**.</span><span class="sxs-lookup"><span data-stu-id="d60a9-103">As the admin, you can **recall messages on behalf of users using PowerShell**.</span></span> <span data-ttu-id="d60a9-104">Nije moguće opozvati poruke iz centra za administraciju.</span><span class="sxs-lookup"><span data-stu-id="d60a9-104">You can't recall messages from the admin center.</span></span>
- <span data-ttu-id="d60a9-105">Možete **samo opoziv poruke koje se šalju osobe u vašoj organizaciji**.</span><span class="sxs-lookup"><span data-stu-id="d60a9-105">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="d60a9-106">Ako je poruka poslana na adresu Gmail, na primjer, ne možete opozvati ga.</span><span class="sxs-lookup"><span data-stu-id="d60a9-106">If the message was sent to a Gmail address, for example, you can't recall it.</span></span>
- <span data-ttu-id="d60a9-107">Možete **samo opoziv poruke poslane iz Outlook 2016 na Računalu**.</span><span class="sxs-lookup"><span data-stu-id="d60a9-107">You can **only recall messages sent from Outlook 2016 on the PC**.</span></span> <span data-ttu-id="d60a9-108">Ako korisnik pošalje poruku koristeći Outlook za Mac ili Outlook na webu, ne može se opozvati.</span><span class="sxs-lookup"><span data-stu-id="d60a9-108">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>

<span data-ttu-id="d60a9-109">Kako opozvati ili zamijeniti poruku e-pošte:</span><span class="sxs-lookup"><span data-stu-id="d60a9-109">To recall or replace an email message:</span></span>

1. <span data-ttu-id="d60a9-110">U oknu mape na lijevoj strani prozora programa Outlook, odaberite mapu poslane stavke.</span><span class="sxs-lookup"><span data-stu-id="d60a9-110">In the folder pane on the left of the Outlook window, select the Sent Items folder.</span></span>
1. <span data-ttu-id="d60a9-111">Dvokliknite poruku koju želite opozvati da biste ga otvorili.</span><span class="sxs-lookup"><span data-stu-id="d60a9-111">Double-click the message you want to recall to open it.</span></span>
1. <span data-ttu-id="d60a9-112">Odaberite karticu **poruku** , a zatim odaberite **Akcije** > **Opoziv ove poruke**.</span><span class="sxs-lookup"><span data-stu-id="d60a9-112">Select the **Message** tab, and then select **Actions** > **Recall This Message**.</span></span>
1. <span data-ttu-id="d60a9-113">Odaberite **izbrisati nepročitane kopije ove poruke** ili **izbrisati nepročitane kopije i zamijeniti novu poruku**, a zatim odaberite **u redu**.</span><span class="sxs-lookup"><span data-stu-id="d60a9-113">Select **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, and then select **OK**.</span></span>
1. <span data-ttu-id="d60a9-114">Ako šaljete poruku zamjenski sastavite poruku, a zatim odaberite **Pošalji**.</span><span class="sxs-lookup"><span data-stu-id="d60a9-114">If you're sending a replacement message, compose the message, and then select **Send**.</span></span>
1. <span data-ttu-id="d60a9-115">Uspjeh ili Neuspjeh opoziva poruke ovisi o postavkama primatelja u programu Outlook.</span><span class="sxs-lookup"><span data-stu-id="d60a9-115">The success or failure of a message recall depends on the recipient's settings in Outlook.</span></span> <span data-ttu-id="d60a9-116">Korake provjeriti opoziv potražite u [ovom članku](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span><span class="sxs-lookup"><span data-stu-id="d60a9-116">For steps to check on the recall, see [this article](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="d60a9-117">Traženje i brisanje poruka e-pošte u vašoj organizaciji</span><span class="sxs-lookup"><span data-stu-id="d60a9-117">Search for and delete email messages in your organization</span></span>

- <span data-ttu-id="d60a9-118">Ako niste globalni administrator, vaš račun mora dodati predočavanja elektroničkih dokumenata Upravitelj ulogu ili uloge Upravljanje usklađenosti pretraživanja za traženje poruke.</span><span class="sxs-lookup"><span data-stu-id="d60a9-118">If you're not a global admin, your account must be added to the eDiscovery Manager role or Compliance Search management role to search for messages.</span></span> <span data-ttu-id="d60a9-119">Za brisanje poruka, trebat ćete pridružiti grupe uloga upravljanja organizacije ili upravljanje uloga pretraživanja i Pročisti.</span><span class="sxs-lookup"><span data-stu-id="d60a9-119">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="d60a9-120">Dozvole za ove uloge dodjeljuju se u [centru sigurnosti i usklađenosti](https://go.microsoft.com/fwlink/?linkid=2083731).</span><span class="sxs-lookup"><span data-stu-id="d60a9-120">Permissions for these roles are assigned in the [Security and compliance center](https://go.microsoft.com/fwlink/?linkid=2083731).</span></span>
- <span data-ttu-id="d60a9-121">[Stvaranje sadržaja pretraživanja](https://docs.microsoft.com/office365/securitycompliance/content-search) da biste pronašli poruku za brisanje.</span><span class="sxs-lookup"><span data-stu-id="d60a9-121">[Create a content search](https://docs.microsoft.com/office365/securitycompliance/content-search) to find the message to delete.</span></span>
- <span data-ttu-id="d60a9-122">[Povezivanje s sigurnost i usklađenosti centar PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="d60a9-122">[Connect to Security and Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span></span>

<span data-ttu-id="d60a9-123">Ako koristite višestruku provjeru autentičnosti, pogledajte [povezivanje za Office 365 sigurnost i usklađenosti centar PowerShell korištenjem višestruku provjeru autentičnosti](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="d60a9-123">If you're using multi-factor authentication, see [Connect to Office 365 Security and Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span></span>