---
title: Outlook desktopa opoziv ili zamjena poruke e-pošte
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: 578e2690061286bde74ee0b4b74a197630716f59
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663982"
---
# <a name="recall-or-replace-an-outlook-email-message"></a><span data-ttu-id="d7ddd-102">Opoziv ili zamjena poruke e-pošte programa Outlook</span><span class="sxs-lookup"><span data-stu-id="d7ddd-102">Recall or replace an Outlook email message</span></span>

- <span data-ttu-id="d7ddd-103">Kao administrator možete **opozvati poruke u ime korisnika pomoću komponente PowerShell**.</span><span class="sxs-lookup"><span data-stu-id="d7ddd-103">As the admin, you can **recall messages on behalf of users using PowerShell**.</span></span> <span data-ttu-id="d7ddd-104">Ne možete se prisjetiti poruka iz centra za administratore.</span><span class="sxs-lookup"><span data-stu-id="d7ddd-104">You can't recall messages from the admin center.</span></span>
- <span data-ttu-id="d7ddd-105">Možete se **prisjetiti samo poruka koje se šalju osobama u vašoj tvrtki ili ustanovi**.</span><span class="sxs-lookup"><span data-stu-id="d7ddd-105">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="d7ddd-106">Ako je poruka poslana na adresu servisa Gmail, na primjer, ne možete je opozvati.</span><span class="sxs-lookup"><span data-stu-id="d7ddd-106">If the message was sent to a Gmail address, for example, you can't recall it.</span></span>
- <span data-ttu-id="d7ddd-107">Možete se **prisjetiti samo poruka poslane iz programa Outlook 2016 na PC-ju**.</span><span class="sxs-lookup"><span data-stu-id="d7ddd-107">You can **only recall messages sent from Outlook 2016 on the PC**.</span></span> <span data-ttu-id="d7ddd-108">Ako korisnik pošalje poruku pomoću programa Outlook za Mac ili Outlook na webu, ne možete je opozvati.</span><span class="sxs-lookup"><span data-stu-id="d7ddd-108">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>

<span data-ttu-id="d7ddd-109">Opoziv ili zamjena poruke e-pošte:</span><span class="sxs-lookup"><span data-stu-id="d7ddd-109">To recall or replace an email message:</span></span>

1. <span data-ttu-id="d7ddd-110">U oknu s mapama na lijevoj strani prozora programa Outlook odaberite mapu poslane stavke.</span><span class="sxs-lookup"><span data-stu-id="d7ddd-110">In the folder pane on the left of the Outlook window, select the Sent Items folder.</span></span>
1. <span data-ttu-id="d7ddd-111">Dvokliknite poruku koju želite opozvati da biste je otvorili.</span><span class="sxs-lookup"><span data-stu-id="d7ddd-111">Double-click the message you want to recall to open it.</span></span>
1. <span data-ttu-id="d7ddd-112">Odaberite karticu **poruka** , a zatim odaberite **Akcije**  >  **Opoziv ove poruke**.</span><span class="sxs-lookup"><span data-stu-id="d7ddd-112">Select the **Message** tab, and then select **Actions** > **Recall This Message**.</span></span>
1. <span data-ttu-id="d7ddd-113">Odaberite **Izbriši nepročitane kopije ove poruke** ili **izbrišite nepročitane kopije i zamijenite je novom porukom**, a zatim odaberite **u redu**.</span><span class="sxs-lookup"><span data-stu-id="d7ddd-113">Select **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, and then select **OK**.</span></span>
1. <span data-ttu-id="d7ddd-114">Ako šaljete zamjensku poruku, sastavite poruku, a zatim odaberite Send ( **Šalji**).</span><span class="sxs-lookup"><span data-stu-id="d7ddd-114">If you're sending a replacement message, compose the message, and then select **Send**.</span></span>
1. <span data-ttu-id="d7ddd-115">Uspjeh ili neuspjeh opoziv poruke ovisi o postavkama primatelja u programu Outlook.</span><span class="sxs-lookup"><span data-stu-id="d7ddd-115">The success or failure of a message recall depends on the recipient's settings in Outlook.</span></span> <span data-ttu-id="d7ddd-116">Upute za provjeru opoziv potražite u [ovom članku](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span><span class="sxs-lookup"><span data-stu-id="d7ddd-116">For steps to check on the recall, see [this article](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="d7ddd-117">Traženje i brisanje poruka e-pošte u tvrtki ili ustanovi</span><span class="sxs-lookup"><span data-stu-id="d7ddd-117">Search for and delete email messages in your organization</span></span>

- <span data-ttu-id="d7ddd-118">Ako niste globalni administrator, vaš račun mora biti dodan u ulogu upravitelja programa za otkrivanje ili usklađenost pretraživanja da biste potražili poruke.</span><span class="sxs-lookup"><span data-stu-id="d7ddd-118">If you're not a global admin, your account must be added to the eDiscovery Manager role or Compliance Search management role to search for messages.</span></span> <span data-ttu-id="d7ddd-119">Da biste izbrisali poruke, morat ćete se pridružiti grupi uloga za upravljanje organizacijom ili ulogu pretraživanja i brisanja.</span><span class="sxs-lookup"><span data-stu-id="d7ddd-119">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="d7ddd-120">Dozvole za ove uloge dodijeljene su u [centru za sigurnost i usklađenost](https://go.microsoft.com/fwlink/?linkid=2083731).</span><span class="sxs-lookup"><span data-stu-id="d7ddd-120">Permissions for these roles are assigned in the [Security and compliance center](https://go.microsoft.com/fwlink/?linkid=2083731).</span></span>
- <span data-ttu-id="d7ddd-121">[Stvorite pretraživanje sadržaja](https://docs.microsoft.com/microsoft-365/compliance/content-search) da biste pronašli poruku koja će se izbrisati.</span><span class="sxs-lookup"><span data-stu-id="d7ddd-121">[Create a content search](https://docs.microsoft.com/microsoft-365/compliance/content-search) to find the message to delete.</span></span>
- <span data-ttu-id="d7ddd-122">[Spojite se na PowerShell centra za sigurnost i usklađenost](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="d7ddd-122">[Connect to Security and Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span></span>

<span data-ttu-id="d7ddd-123">Ako koristite višestruka provjera autentičnosti, pročitajte članak [Povezivanje s pomoću komponente Security i centar za usklađenost s microsoftovim 365 uz multi-Factor](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="d7ddd-123">If you're using multi-factor authentication, see [Connect to Microsoft 365 security and Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span></span>