---
title: Antispam - 5.7.23
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: e494e8017f24d65a94d1a7490be4d67c46a2120b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821403"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a><span data-ttu-id="c5d1e-102">Rješavanje problema s isporukom e-pošte za kod pogreške 5.7.23</span><span class="sxs-lookup"><span data-stu-id="c5d1e-102">Fix email delivery issues for error code 5.7.23</span></span>

<span data-ttu-id="c5d1e-103">Provjerite SPF DNS zapis za svoju domenu na javno dostupnoj provjeri SPF ili DNS zapisa na webu.</span><span class="sxs-lookup"><span data-stu-id="c5d1e-103">Verify the SPF DNS record for your domain at a publicly available SPF or DNS record checker on the web.</span></span>

<span data-ttu-id="c5d1e-104">Provjerite nije li Microsoft prepoznao izlaznu poruku kao neželjenu poštu i usmjeravao je putem centra za isporuku [visokog rizika](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages).</span><span class="sxs-lookup"><span data-stu-id="c5d1e-104">Verify that the outbound message wasn't identified as spam by Microsoft and routed through the [High Risk Delivery Pool](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages).</span></span> <span data-ttu-id="c5d1e-105">Poruke u visokorizičnoj isporuci neće proći provjere SPF-a, pa je stoga odredišna tvrtka ili ustanova za e-poštu neće prihvatiti.</span><span class="sxs-lookup"><span data-stu-id="c5d1e-105">Messages in the High Risk Delivery Pool won't pass SPF checks, and therefore won't be accepted by the destination email organization.</span></span>

<span data-ttu-id="c5d1e-106">Ako se problem nastavi pojavljivati, možda ćete se morati obratiti administratoru glavnog računala e-pošte kojemu pokušavate poslati poruku e-pošte.</span><span class="sxs-lookup"><span data-stu-id="c5d1e-106">If the problem persists, you may need to contact the admin of the mail host to which you are attempting to send email.</span></span> <span data-ttu-id="c5d1e-107">Zabilježite detaljnu vanjsku pogrešku koja je dostupna u poruci o odskoci.</span><span class="sxs-lookup"><span data-stu-id="c5d1e-107">Make note of the detailed external error available in the bounce message.</span></span> <span data-ttu-id="c5d1e-108">Microsoftova podrška možda neće moći dodatno pomoći.</span><span class="sxs-lookup"><span data-stu-id="c5d1e-108">Microsoft support may not be able to assist further.</span></span>
