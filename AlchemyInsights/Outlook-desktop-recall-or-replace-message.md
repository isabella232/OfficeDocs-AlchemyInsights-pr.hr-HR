---
title: Opoziv ili zamjena poruke e-pošte za Outlook za stolna računala
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: bb84363ae7d3c91750d5de789c091c7cebbbedc2
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44502311"
---
# <a name="recall-or-replace-an-outlook-email-message"></a><span data-ttu-id="7766a-102">Opoziv ili zamjena poruke e-pošte programa Outlook</span><span class="sxs-lookup"><span data-stu-id="7766a-102">Recall or replace an Outlook email message</span></span>

- <span data-ttu-id="7766a-103">Kao administrator možete **opozvati poruke u ime korisnika pomoću powershell**.</span><span class="sxs-lookup"><span data-stu-id="7766a-103">As the admin, you can **recall messages on behalf of users using PowerShell**.</span></span> <span data-ttu-id="7766a-104">Ne možete se sjetiti poruka iz centra za administratore.</span><span class="sxs-lookup"><span data-stu-id="7766a-104">You can't recall messages from the admin center.</span></span>
- <span data-ttu-id="7766a-105">Možete **se sjetiti samo poruka koje se šalju osobama u vašoj organizaciji**.</span><span class="sxs-lookup"><span data-stu-id="7766a-105">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="7766a-106">Ako je poruka poslana na Gmail adresu, na primjer, ne možete je se sjetiti.</span><span class="sxs-lookup"><span data-stu-id="7766a-106">If the message was sent to a Gmail address, for example, you can't recall it.</span></span>
- <span data-ttu-id="7766a-107">Možete **se sjetiti samo poruka poslanih iz programa Outlook 2016 na PC- u**.</span><span class="sxs-lookup"><span data-stu-id="7766a-107">You can **only recall messages sent from Outlook 2016 on the PC**.</span></span> <span data-ttu-id="7766a-108">Ako korisnik pošalje poruku pomoću programa Outlook za Mac ili Outlook na webu, ne možete je se sjetiti.</span><span class="sxs-lookup"><span data-stu-id="7766a-108">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>

<span data-ttu-id="7766a-109">Da biste opozvali ili zamijenili poruku e-pošte:</span><span class="sxs-lookup"><span data-stu-id="7766a-109">To recall or replace an email message:</span></span>

1. <span data-ttu-id="7766a-110">U oknu mape s lijeve strane prozora programa Outlook odaberite mapu Poslane stavke.</span><span class="sxs-lookup"><span data-stu-id="7766a-110">In the folder pane on the left of the Outlook window, select the Sent Items folder.</span></span>
1. <span data-ttu-id="7766a-111">Dvokliknite poruku koju želite opozvati da biste je otvorili.</span><span class="sxs-lookup"><span data-stu-id="7766a-111">Double-click the message you want to recall to open it.</span></span>
1. <span data-ttu-id="7766a-112">Odaberite karticu **Poruka** , a zatim **Akcije**  >  **Opoziv ove poruke**.</span><span class="sxs-lookup"><span data-stu-id="7766a-112">Select the **Message** tab, and then select **Actions** > **Recall This Message**.</span></span>
1. <span data-ttu-id="7766a-113">Odaberite **Izbriši nepročitane kopije ove poruke** ili Izbriši **nepročitane kopije i zamijenite ga novom porukom**, a zatim odaberite U **redu**.</span><span class="sxs-lookup"><span data-stu-id="7766a-113">Select **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, and then select **OK**.</span></span>
1. <span data-ttu-id="7766a-114">Ako šaljete zamjensku poruku, sastavite poruku, a zatim odaberite **Pošalji**.</span><span class="sxs-lookup"><span data-stu-id="7766a-114">If you're sending a replacement message, compose the message, and then select **Send**.</span></span>
1. <span data-ttu-id="7766a-115">Uspjeh ili neuspjeh opoziva poruke ovisi o postavkama primatelja u programu Outlook.</span><span class="sxs-lookup"><span data-stu-id="7766a-115">The success or failure of a message recall depends on the recipient's settings in Outlook.</span></span> <span data-ttu-id="7766a-116">Upute za provjeru opoziva potražite u [ovom članku](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span><span class="sxs-lookup"><span data-stu-id="7766a-116">For steps to check on the recall, see [this article](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="7766a-117">Traženje i brisanje poruka e-pošte u tvrtki ili ustanovi</span><span class="sxs-lookup"><span data-stu-id="7766a-117">Search for and delete email messages in your organization</span></span>

- <span data-ttu-id="7766a-118">Ako niste globalni administrator, vaš račun mora biti dodan ulozi upravitelja predočavanja elektroničkih dokumenata ili ulozi upravljanja pretraživanjem usklađenosti da biste potražili poruke.</span><span class="sxs-lookup"><span data-stu-id="7766a-118">If you're not a global admin, your account must be added to the eDiscovery Manager role or Compliance Search management role to search for messages.</span></span> <span data-ttu-id="7766a-119">Da biste izbrisali poruke, morat ćete se pridružiti grupi uloga upravljanje organizacijom ili ulozi upravljanja pretraživanjem i čišćenjem.</span><span class="sxs-lookup"><span data-stu-id="7766a-119">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="7766a-120">Dozvole za te uloge dodijeljene su u [centru za sigurnost i usklađenost](https://go.microsoft.com/fwlink/?linkid=2083731).</span><span class="sxs-lookup"><span data-stu-id="7766a-120">Permissions for these roles are assigned in the [Security and compliance center](https://go.microsoft.com/fwlink/?linkid=2083731).</span></span>
- <span data-ttu-id="7766a-121">[Stvorite pretraživanje sadržaja](https://docs.microsoft.com/microsoft-365/compliance/content-search) da biste pronašli poruku koju želite izbrisati.</span><span class="sxs-lookup"><span data-stu-id="7766a-121">[Create a content search](https://docs.microsoft.com/microsoft-365/compliance/content-search) to find the message to delete.</span></span>
- <span data-ttu-id="7766a-122">[Povezivanje sa sigurnosnom jezgrom i powershell centrom za usklađenost](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="7766a-122">[Connect to Security and Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span></span>

<span data-ttu-id="7766a-123">Ako koristite višestruku provjeru autentičnosti, pročitajte mogućnost [Povezivanje sa sigurnošću sustava Microsoft 365 i PowerShell centar za usklađenost pomoću višestruke provjere autentičnosti](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="7766a-123">If you're using multi-factor authentication, see [Connect to Microsoft 365 security and Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span></span>