---
title: S/MIME u programu Outlook na webu
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 6915470655b85922f6f97e8ca6fac353224b1ae0
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36752852"
---
# <a name="encrypt-email-messages-in-outlook"></a><span data-ttu-id="fa5ab-102">Šifriranje poruke e-pošte u programu Outlook</span><span class="sxs-lookup"><span data-stu-id="fa5ab-102">Encrypt email messages in Outlook</span></span>

<span data-ttu-id="fa5ab-103">Šifriranje poruke Office 365 izgrađen na Microsoft Azure upravljanje pravima (Azure RMS), koji je dio Azure informacije zaštitu.</span><span class="sxs-lookup"><span data-stu-id="fa5ab-103">Office 365 Message Encryption is built on Microsoft Azure Rights Management (Azure RMS), which is part of Azure Information Protection.</span></span> <span data-ttu-id="fa5ab-104">Ako vaša pretplata uključuje Azure pravima ili zaštita Azure informacije **ne trebate poduzeti akcije ručno omogućiti ili aktivirati** uslugu upravljanja pravima.</span><span class="sxs-lookup"><span data-stu-id="fa5ab-104">If your subscription includes Azure Rights Management or Azure Information Protection, **you do not need to take any actions to manually enable or activate** the Rights Management Service.</span></span>

<span data-ttu-id="fa5ab-105">Na temelju povratnih smo će više neće biti omogućavanje pravila toka pošte Exchange automatski šifrirati izlaznog e-pošta koja sadrži određene vrste osjetljive informacije u vašem klijentske po zadanom.</span><span class="sxs-lookup"><span data-stu-id="fa5ab-105">Based on customer feedback, we will no longer be enabling Exchange mail flow rules to automatically encrypt outbound email containing certain type of sensitive information in your tenant by default.</span></span> <span data-ttu-id="fa5ab-106">Smo se umjesto toga pruža detaljne upute na kako to možete učiniti yourselves.</span><span class="sxs-lookup"><span data-stu-id="fa5ab-106">Instead, we are providing detailed instructions on how you can do so yourselves.</span></span> <span data-ttu-id="fa5ab-107">Za dodatne pojedinosti o tome kako stvoriti pravilo prijevoza za šifriranje osjetljivih informacija, pogledajte [Ovaj članak](https://aka.ms/OmeEtr).</span><span class="sxs-lookup"><span data-stu-id="fa5ab-107">For additional details on how to create a transport rule to encrypt sensitive information, see [this article](https://aka.ms/OmeEtr).</span></span>

- <span data-ttu-id="fa5ab-108">Ako pomoću programa Outlook na webu (prije **OWA**): kada sastavljate poruku e-pošte, jednostavno kliknite **zaštiti** u programu OWA.</span><span class="sxs-lookup"><span data-stu-id="fa5ab-108">If using Outlook on the Web (formerly **OWA**): When composing an email message, simply click **Protect** in OWA.</span></span> <span data-ttu-id="fa5ab-109">To će se primijeniti dozvole "Ne prosljeđuj".</span><span class="sxs-lookup"><span data-stu-id="fa5ab-109">This will apply "Do not forward" permission.</span></span> <span data-ttu-id="fa5ab-110">Kliknite **Promijeni dozvole** i odaberite **Šifriraj** samo šifrirati poruke.</span><span class="sxs-lookup"><span data-stu-id="fa5ab-110">Click **Change permission** and choose **Encrypt** to only encrypt the message.</span></span>

- <span data-ttu-id="fa5ab-111">Ako koristite **Outlook klijent**: poslati šifriranu poruku iz Outlook 2013 ili 2016 ili Outlook 2016 za Mac odaberite **Mogućnosti** > **dozvole**, a zatim odaberite mogućnost zaštite trebate.</span><span class="sxs-lookup"><span data-stu-id="fa5ab-111">If using **Outlook client**: To send an encrypted message from Outlook 2013 or 2016, or Outlook 2016 for Mac, select **Options** > **Permissions**, then select the protection option you need.</span></span>

- <span data-ttu-id="fa5ab-112">Da biste **automatski šifriranje sve e-pošte** šalju određene primatelje ili vanjski partner organizacijama, morate stvoriti pravilo toka prijevoza pošte u centru za administraciju sustava Exchange.</span><span class="sxs-lookup"><span data-stu-id="fa5ab-112">To **automatically encrypt all email** sent to certain recipients or external partner organizations, you need to create a mail flow transport rule in the Exchange Admin Center.</span></span> <span data-ttu-id="fa5ab-113">U [ovom članku za podršku](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities)se daju detaljne upute.</span><span class="sxs-lookup"><span data-stu-id="fa5ab-113">Detailed instructions are provided in [this support article](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities).</span></span>

