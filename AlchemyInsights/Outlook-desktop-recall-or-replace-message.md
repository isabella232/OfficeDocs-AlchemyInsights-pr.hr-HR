---
title: Outlook Desktop opoziv ili zamijeniti poruku e-pošte
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
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 10/25/2019
ms.locfileid: "36496103"
---
# <a name="recall-or-replace-an-outlook-email-message"></a><span data-ttu-id="db036-102">Opoziv ili zamjena poruke e-pošte programa Outlook</span><span class="sxs-lookup"><span data-stu-id="db036-102">Recall or replace an Outlook email message</span></span>

- <span data-ttu-id="db036-103">Kao administrator, možete **opozvati poruke u ime korisnika pomoću PowerShell**.</span><span class="sxs-lookup"><span data-stu-id="db036-103">As the admin, you can **recall messages on behalf of users using PowerShell**.</span></span> <span data-ttu-id="db036-104">Ne možete se sjetiti poruka iz centra za administraciju.</span><span class="sxs-lookup"><span data-stu-id="db036-104">You can't recall messages from the admin center.</span></span>
- <span data-ttu-id="db036-105">Možete se **prisjetiti samo poruka koje se šalju osobama u vašoj organizaciji**.</span><span class="sxs-lookup"><span data-stu-id="db036-105">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="db036-106">Ako je poruka poslana na Gmail adresu, na primjer, ne možete ga opozvati.</span><span class="sxs-lookup"><span data-stu-id="db036-106">If the message was sent to a Gmail address, for example, you can't recall it.</span></span>
- <span data-ttu-id="db036-107">Možete se **prisjetiti samo poruka poslane iz outlooka 2016 na PC-ju**.</span><span class="sxs-lookup"><span data-stu-id="db036-107">You can **only recall messages sent from Outlook 2016 on the PC**.</span></span> <span data-ttu-id="db036-108">Ako korisnik pošalje poruku pomoću programa Outlook za Mac ili Outlook na webu, ne možete ga opozvati.</span><span class="sxs-lookup"><span data-stu-id="db036-108">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>

<span data-ttu-id="db036-109">Da biste opozvali ili zamijenili poruku e-pošte:</span><span class="sxs-lookup"><span data-stu-id="db036-109">To recall or replace an email message:</span></span>

1. <span data-ttu-id="db036-110">U oknu mape s lijeve strane prozora programa Outlook odaberite mapu poslane stavke.</span><span class="sxs-lookup"><span data-stu-id="db036-110">In the folder pane on the left of the Outlook window, select the Sent Items folder.</span></span>
1. <span data-ttu-id="db036-111">Dvaput pritisnite poruku koju želite podsjetiti da biste je otvorili.</span><span class="sxs-lookup"><span data-stu-id="db036-111">Double-click the message you want to recall to open it.</span></span>
1. <span data-ttu-id="db036-112">Odaberite karticu **poruka** , a zatim odaberite **Akcije** > **Opozovi ovu poruku**.</span><span class="sxs-lookup"><span data-stu-id="db036-112">Select the **Message** tab, and then select **Actions** > **Recall This Message**.</span></span>
1. <span data-ttu-id="db036-113">Odaberite **Izbriši nepročitanih kopija ove poruke** ili **izbrišite nepročitanih kopija i zamijenite novom porukom**, a zatim odaberite **u redu**.</span><span class="sxs-lookup"><span data-stu-id="db036-113">Select **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, and then select **OK**.</span></span>
1. <span data-ttu-id="db036-114">Ako šaljete zamjensku poruku, sastavite poruku, a zatim odaberite **Pošalji**.</span><span class="sxs-lookup"><span data-stu-id="db036-114">If you're sending a replacement message, compose the message, and then select **Send**.</span></span>
1. <span data-ttu-id="db036-115">Uspjeh ili neuspjeh opoziv poruke ovisi o postavkama primatelja u programu Outlook.</span><span class="sxs-lookup"><span data-stu-id="db036-115">The success or failure of a message recall depends on the recipient's settings in Outlook.</span></span> <span data-ttu-id="db036-116">Za korake za provjeru opoziva pogledajte [ovaj članak](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span><span class="sxs-lookup"><span data-stu-id="db036-116">For steps to check on the recall, see [this article](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="db036-117">Traženje i brisanje poruka e-pošte u organizaciji</span><span class="sxs-lookup"><span data-stu-id="db036-117">Search for and delete email messages in your organization</span></span>

- <span data-ttu-id="db036-118">Ako niste globalni administrator, vaš račun mora biti dodan ulozi eDiscovery managera ili u ulozi za upravljanje pretraživanjem usklađenosti da biste potražili poruke.</span><span class="sxs-lookup"><span data-stu-id="db036-118">If you're not a global admin, your account must be added to the eDiscovery Manager role or Compliance Search management role to search for messages.</span></span> <span data-ttu-id="db036-119">Da biste izbrisali poruke, morate se pridružiti grupi uloga za upravljanje organizacijom ili u ulozi upravljanja pretraživanjem i pročišćavanja.</span><span class="sxs-lookup"><span data-stu-id="db036-119">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="db036-120">Dozvole za te uloge dodijeljene su u [centru za sigurnost i usklađenost](https://go.microsoft.com/fwlink/?linkid=2083731).</span><span class="sxs-lookup"><span data-stu-id="db036-120">Permissions for these roles are assigned in the [Security and compliance center](https://go.microsoft.com/fwlink/?linkid=2083731).</span></span>
- <span data-ttu-id="db036-121">[Stvorite pretraživanje sadržaja](https://docs.microsoft.com/office365/securitycompliance/content-search) da biste pronašli poruku koju želite izbrisati.</span><span class="sxs-lookup"><span data-stu-id="db036-121">[Create a content search](https://docs.microsoft.com/office365/securitycompliance/content-search) to find the message to delete.</span></span>
- <span data-ttu-id="db036-122">[Povežite se s PowerShell centrom za sigurnost i usklađenost](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="db036-122">[Connect to Security and Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span></span>

<span data-ttu-id="db036-123">Ako koristite multi-faktor provjeru autentičnosti, pogledajte [Povezivanje na Office 365 sigurnost i usklađenost centar PowerShell pomoću multi-faktor provjere autentičnosti](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="db036-123">If you're using multi-factor authentication, see [Connect to Office 365 Security and Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span></span>