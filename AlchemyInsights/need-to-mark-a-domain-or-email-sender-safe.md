---
title: Morate označiti domenu ili pošiljatelja e-pošte sigurnim?
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002921"
- "5673"
ms.openlocfilehash: a1c4c4d2fadaf75eda9b5b322aca35c32dfee8ea
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51792124"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a><span data-ttu-id="275f7-102">Morate označiti domenu ili pošiljatelja e-pošte sigurnim?</span><span class="sxs-lookup"><span data-stu-id="275f7-102">Need to mark a domain or email sender safe?</span></span>

- <span data-ttu-id="275f7-103">Korištenje popisa **sigurnih pošiljatelja ne preporučuje** se jer se u tvrtki ili ustanovi otvara neželjena pošta, fazani i lažni napadi.</span><span class="sxs-lookup"><span data-stu-id="275f7-103">Use of **safe sender lists is not recommended** since it opens up your organization to spam, phish, and spoofing attacks.</span></span>
- <span data-ttu-id="275f7-104">No ako postoji poslovni preduvjet, **preporučujemo** da za to koristite **[pravila tijeka](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** pošte.</span><span class="sxs-lookup"><span data-stu-id="275f7-104">However, if there is a business requirement, we **recommend** using **[Mail Flow Rules](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** for this.</span></span> <span data-ttu-id="275f7-105">Naše smjernice osiguravaju provjeru autentičnosti pošiljatelja (potvrđuje da se domena pošiljatelja ne može smućiti).</span><span class="sxs-lookup"><span data-stu-id="275f7-105">Our guidance ensures sender authentication (verifies sending domain is not being spoofed).</span></span> <span data-ttu-id="275f7-106">**Napomena:** ne preporučujemo upravljanje lažnim pozitivnim vrijednostima pomoću popisa sigurnih pošiljatelja jer iznimke od filtriranja neželjene pošte mogu otvoriti vašu organizaciju za sigurnosne napade.</span><span class="sxs-lookup"><span data-stu-id="275f7-106">**Note**: We don't recommend managing false positives by using safe sender lists, because exceptions to spam filtering can open your organization to security attacks.</span></span> <span data-ttu-id="275f7-107">Ako vaši korisnici primaju poruke koje su pogrešno označene kao neželjena ili bezvrijedna e-pošta, **[prijavite poruke i datoteke Microsoftu.](https://protection.office.com/reportsubmission)**</span><span class="sxs-lookup"><span data-stu-id="275f7-107">If your user(s) receive messages incorrectly marked as spam or junk email, please **[Report messages and files to Microsoft](https://protection.office.com/reportsubmission)**.</span></span>
- <span data-ttu-id="275f7-108">Sigurni pošiljatelji u programu Outlook, popis dopuštenih pošiljatelja  ili popis dopuštenih domena u pravilima za zaštitu od neželjene pošte moraju se izbjegavati jer pošiljatelji zaobilaze svu neželjenu poštu, podvala i phish zaštitu te provjeru autentičnosti pošiljatelja (SPF, DKIM, DMARC).</span><span class="sxs-lookup"><span data-stu-id="275f7-108">Safe Senders in Outlook, Allowed sender list, or allowed domain list in anti-spam policies **should be avoided** because senders bypass all spam, spoof, and phish protection, and sender authentication (SPF, DKIM, DMARC).</span></span> <span data-ttu-id="275f7-109">Ta se metoda najbolje koristi samo za privremeno testiranje.</span><span class="sxs-lookup"><span data-stu-id="275f7-109">This method is best used for temporary testing only.</span></span>
