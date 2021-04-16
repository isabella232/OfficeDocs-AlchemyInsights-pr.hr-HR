---
title: Jesu li korisnici primili zlonamjernu e-poštu
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
- "9002907"
- "5594"
- "3100017"
- "2578"
ms.openlocfilehash: 425f9ba488fd69b8c5ea29636bccccd995bf48fd
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51815238"
---
# <a name="did-your-users-receive-malicious-email"></a><span data-ttu-id="b3738-102">Jesu li korisnici primili zlonamjernu e-poštu?</span><span class="sxs-lookup"><span data-stu-id="b3738-102">Did your users receive malicious email?</span></span>

- <span data-ttu-id="b3738-103">Sada možete prijaviti zlonamjernu e-poštu Microsoftu pomoću poslanih [administratora u centru za & usklađenosti](https://sip.protection.office.com/reportsubmission).</span><span class="sxs-lookup"><span data-stu-id="b3738-103">You can now report the malicious email to Microsoft using the [Admin Submissions in Security & Compliance Center](https://sip.protection.office.com/reportsubmission).</span></span>

<span data-ttu-id="b3738-104">Poruke poslane u [podnescima administratora](https://sip.protection.office.com/reportsubmission) skeniraju se i sljedeći rezultati prikazani u podlošci detalja: </span><span class="sxs-lookup"><span data-stu-id="b3738-104">Messages that are submitted in [admin submissions](https://sip.protection.office.com/reportsubmission) are scanned, and the following results shown in the **details** flyout:</span></span>

- <span data-ttu-id="b3738-105">Ako je prilikom isporuke došlo do pogreške u provjeri autentičnosti e-pošte pošiljatelja.</span><span class="sxs-lookup"><span data-stu-id="b3738-105">If there was a failure in the sender's email authentication at the time of delivery.</span></span>
- <span data-ttu-id="b3738-106">Informacije o učitavanjima pravilnika koje su mogle utjecati na ili nadjačati presudu poruke.</span><span class="sxs-lookup"><span data-stu-id="b3738-106">Information about any policy hits that could have affected or overridden the verdict of a message.</span></span>
- <span data-ttu-id="b3738-107">Trenutni rezultati detonacije da biste vidjeli jesu li URL-ovi ili datoteke sadržane u poruci zlonamjerni ili ne.</span><span class="sxs-lookup"><span data-stu-id="b3738-107">Current detonation results to see if the URLs or files contained in the message were malicious or not.</span></span>
- <span data-ttu-id="b3738-108">Povratne informacije od gradera</span><span class="sxs-lookup"><span data-stu-id="b3738-108">Feedback from graders</span></span>

<span data-ttu-id="b3738-109">Ako je nadjačavanje pronađeno, ponovno se može dovršiti za nekoliko minuta.</span><span class="sxs-lookup"><span data-stu-id="b3738-109">If an override was found, the rescan should complete in several minutes.</span></span> <span data-ttu-id="b3738-110">Ako nije bilo problema s provjerom autentičnosti e-pošte ili ako nadjačavanje nije utjecalo na isporuku, povratne informacije od gradera mogle bi potrajati i do jednog dana.</span><span class="sxs-lookup"><span data-stu-id="b3738-110">If there wasn't a problem in email authentication or if the delivery wasn't affected by an override, then the feedback from graders could take up to a day.</span></span>

<span data-ttu-id="b3738-111">Ako se ne slažete s konačnom presudom o poruci, URL-u ili datoteci (blokirano vs. nije blokirano), ponovno pošaljite poruku nakon jednog dana radi ponovnog slanja.</span><span class="sxs-lookup"><span data-stu-id="b3738-111">If you disagree with the final verdict on a message, URL or file (blocked vs. not blocked), submit the message again after a day for rescan.</span></span> <span data-ttu-id="b3738-112">Velike su šanse da će se nakon slanja poruke ponovno promijeniti odluka.</span><span class="sxs-lookup"><span data-stu-id="b3738-112">The chances are high that the verdict would change after submitting the message again.</span></span>

<span data-ttu-id="b3738-113">U međuvremenu možete ukloniti zlonamjernu e-poštu iz korisničkih uštenih okvira slijedeći upute [u ovom članku.](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)</span><span class="sxs-lookup"><span data-stu-id="b3738-113">Meanwhile, you can remove malicious email from user inboxes by following the instructions in [this article](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization).</span></span>

- <span data-ttu-id="b3738-114">Korisnici s programom Microsoft Defender za Office 365 mogu:</span><span class="sxs-lookup"><span data-stu-id="b3738-114">Customers with Microsoft Defender for Office 365 can:</span></span>
    - <span data-ttu-id="b3738-115">Traženje [i brisanje sumnjive e-pošte pomoću eksplorera za prijetnje](https://docs.microsoft.com/microsoft-365/security/office-365-security/investigate-malicious-email-that-was-delivered)</span><span class="sxs-lookup"><span data-stu-id="b3738-115">use [Threat Explorer to Find and Delete Suspicious email](https://docs.microsoft.com/microsoft-365/security/office-365-security/investigate-malicious-email-that-was-delivered)</span></span>
    - <span data-ttu-id="b3738-116">[blokiranje pristupa zlonamjernom URL-u pomoću](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-safe-links) sigurnih veza</span><span class="sxs-lookup"><span data-stu-id="b3738-116">[use Safe Links to block access](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-safe-links) to a malicious URL</span></span>
    - <span data-ttu-id="b3738-117">praćenje korisnika koji su klikali i pristupali zlonamjernim URL-ovima: Prikaz URL-a za [krađu identiteta i klika](https://docs.microsoft.com/microsoft-365/security/office-365-security/threat-explorer)na podatke o  &  [presudi Get-UrlTrace](https://docs.microsoft.com/powershell/module/exchange/get-urltrace)</span><span class="sxs-lookup"><span data-stu-id="b3738-117">track users who clicked and accessed malicious URLs: [View phishing URL and click verdict data](https://docs.microsoft.com/microsoft-365/security/office-365-security/threat-explorer) & [Get-UrlTrace](https://docs.microsoft.com/powershell/module/exchange/get-urltrace)</span></span>
    - <span data-ttu-id="b3738-118">ručno [pokretanje automatizirane pretrage](https://docs.microsoft.com/microsoft-365/security/office-365-security/automated-investigation-response-office)</span><span class="sxs-lookup"><span data-stu-id="b3738-118">manually [start an Automated Investigation](https://docs.microsoft.com/microsoft-365/security/office-365-security/automated-investigation-response-office)</span></span>

<span data-ttu-id="b3738-119">Možete i zaštititi od zlonamjernih datoteka i URL-ova slijedeći upute u aplikaciji [Zaštita od zlonamjernih URL-ova i datoteka](https://docs.microsoft.com/microsoft-365/security/office-365-security/protect-against-threats).</span><span class="sxs-lookup"><span data-stu-id="b3738-119">You can also protect against malicious files and URLs by following the instructions in [Protection from malicious URLs and files](https://docs.microsoft.com/microsoft-365/security/office-365-security/protect-against-threats).</span></span>