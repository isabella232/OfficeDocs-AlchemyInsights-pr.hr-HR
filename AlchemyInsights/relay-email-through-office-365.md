---
title: Razmjena e-pošte putem sustava Microsoft 365
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
- "154"
- "3000003"
ms.assetid: 84191e23-496c-495a-a2ec-28c5ae0d4c0b
ms.openlocfilehash: 56936541c52e56d7aa9b0f5dad7b9a359c5b6185
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51809647"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email"></a><span data-ttu-id="883f5-102">Postavljanje višefunkcijskog uređaja ili aplikacije za slanje e-pošte</span><span class="sxs-lookup"><span data-stu-id="883f5-102">Set up a multifunction device or application to send email</span></span>

<span data-ttu-id="883f5-103">Informacije o dostupnim mogućnostima i upute potražite u članku [Postavljanje višefunkcijskog uređaja ili aplikacije za slanje e-pošte pomoću sustava Microsoft 365](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).</span><span class="sxs-lookup"><span data-stu-id="883f5-103">To learn about your options and the steps, see [How to set up a multifunction device or application to send email using Microsoft 365](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).</span></span>
  
<span data-ttu-id="883f5-104">**Napomena:** ako imate uređaj ili aplikaciju koji su nedavno prestali funkcionirati, imajte na umu da smo nedavno počeli s [onemogućivanjem šifriranja 3DES](https://docs.microsoft.com/microsoft-365/compliance/technical-reference-details-about-encryption), kao što smo i planirali.</span><span class="sxs-lookup"><span data-stu-id="883f5-104">**Note:** If you have a device or application that recently stopped working, please note we have recently begun [disabling the 3DES cipher](https://docs.microsoft.com/microsoft-365/compliance/technical-reference-details-about-encryption) as planned.</span></span> <span data-ttu-id="883f5-105">Da biste vidjeli zahvaćene uređaje, idite na izvješće [Klijenti SMTP provjere autentičnosti](https://protection.office.com/mailflow/dashboard).</span><span class="sxs-lookup"><span data-stu-id="883f5-105">To see affected devices, go to the [SMTP Auth Clients report](https://protection.office.com/mailflow/dashboard).</span></span> <span data-ttu-id="883f5-106">Uobičajene pogreške mogu biti slične ovima: pogreška provjere autentičnosti, pogreška TLS-a, pogreška algoritma za šifriranje, nepodudarnost algoritama ili prekid veze.</span><span class="sxs-lookup"><span data-stu-id="883f5-106">Common errors could be similar to: Authentication failure/error, TLS failure/error, Cipher algorithm error, Algorithm mismatch, or Connection dropped.</span></span> <span data-ttu-id="883f5-107">Da biste riješili problem napravite sljedeće:</span><span class="sxs-lookup"><span data-stu-id="883f5-107">To resolve the issue:</span></span>

 - <span data-ttu-id="883f5-108">**Windows Server 2003 IIS SMTP više neće funkcionirati – trebate noviju verziju sustava Windows.**</span><span class="sxs-lookup"><span data-stu-id="883f5-108">**Windows Server 2003 IIS SMTP will no longer work – a newer version of Windows is required.**</span></span>  
 - <span data-ttu-id="883f5-109">Obratite se proizvođaču aplikacije ili uređaja da biste saznali podržava li moderno šifriranje i postoji li pripadno ažuriranje.</span><span class="sxs-lookup"><span data-stu-id="883f5-109">Please check with your application or device vendor to see if a modern cipher is supported or if there is an update.</span></span>
