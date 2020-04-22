---
title: Pogreška pri slanju e-pošte koju je blokirao SpamHaus
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 3ff4f7a155fe74f5b42a1bd43e67ef0a751d7fbd
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43714250"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a><span data-ttu-id="02033-102">Pogreška pri slanju e-pošte: Glavno računalo klijenta blokirano je pomoću usluge Spamhaus</span><span class="sxs-lookup"><span data-stu-id="02033-102">Error sending email: Client host blocked using Spamhaus</span></span>

<span data-ttu-id="02033-103">IP adresa koja je poslala poruku nalazi se na popisu blokova u vlasništvu [Spamhausa](https://go.microsoft.com/fwlink/p/?linkid=123245).</span><span class="sxs-lookup"><span data-stu-id="02033-103">The IP address that sent the message is on a block list owned by [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span></span> <span data-ttu-id="02033-104">Razlozi za blokiranje u spamhausu uključuju ugrožene račune, kompromitirane strojeve koji dijele javnu IP adresu i pravila davatelja internetskih usluga (ISP- a).</span><span class="sxs-lookup"><span data-stu-id="02033-104">Reasons for being blocked by Spamhaus include compromised accounts, compromised machines sharing a public IP address, and Internet Service Provider (ISP) policies.</span></span> <span data-ttu-id="02033-105">Mogući popravci su:</span><span class="sxs-lookup"><span data-stu-id="02033-105">Possible fixes are:</span></span>
  
- <span data-ttu-id="02033-106">Za blokirane dolazne poruke u kojima upravljate izvornim poslužiteljem e-pošte morate odrediti uzrok i ukloniti blok s web-mjesta Spamhaus.</span><span class="sxs-lookup"><span data-stu-id="02033-106">For blocked inbound messages where you control the source email server, you need to determine the cause and remove the block from the Spamhaus website.</span></span>

- <span data-ttu-id="02033-107">Za blokirane dolazne poruke gdje izvorNA IP adresa pripada nekome drugome, vlasnik adrese mora ukloniti blok s web-mjesta Spamhaus.</span><span class="sxs-lookup"><span data-stu-id="02033-107">For blocked inbound messages where the source IP address belongs to someone else, the address owner needs to remove the block from the Spamhaus website.</span></span> <span data-ttu-id="02033-108">Ako se IP adresa nalazi na popisu blokiranih pravila (PBL), vlasnik može dodijeliti drugu statičku IP adresu ili ukloniti adresu iz PBL-a.</span><span class="sxs-lookup"><span data-stu-id="02033-108">If the IP address is on the Policy Block List (PBL), the owner can assign a different static IP address or remove the address from the PBL.</span></span>

- <span data-ttu-id="02033-109">Za blokirane izlazne poruke s domene povezane s Microsoftom možete primiti ovu pogrešku ako se poruke usmjeravaju putem servisa treće strane.</span><span class="sxs-lookup"><span data-stu-id="02033-109">For blocked outbound messages from your domain connected to Microsoft, you can receive this error if the messages are routed through a 3rd party service.</span></span> <span data-ttu-id="02033-110">Pomoću whois alata za pretraživanje možete pronaći vlasnika blokirane IP adrese.</span><span class="sxs-lookup"><span data-stu-id="02033-110">You can use a WHOIS lookup tool to find the blocked IP address owner.</span></span>
