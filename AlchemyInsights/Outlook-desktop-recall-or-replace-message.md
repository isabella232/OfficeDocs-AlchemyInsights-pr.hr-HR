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
ms.openlocfilehash: 3d3a6c253317137b7069a978b907c97d61bf7313
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36496103"
---
# <a name="recall-or-replace-an-outlook-email-message"></a><span data-ttu-id="31339-102">Opozvati ili zamijeniti poruku e-pošte programa Outlook</span><span class="sxs-lookup"><span data-stu-id="31339-102">Recall or replace an Outlook email message</span></span>

- <span data-ttu-id="31339-103">Kao administrator, možete **opoziv poruke u ime korisnika pomoću PowerShell**.</span><span class="sxs-lookup"><span data-stu-id="31339-103">As the admin, you can **recall messages on behalf of users using PowerShell**.</span></span> <span data-ttu-id="31339-104">Nije moguće opozvati poruke iz centra za administraciju.</span><span class="sxs-lookup"><span data-stu-id="31339-104">You can't recall messages from the admin center.</span></span>
- <span data-ttu-id="31339-105">Možete **samo opoziv poruke koje se šalju osobe u vašoj organizaciji**.</span><span class="sxs-lookup"><span data-stu-id="31339-105">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="31339-106">Ako je poruka poslana na adresu Gmail, na primjer, ne možete opozvati ga.</span><span class="sxs-lookup"><span data-stu-id="31339-106">If the message was sent to a Gmail address, for example, you can't recall it.</span></span>
- <span data-ttu-id="31339-107">Možete **samo opoziv poruke poslane iz Outlook 2016 na Računalu**.</span><span class="sxs-lookup"><span data-stu-id="31339-107">You can **only recall messages sent from Outlook 2016 on the PC**.</span></span> <span data-ttu-id="31339-108">Ako korisnik pošalje poruku koristeći Outlook za Mac ili Outlook na webu, ne može se opozvati.</span><span class="sxs-lookup"><span data-stu-id="31339-108">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>

<span data-ttu-id="31339-109">Kako opozvati ili zamijeniti poruku e-pošte:</span><span class="sxs-lookup"><span data-stu-id="31339-109">To recall or replace an email message:</span></span>

1. <span data-ttu-id="31339-110">U oknu mape na lijevoj strani prozora programa Outlook, odaberite mapu poslane stavke.</span><span class="sxs-lookup"><span data-stu-id="31339-110">In the folder pane on the left of the Outlook window, select the Sent Items folder.</span></span>
1. <span data-ttu-id="31339-111">Dvokliknite poruku koju želite opozvati da biste ga otvorili.</span><span class="sxs-lookup"><span data-stu-id="31339-111">Double-click the message you want to recall to open it.</span></span>
1. <span data-ttu-id="31339-112">Odaberite karticu **poruku** , a zatim odaberite **Akcije** > **Opoziv ove poruke**.</span><span class="sxs-lookup"><span data-stu-id="31339-112">Select the **Message** tab, and then select **Actions** > **Recall This Message**.</span></span>
1. <span data-ttu-id="31339-113">Odaberite **izbrisati nepročitane kopije ove poruke** ili **izbrisati nepročitane kopije i zamijeniti novu poruku**, a zatim odaberite **u redu**.</span><span class="sxs-lookup"><span data-stu-id="31339-113">Select **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, and then select **OK**.</span></span>
1. <span data-ttu-id="31339-114">Ako šaljete poruku zamjenski sastavite poruku, a zatim odaberite **Pošalji**.</span><span class="sxs-lookup"><span data-stu-id="31339-114">If you're sending a replacement message, compose the message, and then select **Send**.</span></span>
1. <span data-ttu-id="31339-115">Uspjeh ili Neuspjeh opoziva poruke ovisi o postavkama primatelja u programu Outlook.</span><span class="sxs-lookup"><span data-stu-id="31339-115">The success or failure of a message recall depends on the recipient's settings in Outlook.</span></span> <span data-ttu-id="31339-116">Korake provjeriti opoziv potražite u [ovom članku](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span><span class="sxs-lookup"><span data-stu-id="31339-116">For steps to check on the recall, see [this article](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="31339-117">Traženje i brisanje poruka e-pošte u vašoj organizaciji</span><span class="sxs-lookup"><span data-stu-id="31339-117">Search for and delete email messages in your organization</span></span>

- <span data-ttu-id="31339-118">Ako niste globalni administrator, vaš račun mora dodati predočavanja elektroničkih dokumenata Upravitelj ulogu ili uloge Upravljanje usklađenosti pretraživanja za traženje poruke.</span><span class="sxs-lookup"><span data-stu-id="31339-118">If you're not a global admin, your account must be added to the eDiscovery Manager role or Compliance Search management role to search for messages.</span></span> <span data-ttu-id="31339-119">Za brisanje poruka, trebat ćete pridružiti grupe uloga upravljanja organizacije ili upravljanje uloga pretraživanja i Pročisti.</span><span class="sxs-lookup"><span data-stu-id="31339-119">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="31339-120">Dozvole za ove uloge dodjeljuju se u [centru sigurnosti i usklađenosti](https://go.microsoft.com/fwlink/?linkid=2083731).</span><span class="sxs-lookup"><span data-stu-id="31339-120">Permissions for these roles are assigned in the [Security and compliance center](https://go.microsoft.com/fwlink/?linkid=2083731).</span></span>
- <span data-ttu-id="31339-121">[Stvaranje sadržaja pretraživanja](https://docs.microsoft.com/office365/securitycompliance/content-search) da biste pronašli poruku za brisanje.</span><span class="sxs-lookup"><span data-stu-id="31339-121">[Create a content search](https://docs.microsoft.com/office365/securitycompliance/content-search) to find the message to delete.</span></span>
- <span data-ttu-id="31339-122">[Povezivanje s sigurnost i usklađenosti centar PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="31339-122">[Connect to Security and Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span></span>

<span data-ttu-id="31339-123">Ako koristite višestruku provjeru autentičnosti, pogledajte [povezivanje za Office 365 sigurnost i usklađenosti centar PowerShell korištenjem višestruku provjeru autentičnosti](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="31339-123">If you're using multi-factor authentication, see [Connect to Office 365 Security and Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span></span>