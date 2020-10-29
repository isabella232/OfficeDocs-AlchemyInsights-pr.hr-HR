---
title: Otklanjanje poteškoća s programom Microsoft Defender za Office 365 (ATP)
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: cf54d5b3b854587202ff1b575889b9602228dd06
ms.sourcegitcommit: 4caf5e6c2fee2903ccaf92cfc9006eb580faa7ba
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 10/29/2020
ms.locfileid: "48801399"
---
# <a name="troubleshoot-issues-with-office-365-atp"></a><span data-ttu-id="d7d22-102">Otklanjanje poteškoća sa sustavom Office 365 ATP</span><span class="sxs-lookup"><span data-stu-id="d7d22-102">Troubleshoot issues with Office 365 ATP</span></span>

- <span data-ttu-id="d7d22-103">**Obavijest o zastojima uz isporuku poruke e-pošte** ?</span><span class="sxs-lookup"><span data-stu-id="d7d22-103">**Notice delays with email message delivery** ?</span></span> <span data-ttu-id="d7d22-104">Pokušajte koristiti dinamičku mogućnost isporuke za svoje pravilnike o sigurnim prilozima.</span><span class="sxs-lookup"><span data-stu-id="d7d22-104">Try using the Dynamic Delivery option for your ATP Safe Attachments policies.</span></span> <span data-ttu-id="d7d22-105">Time će se izbjegavati kašnjenje isporuke poruka e-pošte dok se primatelji štite od zlonamjernih datoteka.</span><span class="sxs-lookup"><span data-stu-id="d7d22-105">This will avoid email message delivery delays while protecting recipients from malicious files.</span></span>
- <span data-ttu-id="d7d22-106">**Želite li prijaviti FALSE pozitivni ili lažni negativi** ?</span><span class="sxs-lookup"><span data-stu-id="d7d22-106">**Do you want to report false positives or false negatives** ?</span></span> <span data-ttu-id="d7d22-107">Upotrijebite ovu vezu da biste poslali datoteku za analizu: [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span><span class="sxs-lookup"><span data-stu-id="d7d22-107">Use this link to submit your file for analysis: [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span></span>
- <span data-ttu-id="d7d22-108">**Jeste li znali da možete omogućiti ATP sigurne veze zaštite za e-poštu poslanu među osobama u vašoj tvrtki ili ustanovi** ?</span><span class="sxs-lookup"><span data-stu-id="d7d22-108">**Did you know that you can enable ATP Safe Links protection for email sent between people in your organization** ?</span></span> <span data-ttu-id="d7d22-109">Slijedite ove korake:</span><span class="sxs-lookup"><span data-stu-id="d7d22-109">Follow these steps:</span></span>
    1. <span data-ttu-id="d7d22-110">Idite na https://protection.office.com , a zatim se prijavite.</span><span class="sxs-lookup"><span data-stu-id="d7d22-110">Go to https://protection.office.com, and sign in.</span></span>
    2. <span data-ttu-id="d7d22-111">Idite na **Threat management**  >  **Policy**  >  **sigurne veze** u pravilima upravljanja prijetnjama.</span><span class="sxs-lookup"><span data-stu-id="d7d22-111">Go to **Threat management** > **Policy** > **Safe Links** .</span></span>
    3. <span data-ttu-id="d7d22-112">U odjeljku **pravila koja se primjenjuju na određene primatelje** uredite (ili dodajte) pravilo.</span><span class="sxs-lookup"><span data-stu-id="d7d22-112">Under **Policies that apply to specific recipients** , edit (or add) a policy.</span></span>
    4. <span data-ttu-id="d7d22-113">Odaberite **Primijeni sigurne veze na poruke poslane unutar tvrtke ili ustanove** .</span><span class="sxs-lookup"><span data-stu-id="d7d22-113">Select **Apply safe links to messages sent within the organization** .</span></span>
    5. <span data-ttu-id="d7d22-114">Spremite pravilo i dopustite oko 30 minuta da vaše promjene funkcioniraju na svoj način putem podatkovnog programa.</span><span class="sxs-lookup"><span data-stu-id="d7d22-114">Save your policy, and allow about 30 minutes for your changes to work their way through your datacenter.</span></span>
- <span data-ttu-id="d7d22-115">Da biste dobili dodatnu pomoć za ATP, pročitajte članak [Microsoft Defender za Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp).</span><span class="sxs-lookup"><span data-stu-id="d7d22-115">To get more help with ATP, see [Microsoft Defender for Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp).</span></span>