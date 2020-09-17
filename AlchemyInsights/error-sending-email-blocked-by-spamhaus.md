---
title: Pogreška prilikom slanja e-pošte koju je blokirao SpamHaus
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: a0c2f4be0b2d8ba6fd3dadbdf306e6ce623ad380
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47783795"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a><span data-ttu-id="ea7d1-102">Pogreška prilikom slanja e-pošte: klijentsko glavno računalo blokirano pomoću spamhaus</span><span class="sxs-lookup"><span data-stu-id="ea7d1-102">Error sending email: Client host blocked using Spamhaus</span></span>

<span data-ttu-id="ea7d1-103">IP adresa koja je poslala poruku nalazi se na popisu blokova u vlasništvu servisa [spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span><span class="sxs-lookup"><span data-stu-id="ea7d1-103">The IP address that sent the message is on a block list owned by [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span></span> <span data-ttu-id="ea7d1-104">Razlozi zbog kojih je spamhaus blokirao obuhvaćaju ugroћene račune, kompromitirani strojevi koji zajednički koriste javnu IP adresu i pravila davatelja internetskih usluga (ISP-a).</span><span class="sxs-lookup"><span data-stu-id="ea7d1-104">Reasons for being blocked by Spamhaus include compromised accounts, compromised machines sharing a public IP address, and Internet Service Provider (ISP) policies.</span></span> <span data-ttu-id="ea7d1-105">Mogući su popravci:</span><span class="sxs-lookup"><span data-stu-id="ea7d1-105">Possible fixes are:</span></span>
  
- <span data-ttu-id="ea7d1-106">Da biste blokirali ulazne poruke na kojima kontrolirate izvorni poslužitelj e-pošte, morate odrediti uzrok i ukloniti blok s web-mjesta spamhaus.</span><span class="sxs-lookup"><span data-stu-id="ea7d1-106">For blocked inbound messages where you control the source email server, you need to determine the cause and remove the block from the Spamhaus website.</span></span>

- <span data-ttu-id="ea7d1-107">Da biste blokirali ulazne poruke u kojima adresa izvornog IP-a pripada nekome drugome, vlasnik adrese mora ukloniti blok s web-mjesta spamhaus.</span><span class="sxs-lookup"><span data-stu-id="ea7d1-107">For blocked inbound messages where the source IP address belongs to someone else, the address owner needs to remove the block from the Spamhaus website.</span></span> <span data-ttu-id="ea7d1-108">Ako je IP adresa na popisu poljski blok (PBL), vlasnik može dodijeliti neku drugu statičnu IP adresu ili ukloniti adresu iz PBL-a.</span><span class="sxs-lookup"><span data-stu-id="ea7d1-108">If the IP address is on the Policy Block List (PBL), the owner can assign a different static IP address or remove the address from the PBL.</span></span>

- <span data-ttu-id="ea7d1-109">Ako ste blokirali odlazne poruke iz domene povezane s Microsoftom, možete primiti ovu pogrešku ako su poruke preusmjerene putem servisa trećih strana.</span><span class="sxs-lookup"><span data-stu-id="ea7d1-109">For blocked outbound messages from your domain connected to Microsoft, you can receive this error if the messages are routed through a 3rd party service.</span></span> <span data-ttu-id="ea7d1-110">Možete koristiti alat za traženje funkcije WHOIS da biste pronašli vlasnika blokiranih IP adresa.</span><span class="sxs-lookup"><span data-stu-id="ea7d1-110">You can use a WHOIS lookup tool to find the blocked IP address owner.</span></span>
