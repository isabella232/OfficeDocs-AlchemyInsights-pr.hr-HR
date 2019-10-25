---
title: Antispam-5.7.23
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
ms.openlocfilehash: 9c9bc2d04fb8efaa5e75194b4ca09316d24e018e
ms.sourcegitcommit: 07b47d7f3ca191363e6bc84140e8e01524d6f08e
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 10/24/2019
ms.locfileid: "37682066"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a><span data-ttu-id="64802-102">Popravak problema isporuke e-pošte za kôd pogreške 5.7.23</span><span class="sxs-lookup"><span data-stu-id="64802-102">Fix email delivery issues for error code 5.7.23</span></span>

<span data-ttu-id="64802-103">Provjerite SPF DNS zapis za svoju domenu na javno dostupnom SPF ili DNS zapisu za provjeru na webu.</span><span class="sxs-lookup"><span data-stu-id="64802-103">Verify the SPF DNS record for your domain at a publicly available SPF or DNS record checker on the web.</span></span>

<span data-ttu-id="64802-104">Provjerite je li pošta u izlaznim porukama identificirana kao spam od strane sustava Office 365 i preusmjeren kroz [skup visokih rizika](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages).</span><span class="sxs-lookup"><span data-stu-id="64802-104">Verify that the outbound message wasn't identified as spam by Office 365 and routed through the [High Risk Delivery Pool](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages).</span></span> <span data-ttu-id="64802-105">Poruke u bazenu velike rizike dostave neće proći SPF provjere i stoga neće biti prihvaćena od strane odredišne organizacije e-pošte.</span><span class="sxs-lookup"><span data-stu-id="64802-105">Messages in the High Risk Delivery Pool won't pass SPF checks, and therefore won't be accepted by the destination email organization.</span></span>

<span data-ttu-id="64802-106">Ako se problem nastavi pojavljivati, možda ćete morati kontaktirati admin host pošte na koji pokušavate poslati e-poštu.</span><span class="sxs-lookup"><span data-stu-id="64802-106">If the problem persists, you may need to contact the admin of the mail host to which you are attempting to send email.</span></span> <span data-ttu-id="64802-107">Zabilježite detaljnu vanjsku grešku dostupnu u poruci napuštanja početne stranice.</span><span class="sxs-lookup"><span data-stu-id="64802-107">Make note of the detailed external error available in the bounce message.</span></span>  <span data-ttu-id="64802-108">Office 365 podrška možda neće moći dodatno pomoći.</span><span class="sxs-lookup"><span data-stu-id="64802-108">Office 365 support may not be able to assist further.</span></span>