---
title: 2491 Upozorenje poruka e-pošte iz pravila "Krađa identiteta isporučena zbog nadjačavanja klijenta ili korisnika"
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 2e4efd504304da757687e697ff23374aeea31851
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43758900"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a><span data-ttu-id="a7e3c-102">Upozoravajte poruke e-pošte iz pravila "Krađa identiteta isporučena zbog nadjačavanja klijenta ili korisnika"</span><span class="sxs-lookup"><span data-stu-id="a7e3c-102">Alert email messages from the 'Phish Delivered due to tenant or user override' policy</span></span>

<span data-ttu-id="a7e3c-103">Zadano pravilo upozorenja pod nazivom "Krađa identiteta isporučena zbog nadjačavanja klijenta ili korisnika" uvedena je na klijentima s atp i P2 licencama za Office 365.</span><span class="sxs-lookup"><span data-stu-id="a7e3c-103">A default alert policy named "Phish Delivered due to tenant or user override" has been rolled out to tenants with Office 365 ATP P1 and P2 licenses.</span></span> <span data-ttu-id="a7e3c-104">Ako ste primili ovo upozorenje, evo koraka za istraživanje:</span><span class="sxs-lookup"><span data-stu-id="a7e3c-104">If you received this alert, here are the steps to investigate:</span></span>

1. <span data-ttu-id="a7e3c-105">U poruci upozorenja kliknite **Prikaz upozorenja** da biste otišli na stranicu **Upozorenja** u centru za & usklađenosti.</span><span class="sxs-lookup"><span data-stu-id="a7e3c-105">From the alert message, click **View Alert** to go to the **Alerts** page in the Security & Compliance Center.</span></span>

2. <span data-ttu-id="a7e3c-106">Odaberite upozorenje da biste vidjeli mogućnost **Prikaz popisa poruka** ili Prikaz poruka u **exploreru**.</span><span class="sxs-lookup"><span data-stu-id="a7e3c-106">Select the alert to see the option to **View message list** or **View messages in Explorer**.</span></span> <span data-ttu-id="a7e3c-107">Obje ove mogućnosti vode vas do pojedinosti poruke, što uključuje ID poruke.</span><span class="sxs-lookup"><span data-stu-id="a7e3c-107">Both of these options take you to the details of the message, which includes the Message ID.</span></span> <span data-ttu-id="a7e3c-108">Imajte na umu da će veza Threat Explorer automatski filtrirati poruke koje odgovaraju kriterijima upozorenja.</span><span class="sxs-lookup"><span data-stu-id="a7e3c-108">Note that the Threat Explorer link will automatically filter the messages that match the alert criteria.</span></span> <span data-ttu-id="a7e3c-109">Možda ćete morati prilagoditi filtar datuma u programu Threat Explorer.</span><span class="sxs-lookup"><span data-stu-id="a7e3c-109">You might need to adjust the date filter in Threat Explorer.</span></span>

<span data-ttu-id="a7e3c-110">Poruka o krađi identiteta isporučena je zbog ručno konfiguriranog nadjačavanja:</span><span class="sxs-lookup"><span data-stu-id="a7e3c-110">The phishing message was delivered because of a manually configured override:</span></span>

- <span data-ttu-id="a7e3c-111">Dopušteni pošiljatelj ili domena koje je postavio korisnik.</span><span class="sxs-lookup"><span data-stu-id="a7e3c-111">An allowed sender or domain set by the user.</span></span>

- <span data-ttu-id="a7e3c-112">Dopušteni pošiljatelj ili domena koje je administrator postavio u pravilima protiv neželjene pošte.</span><span class="sxs-lookup"><span data-stu-id="a7e3c-112">An allowed sender or domain set by the admin in an anti-spam policy.</span></span>

- <span data-ttu-id="a7e3c-113">Dopuštena IP adresa u pravilniku filtra veze.</span><span class="sxs-lookup"><span data-stu-id="a7e3c-113">An allowed IP address in a connection filter policy.</span></span>

- <span data-ttu-id="a7e3c-114">Pravilo tijeka pošte (poznato i kao pravilo prijenosa) konfigurirano tako da dopušta poruke.</span><span class="sxs-lookup"><span data-stu-id="a7e3c-114">A mail flow rule (also known as a transport rule) that's configured to allow messages in.</span></span>

<span data-ttu-id="a7e3c-115">Ako smatrate da je poruka pogrešno označena kao krađa identiteta, upotrijebite [dodatak Poruka izvješća programa](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) Outlook da biste microsoftu poslali uzorke poruka.</span><span class="sxs-lookup"><span data-stu-id="a7e3c-115">If you believe the message was incorrectly marked as phish, use the Outlook [Report Message add-in](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) to submit message samples to Microsoft.</span></span>
