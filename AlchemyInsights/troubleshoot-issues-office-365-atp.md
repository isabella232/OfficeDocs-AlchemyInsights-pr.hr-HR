---
title: Otklanjanje poteškoća s asustavom Office 365 Advanced Threat Protection (ATP)
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: 99bc985f2d66693aca45f0833ab47c043acc1324
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766737"
---
# <a name="troubleshoot-issues-with-office-365-atp"></a><span data-ttu-id="8c1cf-102">Otklanjanje poteškoća s ATP-om sustava Office 365</span><span class="sxs-lookup"><span data-stu-id="8c1cf-102">Troubleshoot issues with Office 365 ATP</span></span>

- <span data-ttu-id="8c1cf-103">**Obavijest kašnjenja s isporukom e-pošte**poruka?</span><span class="sxs-lookup"><span data-stu-id="8c1cf-103">**Notice delays with email message delivery**?</span></span> <span data-ttu-id="8c1cf-104">Pokušajte koristiti mogućnost Dinamička isporuka za pravila o SIGURNIM PRIVICIMA ATP-a.</span><span class="sxs-lookup"><span data-stu-id="8c1cf-104">Try using the Dynamic Delivery option for your ATP Safe Attachments policies.</span></span> <span data-ttu-id="8c1cf-105">Time će se izbjeći kašnjenja isporuke poruka e-pošte uz zaštitu primatelja od zlonamjernih datoteka.</span><span class="sxs-lookup"><span data-stu-id="8c1cf-105">This will avoid email message delivery delays while protecting recipients from malicious files.</span></span>
- <span data-ttu-id="8c1cf-106">**Želite li prijaviti lažno pozitivan ili lažni negativ**?</span><span class="sxs-lookup"><span data-stu-id="8c1cf-106">**Do you want to report false positives or false negatives**?</span></span> <span data-ttu-id="8c1cf-107">Pomoću ovog linka pošaljite datoteku na analizu:[https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span><span class="sxs-lookup"><span data-stu-id="8c1cf-107">Use this link to submit your file for analysis: [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span></span>
- <span data-ttu-id="8c1cf-108">**Jeste li znali da možete omogućiti ATP safe links zaštitu za e-poštu poslanu između ljudi u vašoj organizaciji**?</span><span class="sxs-lookup"><span data-stu-id="8c1cf-108">**Did you know that you can enable ATP Safe Links protection for email sent between people in your organization**?</span></span> <span data-ttu-id="8c1cf-109">Slijedite ove korake:</span><span class="sxs-lookup"><span data-stu-id="8c1cf-109">Follow these steps:</span></span>
    1. <span data-ttu-id="8c1cf-110">Idite https://protection.office.comna i prijavite se.</span><span class="sxs-lookup"><span data-stu-id="8c1cf-110">Go to https://protection.office.com, and sign in.</span></span>
    2. <span data-ttu-id="8c1cf-111">Idite na Sigurnosne veze > **pravila upravljanja** >  **prijetnjama**.**Safe Links**</span><span class="sxs-lookup"><span data-stu-id="8c1cf-111">Go to **Threat management** > **Policy** > **Safe Links**.</span></span>
    3. <span data-ttu-id="8c1cf-112">U **odjeljku Pravila koja se primjenjuju na određene primatelje**uredite (ili dodajte) pravilo.</span><span class="sxs-lookup"><span data-stu-id="8c1cf-112">Under **Policies that apply to specific recipients**, edit (or add) a policy.</span></span>
    4. <span data-ttu-id="8c1cf-113">Odaberite **Primijeni sigurne veze na poruke poslane unutar organizacije**.</span><span class="sxs-lookup"><span data-stu-id="8c1cf-113">Select **Apply safe links to messages sent within the organization**.</span></span>
    5. <span data-ttu-id="8c1cf-114">Spremite pravila i dopustite da promjene funkcioniraju putem podatkovnog centra.</span><span class="sxs-lookup"><span data-stu-id="8c1cf-114">Save your policy, and allow about 30 minutes for your changes to work their way through your datacenter.</span></span>
- <span data-ttu-id="8c1cf-115">Dodatne pomoći za ATP potražite u članku [Napredna zaštita od prijetnji sustava Office 365](https://docs.microsoft.com/office365/securitycompliance/office-365-atp).</span><span class="sxs-lookup"><span data-stu-id="8c1cf-115">To get more help with ATP, see [Office 365 Advanced Threat Protection](https://docs.microsoft.com/office365/securitycompliance/office-365-atp).</span></span>