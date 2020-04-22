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
ms.openlocfilehash: 307b738c40c620d057e68eff7d218c8c9b5eb665
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43676489"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a><span data-ttu-id="149a2-102">Rješavanje problema s isporukom e-pošte za kod pogreške 5.7.23</span><span class="sxs-lookup"><span data-stu-id="149a2-102">Fix email delivery issues for error code 5.7.23</span></span>

<span data-ttu-id="149a2-103">Provjerite SPF DNS zapis za svoju domenu na javno dostupnom SPF ili DNS provjeru zapisa na webu.</span><span class="sxs-lookup"><span data-stu-id="149a2-103">Verify the SPF DNS record for your domain at a publicly available SPF or DNS record checker on the web.</span></span>

<span data-ttu-id="149a2-104">Provjerite nije li Microsoft identificirao odlaznu poruku kao neželjenu poštu i usmjerio se putem grupe za [isporuku visokog rizika](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages).</span><span class="sxs-lookup"><span data-stu-id="149a2-104">Verify that the outbound message wasn't identified as spam by Microsoft and routed through the [High Risk Delivery Pool](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages).</span></span> <span data-ttu-id="149a2-105">Poruke u skupu za isporuku visokog rizika neće proći SPF čekove i stoga ih odredišna organizacija e-pošte neće prihvatiti.</span><span class="sxs-lookup"><span data-stu-id="149a2-105">Messages in the High Risk Delivery Pool won't pass SPF checks, and therefore won't be accepted by the destination email organization.</span></span>

<span data-ttu-id="149a2-106">Ako se problem nastavi pojavljivati, možda ćete se morati obratiti administratoru glavnog računala pošte kojem pokušavate poslati e-poštu.</span><span class="sxs-lookup"><span data-stu-id="149a2-106">If the problem persists, you may need to contact the admin of the mail host to which you are attempting to send email.</span></span> <span data-ttu-id="149a2-107">Zabilježite detaljnu vanjsku pogrešku dostupnu u poruci napuštanja početne stranice.</span><span class="sxs-lookup"><span data-stu-id="149a2-107">Make note of the detailed external error available in the bounce message.</span></span> <span data-ttu-id="149a2-108">Microsoftova podrška možda neće moći dodatno pomoći.</span><span class="sxs-lookup"><span data-stu-id="149a2-108">Microsoft support may not be able to assist further.</span></span>
