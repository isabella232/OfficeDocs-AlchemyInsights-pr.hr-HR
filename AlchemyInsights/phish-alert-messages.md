---
title: 2491 upozorite poruke e-pošte iz ' Phish isporučen zbog klijenta ili korisnici nadjačati ' pravilnik
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 5b5faa08542cb5878107f10afb34427f636562ac
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47728603"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a><span data-ttu-id="4b1b0-102">Upozorite poruke e-pošte s servisa ' Phish isporučen zbog korisnika ili pravila nadjačavanja klijenta</span><span class="sxs-lookup"><span data-stu-id="4b1b0-102">Alert email messages from the 'Phish Delivered due to tenant or user override' policy</span></span>

<span data-ttu-id="4b1b0-103">Zadana pravila upozorenja koja se naziva "Phish isporučen zbog korisnika ili nadjačavanja klijenta" odkotrljali su se stanarima sa sustavom Office 365 ATP P1 i P2 licenci.</span><span class="sxs-lookup"><span data-stu-id="4b1b0-103">A default alert policy named "Phish Delivered due to tenant or user override" has been rolled out to tenants with Office 365 ATP P1 and P2 licenses.</span></span> <span data-ttu-id="4b1b0-104">Ako ste primili ovo upozorenje, slijedite upute za istragu:</span><span class="sxs-lookup"><span data-stu-id="4b1b0-104">If you received this alert, here are the steps to investigate:</span></span>

1. <span data-ttu-id="4b1b0-105">U poruci upozorenja kliknite **Prikaži upozorenje** da biste prešli na stranicu s **upozorenjima** u centru za sigurnost & usklađenosti.</span><span class="sxs-lookup"><span data-stu-id="4b1b0-105">From the alert message, click **View Alert** to go to the **Alerts** page in the Security & Compliance Center.</span></span>

2. <span data-ttu-id="4b1b0-106">Odaberite upozorenje da biste vidjeli mogućnost **prikaza popisa poruka** ili **Prikaz poruka u programu Explorer**.</span><span class="sxs-lookup"><span data-stu-id="4b1b0-106">Select the alert to see the option to **View message list** or **View messages in Explorer**.</span></span> <span data-ttu-id="4b1b0-107">Obje te mogućnosti odvesti će vas do pojedinosti poruke, koja sadrži ID poruke.</span><span class="sxs-lookup"><span data-stu-id="4b1b0-107">Both of these options take you to the details of the message, which includes the Message ID.</span></span> <span data-ttu-id="4b1b0-108">Imajte na čemu da će veza eksplorera za prijetnje automatski filtrirati poruke koje odgovaraju kriterijima upozorenja.</span><span class="sxs-lookup"><span data-stu-id="4b1b0-108">Note that the Threat Explorer link will automatically filter the messages that match the alert criteria.</span></span> <span data-ttu-id="4b1b0-109">Možda ćete morati prilagoditi filtar datuma u eksploreru za prijetnje.</span><span class="sxs-lookup"><span data-stu-id="4b1b0-109">You might need to adjust the date filter in Threat Explorer.</span></span>

<span data-ttu-id="4b1b0-110">Poruka o krađi identiteta isporučena je zbog ručnog konfiguriranog premošćivanja:</span><span class="sxs-lookup"><span data-stu-id="4b1b0-110">The phishing message was delivered because of a manually configured override:</span></span>

- <span data-ttu-id="4b1b0-111">Dopušteni pošiljatelj ili domena koje je postavio korisnik.</span><span class="sxs-lookup"><span data-stu-id="4b1b0-111">An allowed sender or domain set by the user.</span></span>

- <span data-ttu-id="4b1b0-112">Dopušteni pošiljatelj ili domena koje je administrator postavio u pravilnik o suzbijanju neželjene pošte.</span><span class="sxs-lookup"><span data-stu-id="4b1b0-112">An allowed sender or domain set by the admin in an anti-spam policy.</span></span>

- <span data-ttu-id="4b1b0-113">Dopuštena IP adresa u pravilima filtra veze.</span><span class="sxs-lookup"><span data-stu-id="4b1b0-113">An allowed IP address in a connection filter policy.</span></span>

- <span data-ttu-id="4b1b0-114">Pravilo protoka pošte (poznato i kao pravilo prijenosa) koje je konfigurirano tako da dopušta poruke u programu.</span><span class="sxs-lookup"><span data-stu-id="4b1b0-114">A mail flow rule (also known as a transport rule) that's configured to allow messages in.</span></span>

<span data-ttu-id="4b1b0-115">Ako smatrate da je poruka neispravno označena kao Phish, upotrijebite [dodatak za poruke](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) programa Outlook da biste Microsoftu poslali uzorke poruka.</span><span class="sxs-lookup"><span data-stu-id="4b1b0-115">If you believe the message was incorrectly marked as phish, use the Outlook [Report Message add-in](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) to submit message samples to Microsoft.</span></span>
