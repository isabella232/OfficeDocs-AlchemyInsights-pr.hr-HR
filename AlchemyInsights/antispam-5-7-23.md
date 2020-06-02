---
title: Antispam - 5.7.23
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: 8122b409a731a5fcc46c718aff1eeda07e26890b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506435"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a><span data-ttu-id="e1f6d-102">Rješavanje problema s isporukom e-pošte za kod pogreške 5.7.23</span><span class="sxs-lookup"><span data-stu-id="e1f6d-102">Fix email delivery issues for error code 5.7.23</span></span>

<span data-ttu-id="e1f6d-103">Provjerite SPF DNS zapis za svoju domenu na javno dostupnom SPF ili DNS zapisu na webu.</span><span class="sxs-lookup"><span data-stu-id="e1f6d-103">Verify the SPF DNS record for your domain at a publicly available SPF or DNS record checker on the web.</span></span>

<span data-ttu-id="e1f6d-104">Provjerite nije li Microsoft identificirao odlaznu poruku kao neželjenu poštu i da je preusmjeren kroz bazen za [isporuku visokog rizika](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages).</span><span class="sxs-lookup"><span data-stu-id="e1f6d-104">Verify that the outbound message wasn't identified as spam by Microsoft and routed through the [High Risk Delivery Pool](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages).</span></span> <span data-ttu-id="e1f6d-105">Poruke u skupu za isporuku visokog rizika neće proći SPF provjere i stoga neće biti prihvaćene od strane odredišne organizacije e-pošte.</span><span class="sxs-lookup"><span data-stu-id="e1f6d-105">Messages in the High Risk Delivery Pool won't pass SPF checks, and therefore won't be accepted by the destination email organization.</span></span>

<span data-ttu-id="e1f6d-106">Ako se problem nastavi pojavljivati, možda ćete se morati obratiti administratoru glavnog računala e-pošte kojem pokušavate poslati e-poštu.</span><span class="sxs-lookup"><span data-stu-id="e1f6d-106">If the problem persists, you may need to contact the admin of the mail host to which you are attempting to send email.</span></span> <span data-ttu-id="e1f6d-107">Zabilježite detaljnu vanjsku pogrešku dostupnu u poruci napuštanja početne stranice.</span><span class="sxs-lookup"><span data-stu-id="e1f6d-107">Make note of the detailed external error available in the bounce message.</span></span> <span data-ttu-id="e1f6d-108">Microsoftova podrška možda neće moći dalje pomagati.</span><span class="sxs-lookup"><span data-stu-id="e1f6d-108">Microsoft support may not be able to assist further.</span></span>
