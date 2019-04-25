---
title: Rješavanje problema s Office 365 Napredno prijetnja zaštite (ATP)
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/01/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: dbdfe2ddcc4afd4477f66ffd060ddb7093af8fd6
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32420288"
---
# <a name="troubleshoot-issues-with-office-365-atp"></a><span data-ttu-id="b577c-102">Rješavanje problema s Office 365 ATP</span><span class="sxs-lookup"><span data-stu-id="b577c-102">Troubleshoot issues with Office 365 ATP</span></span>

- <span data-ttu-id="b577c-103">**Kašnjenja obavijest s isporuka poruka e-pošte**?</span><span class="sxs-lookup"><span data-stu-id="b577c-103">**Notice delays with email message delivery**?</span></span> <span data-ttu-id="b577c-104">Pokušajte koristeći mogućnost dinamičke isporuke za pravila ATP sigurnom privitke.</span><span class="sxs-lookup"><span data-stu-id="b577c-104">Try using the Dynamic Delivery option for your ATP Safe Attachments policies.</span></span> <span data-ttu-id="b577c-105">To će izbjeći kašnjenja dostave poruka e-pošte dok primatelji Zaštita od zlonamjernih datoteke.</span><span class="sxs-lookup"><span data-stu-id="b577c-105">This will avoid email message delivery delays while protecting recipients from malicious files.</span></span>
- <span data-ttu-id="b577c-106">**Želite li izvješće positives false ili false Negacija**?</span><span class="sxs-lookup"><span data-stu-id="b577c-106">**Do you want to report false positives or false negatives**?</span></span> <span data-ttu-id="b577c-107">Koristite ovu vezu za slanje datoteka za analizu:[https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span><span class="sxs-lookup"><span data-stu-id="b577c-107">Use this link to submit your file for analysis: [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span></span>
- <span data-ttu-id="b577c-108">**Jeste li znali možete omogućiti veze sigurnom ATP zaštitu e-pošte poslane između osobe u vašoj organizaciji**?</span><span class="sxs-lookup"><span data-stu-id="b577c-108">**Did you know that you can enable ATP Safe Links protection for email sent between people in your organization**?</span></span> <span data-ttu-id="b577c-109">Slijedite ove korake:</span><span class="sxs-lookup"><span data-stu-id="b577c-109">Follow these steps:</span></span>
    1. <span data-ttu-id="b577c-110">Idi na https://protection.office.com, i prijavite se.</span><span class="sxs-lookup"><span data-stu-id="b577c-110">Go to https://protection.office.com, and sign in.</span></span>
    2. <span data-ttu-id="b577c-111">Idi na **Upravljanje prijetnja** > **pravila** > **Sigurne veze**.</span><span class="sxs-lookup"><span data-stu-id="b577c-111">Go to **Threat management** > **Policy** > **Safe Links**.</span></span>
    3. <span data-ttu-id="b577c-112">Pod **pravila koje se odnose na određene primatelje**uređivanje (ili dodavanje) pravila.</span><span class="sxs-lookup"><span data-stu-id="b577c-112">Under **Policies that apply to specific recipients**, edit (or add) a policy.</span></span>
    4. <span data-ttu-id="b577c-113">Odaberite **Primijeni sigurnom veze poruke šalju unutar organizacije**.</span><span class="sxs-lookup"><span data-stu-id="b577c-113">Select **Apply safe links to messages sent within the organization**.</span></span>
    5. <span data-ttu-id="b577c-114">Spremite pravilo i dopustiti otprilike 30 minuta za promjene rad njihove način kroz vaš datacenter.</span><span class="sxs-lookup"><span data-stu-id="b577c-114">Save your policy, and allow about 30 minutes for your changes to work their way through your datacenter.</span></span>
- <span data-ttu-id="b577c-115">Da biste dobili pomoć s ATP, pogledajte [Office 365 Napredno prijetnja zaštita](https://docs.microsoft.com/office365/securitycompliance/office-365-atp).</span><span class="sxs-lookup"><span data-stu-id="b577c-115">To get more help with ATP, see [Office 365 Advanced Threat Protection](https://docs.microsoft.com/office365/securitycompliance/office-365-atp).</span></span>