---
title: 1332 OWA - Primljeno pravila se ne izvršava za poštanski sandučić
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1332
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: c0b221b5335254bd0f1eb4b258efa6946376ca12
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32372552"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a><span data-ttu-id="598da-102">Pravilo ulazne pošte ne funkcionira prema očekivanjima</span><span class="sxs-lookup"><span data-stu-id="598da-102">An Inbox rule doesn't work as expected</span></span>

<span data-ttu-id="598da-103">Provjerite sljedeće postavke:</span><span class="sxs-lookup"><span data-stu-id="598da-103">Verify the following settings:</span></span>

- <span data-ttu-id="598da-104">Poruku možete biti preusmjereni proslijeđene ili odgovorene automatski na temelju pravila ulazne pošte samo jednom.</span><span class="sxs-lookup"><span data-stu-id="598da-104">A message can be redirected, forwarded, or replied to automatically based on Inbox rules only one time.</span></span> <span data-ttu-id="598da-105">Preusmjeravanje pravilo (pravilo ulazne pošte ili pošte protok pravilo, poznat i kao pravilo prijevoza) možete dodati najviše deset prosljeđivanje primatelji poruke.</span><span class="sxs-lookup"><span data-stu-id="598da-105">A redirecting rule (an Inbox rule or mail flow rule, also known as a transport rule) can add a maximum of ten forwarding recipients to a message.</span></span> <span data-ttu-id="598da-106">Za dodatne informacije pogledajte [temeljnice, prijevoza, i Primljeno pravilo ograničenja](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span><span class="sxs-lookup"><span data-stu-id="598da-106">For more information, see [Journal, Transport, and Inbox rule limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span></span>

- <span data-ttu-id="598da-107">Pravila ulazne pošte ne rade na zamjenski journaling poštanski sandučić.</span><span class="sxs-lookup"><span data-stu-id="598da-107">Inbox rules don't work on the alternate journaling mailbox.</span></span> <span data-ttu-id="598da-108">Dodatne informacije o journaling Alternativni poštanski sandučić pogledajte [Alternativni journaling poštanski sandučić](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span><span class="sxs-lookup"><span data-stu-id="598da-108">For more information about the alternate journaling mailbox, see [Alternate journaling mailbox](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span></span>

<span data-ttu-id="598da-109">Da biste riješili te probleme, pogledajte [KB 2829319](https://support.microsoft.com/kb/2829319).</span><span class="sxs-lookup"><span data-stu-id="598da-109">To fix these issues, see [KB 2829319](https://support.microsoft.com/kb/2829319).</span></span>

<span data-ttu-id="598da-110">Ako ne primijenite prethodne problemi, pokrenite dijagnostičkog izvješća pravilo Primljeno prije Eskaliranje problem Microsoft Support:</span><span class="sxs-lookup"><span data-stu-id="598da-110">If the previous issues don't apply, run the Inbox rule diagnostic report before you escalate the issue to Microsoft Support:</span></span>

1. <span data-ttu-id="598da-111">Otvoriti poštanski sandučić u programu Outlook na webu i kliknite **Postavke** \> **Mogućnosti** \> **e-pošta organiziraj** \> **pravila ulazne pošte**.</span><span class="sxs-lookup"><span data-stu-id="598da-111">Open the mailbox in Outlook on the web, and click **Settings** \> **Options** \> **Organize email** \> **Inbox rules**.</span></span>

2. <span data-ttu-id="598da-112">Na dnu stranice kliknite **Ako vaša pravila ne rade pritisnite ovdje za generiranje dijagnostičkog izvješća**.</span><span class="sxs-lookup"><span data-stu-id="598da-112">At the bottom of the page, click **If your rules are not working click here to generate a diagnostic report**.</span></span>
