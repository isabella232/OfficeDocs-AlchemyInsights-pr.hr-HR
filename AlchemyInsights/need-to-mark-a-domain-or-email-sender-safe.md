---
title: Trebate označiti sigurnu domenu ili pošiljatelja e-pošte?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002921"
- "5673"
ms.openlocfilehash: 7dc1576fd61e87b319c7486c59ed125943b4d959
ms.sourcegitcommit: 43acdecef129bfffc8bbe8ebb08fdd581b238a03
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 05/18/2020
ms.locfileid: "44281128"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a><span data-ttu-id="4e979-102">Trebate označiti sigurnu domenu ili pošiljatelja e-pošte?</span><span class="sxs-lookup"><span data-stu-id="4e979-102">Need to mark a domain or email sender safe?</span></span>

- <span data-ttu-id="4e979-103">Korištenje **popisa sigurnih pošiljatelja ne preporučuje se** jer otvara vašu tvrtku ili ustanovu za neželjenu poštu, krađu identiteta i lažne napade.</span><span class="sxs-lookup"><span data-stu-id="4e979-103">Use of **safe sender lists is not recommended** since it opens up your organization to spam, phish, and spoofing attacks.</span></span>
- <span data-ttu-id="4e979-104">Međutim, ako postoji poslovni preduvjet, **preporučujemo** da za to koristite **[pravila tijeka pošte.](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)**</span><span class="sxs-lookup"><span data-stu-id="4e979-104">However, if there is a business requirement, we **recommend** using **[Mail Flow Rules](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** for this.</span></span> <span data-ttu-id="4e979-105">Naše upute osiguravaju provjeru autentičnosti pošiljatelja (provjerava da se domena slanja ne zavarava).</span><span class="sxs-lookup"><span data-stu-id="4e979-105">Our guidance ensures sender authentication (verifies sending domain is not being spoofed).</span></span> <span data-ttu-id="4e979-106">**Napomena:** Ne preporučujemo upravljanje lažnim pozitivnim korištenjem popisa sigurnih pošiljatelja jer iznimke od filtriranja neželjene pošte mogu otvoriti vašu tvrtku ili ustanovu sigurnosnim napadima.</span><span class="sxs-lookup"><span data-stu-id="4e979-106">**Note**: We don't recommend managing false positives by using safe sender lists, because exceptions to spam filtering can open your organization to security attacks.</span></span> <span data-ttu-id="4e979-107">Ako vaši korisnici primaju poruke neispravno označene kao neželjena ili bezvrijedna e-pošta, **[prijavite poruke i datoteke Microsoftu](https://protection.office.com/reportsubmission)**.</span><span class="sxs-lookup"><span data-stu-id="4e979-107">If your user(s) receive messages incorrectly marked as spam or junk email, please **[Report messages and files to Microsoft](https://protection.office.com/reportsubmission)**.</span></span>
- <span data-ttu-id="4e979-108">Popis sigurnih pošiljatelja u programu Outlook, popisu dopuštenih pošiljatelja ili dopuštenom popisu domena u pravilima protiv neželjene pošte **treba izbjegavati** jer pošiljatelji zaobilaze svu neželjenu poštu, lažnu i zaštitu od krađe identiteta te provjeru autentičnosti pošiljatelja (SPF, DKIM, DMARC).</span><span class="sxs-lookup"><span data-stu-id="4e979-108">Safe Senders in Outlook, Allowed sender list, or allowed domain list in anti-spam policies **should be avoided** because senders bypass all spam, spoof, and phish protection, and sender authentication (SPF, DKIM, DMARC).</span></span> <span data-ttu-id="4e979-109">Ova metoda je najbolje koristiti samo za privremeno testiranje.</span><span class="sxs-lookup"><span data-stu-id="4e979-109">This method is best used for temporary testing only.</span></span>
