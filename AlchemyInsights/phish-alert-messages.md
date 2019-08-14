---
title: Poruka upozorenja e-pošte 2491 iz pravila Phish isporučiti klijentske ili korisnik nadjačati
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 456b186ecea59422c791c79d4df056ad8446bc70
ms.sourcegitcommit: 7c90dcc570d32ebd968e3e4e816a7b482890b3a4
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36391164"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a><span data-ttu-id="7043d-102">Poruka upozorenja e-pošte iz pravila Phish isporučiti klijentske ili korisnik nadjačati</span><span class="sxs-lookup"><span data-stu-id="7043d-102">Alert email messages from the 'Phish Delivered due to tenant or user override' policy</span></span>

<span data-ttu-id="7043d-103">Zadano upozorenja pravilo pod nazivom "Phish Delivered zbog nadjačavanje korisnika ili klijentske" ima je poslednjeg samoposlužni s Office 365 ATP P1 i P2 licence.</span><span class="sxs-lookup"><span data-stu-id="7043d-103">A default alert policy named "Phish Delivered due to tenant or user override" has been rolled out to tenants with Office 365 ATP P1 and P2 licenses.</span></span> <span data-ttu-id="7043d-104">Ako ste primili ovo upozorenje, ovdje se istražiti koraka:</span><span class="sxs-lookup"><span data-stu-id="7043d-104">If you received this alert, here are the steps to investigate:</span></span>

1. <span data-ttu-id="7043d-105">Iz poruke upozorenja kliknite **Prikaz upozorenja** da biste otišli na stranicu **upozorenja** u & usklađenosti centar sigurnosti.</span><span class="sxs-lookup"><span data-stu-id="7043d-105">From the alert message, click **View Alert** to go to the **Alerts** page in the Security & Compliance Center.</span></span>

2. <span data-ttu-id="7043d-106">Odaberite upozorenje da biste vidjeli mogućnost za **Prikaz popisa poruka** ili **Prikaz poruka u programu Explorer**.</span><span class="sxs-lookup"><span data-stu-id="7043d-106">Select the alert to see the option to **View message list** or **View messages in Explorer**.</span></span> <span data-ttu-id="7043d-107">Obje ove opcije poduzeti za pojedinosti poruke uključuje ID poruke.</span><span class="sxs-lookup"><span data-stu-id="7043d-107">Both of these options take you to the details of the message, which includes the Message ID.</span></span> <span data-ttu-id="7043d-108">Imajte na umu vezu prijetnja Explorer automatski filtrirali poruke koje zadovoljavaju kriterije upozorenja.</span><span class="sxs-lookup"><span data-stu-id="7043d-108">Note that the Threat Explorer link will automatically filter the messages that match the alert criteria.</span></span> <span data-ttu-id="7043d-109">Možda ćete morati prilagoditi filtar datuma u programu Explorer prijetnja.</span><span class="sxs-lookup"><span data-stu-id="7043d-109">You might need to adjust the date filter in Threat Explorer.</span></span>

<span data-ttu-id="7043d-110">Phishing poruka isporučena zbog ručno konfiguriran nadjačavanje:</span><span class="sxs-lookup"><span data-stu-id="7043d-110">The phishing message was delivered because of a manually configured override:</span></span>

- <span data-ttu-id="7043d-111">Dopuštenih pošiljatelja ili domene postavio korisnik.</span><span class="sxs-lookup"><span data-stu-id="7043d-111">An allowed sender or domain set by the user.</span></span>

- <span data-ttu-id="7043d-112">Dopuštenih pošiljatelja ili domene postavio admin pravila protiv neželjene pošte.</span><span class="sxs-lookup"><span data-stu-id="7043d-112">An allowed sender or domain set by the admin in an anti-spam policy.</span></span>

- <span data-ttu-id="7043d-113">Dopuštenih IP adresu u pravilima filtar veze.</span><span class="sxs-lookup"><span data-stu-id="7043d-113">An allowed IP address in a connection filter policy.</span></span>

- <span data-ttu-id="7043d-114">Mail protok pravilo (poznate i kao pravilo prijevoza) koja je konfigurirana za dopuštanje poruka u.</span><span class="sxs-lookup"><span data-stu-id="7043d-114">A mail flow rule (also known as a transport rule) that's configured to allow messages in.</span></span>

<span data-ttu-id="7043d-115">Ako mislite da poruka pogrešno označena kao phish, koristite u Outlook [poruka izvještaja dodatak](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) slanje uzoraka poruku tvrtki Microsoft.</span><span class="sxs-lookup"><span data-stu-id="7043d-115">If you believe the message was incorrectly marked as phish, use the Outlook [Report Message add-in](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) to submit message samples to Microsoft.</span></span>
