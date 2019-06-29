---
title: Pogreška slanja e-pošte blokiran SpamHaus
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 2/23/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 52a5c20d59a2eac4c4bf465edaa888952d47f39f
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/28/2019
ms.locfileid: "35387841"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a><span data-ttu-id="9e6cc-102">Pogreška slanja e-pošte: klijent domaćin blokirane pomoću Spamhaus</span><span class="sxs-lookup"><span data-stu-id="9e6cc-102">Error sending email: Client host blocked using Spamhaus</span></span>

<span data-ttu-id="9e6cc-103">IP adresu slanja poruke je na popisu blok vlasništvu [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span><span class="sxs-lookup"><span data-stu-id="9e6cc-103">The IP address that sent the message is on a block list owned by [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span></span> <span data-ttu-id="9e6cc-104">Za blokira Spamhaus razlozi ugrožena račune ugrožena strojeva zajedničko korištenje javne IP adresa i pravila davatelj internetskih usluga (ISP).</span><span class="sxs-lookup"><span data-stu-id="9e6cc-104">Reasons for being blocked by Spamhaus include compromised accounts, compromised machines sharing a public IP address, and Internet Service Provider (ISP) policies.</span></span> <span data-ttu-id="9e6cc-105">Mogući popravke su:</span><span class="sxs-lookup"><span data-stu-id="9e6cc-105">Possible fixes are:</span></span>
  
- <span data-ttu-id="9e6cc-106">Blokirani ulaznih poruka za Office 365 gdje kontrolu izvorni poslužitelj e-pošte, morate odrediti uzrok i uklonite bloka s Spamhaus web-mjesta.</span><span class="sxs-lookup"><span data-stu-id="9e6cc-106">For blocked inbound messages to Office 365 where you control the source email server, you need to determine the cause and remove the block from the Spamhaus website.</span></span>

- <span data-ttu-id="9e6cc-107">Blokirani ulaznih poruka za Office 365 gdje IP adresu izvora pripada nekom drugom, vlasnik adresa mora ukloniti bloka s Spamhaus web-mjesta.</span><span class="sxs-lookup"><span data-stu-id="9e6cc-107">For blocked inbound messages to Office 365 where the source IP address belongs to someone else, the address owner needs to remove the block from the Spamhaus website.</span></span> <span data-ttu-id="9e6cc-108">Ako je IP adresa na na pravila blok popisa (PBL), vlasnik možete dodijeliti različite statička IP adresa ili uklanjanje adresu u PBL.</span><span class="sxs-lookup"><span data-stu-id="9e6cc-108">If the IP address is on the Policy Block List (PBL), the owner can assign a different static IP address or remove the address from the PBL.</span></span>

- <span data-ttu-id="9e6cc-109">Za blokirane izlaznog poruke iz domenu Office 365, možete primati ovu pogrešku ako poruke usmjeravaju kroz 3 servis proizvođača.</span><span class="sxs-lookup"><span data-stu-id="9e6cc-109">For blocked outbound messages from your Office 365 domain, you can receive this error if the messages are routed through a 3rd party service.</span></span> <span data-ttu-id="9e6cc-110">Alat za pronalaženje WHOIS možete koristiti za pronalaženje blokirani vlasnik IP adresu.</span><span class="sxs-lookup"><span data-stu-id="9e6cc-110">You can use a WHOIS lookup tool to find the blocked IP address owner.</span></span>
