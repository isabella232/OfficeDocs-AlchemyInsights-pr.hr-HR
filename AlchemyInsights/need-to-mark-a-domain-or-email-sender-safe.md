---
title: Želite li sigurno označiti domenu ili pošiljatelja e-pošte?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002921"
- "5673"
ms.openlocfilehash: 0ea089b95ad7de25e77017196fb2db895d4d0178
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47803237"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a><span data-ttu-id="76a6e-102">Želite li sigurno označiti domenu ili pošiljatelja e-pošte?</span><span class="sxs-lookup"><span data-stu-id="76a6e-102">Need to mark a domain or email sender safe?</span></span>

- <span data-ttu-id="76a6e-103">Korištenje **popisa sigurnih pošiljatelja ne preporučuje se** budući da otvara vašu tvrtku ili ustanovu za napade neželjene pošte, Phish i podvala.</span><span class="sxs-lookup"><span data-stu-id="76a6e-103">Use of **safe sender lists is not recommended** since it opens up your organization to spam, phish, and spoofing attacks.</span></span>
- <span data-ttu-id="76a6e-104">No ako postoji zahtjev za tvrtke, **preporučujemo** da za to koristite **[pravila protoka pošte](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** .</span><span class="sxs-lookup"><span data-stu-id="76a6e-104">However, if there is a business requirement, we **recommend** using **[Mail Flow Rules](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** for this.</span></span> <span data-ttu-id="76a6e-105">Našim smjernicama osigurana je provjera autentičnosti pošiljatelja (verificirana domena slanja nije varalica).</span><span class="sxs-lookup"><span data-stu-id="76a6e-105">Our guidance ensures sender authentication (verifies sending domain is not being spoofed).</span></span> <span data-ttu-id="76a6e-106">**Pažnja**: ne preporučujemo upravljanje lažnim pozitivnim dodacima pomoću popisa sigurnih pošiljatelja jer iznimke za filtriranje neželjene pošte mogu otvoriti vašu tvrtku ili ustanovu za sigurnosne napade.</span><span class="sxs-lookup"><span data-stu-id="76a6e-106">**Note**: We don't recommend managing false positives by using safe sender lists, because exceptions to spam filtering can open your organization to security attacks.</span></span> <span data-ttu-id="76a6e-107">Ako vaši korisnici na pogrešan način primaju poruke označene kao neželjene ili bezvrijedne e-pošte, **[prijavite poruke i datoteke Microsoftu](https://protection.office.com/reportsubmission)**.</span><span class="sxs-lookup"><span data-stu-id="76a6e-107">If your user(s) receive messages incorrectly marked as spam or junk email, please **[Report messages and files to Microsoft](https://protection.office.com/reportsubmission)**.</span></span>
- <span data-ttu-id="76a6e-108">Sigurni pošiljatelji u programu Outlook, dopušteni popis pošiljatelja ili dopušteni popis domena u pravilima protiv neželjene pošte **moraju se izbjegavati** jer pošiljatelji zaobilaženje svih neželjenih poruka, podvala i Phish zaštite te provjere autentičnosti POŠILJATELJA (SPF, debiran, d).</span><span class="sxs-lookup"><span data-stu-id="76a6e-108">Safe Senders in Outlook, Allowed sender list, or allowed domain list in anti-spam policies **should be avoided** because senders bypass all spam, spoof, and phish protection, and sender authentication (SPF, DKIM, DMARC).</span></span> <span data-ttu-id="76a6e-109">Ovaj se način najbolje koristi samo za privremeno testiranje.</span><span class="sxs-lookup"><span data-stu-id="76a6e-109">This method is best used for temporary testing only.</span></span>
