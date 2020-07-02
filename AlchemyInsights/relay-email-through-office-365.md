---
title: Razmjena e-pošte putem sustava Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "154"
- "3000003"
ms.assetid: 84191e23-496c-495a-a2ec-28c5ae0d4c0b
ms.openlocfilehash: 074a9106553bf3a2a5e563f9ebaca9dfc38111cb
ms.sourcegitcommit: 9872280f71429d2344b0b441e218fba5b3bd3cf7
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 07/02/2020
ms.locfileid: "45023451"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email"></a><span data-ttu-id="eb07d-102">Postavljanje višefunkcijskog uređaja ili aplikacije za slanje e-pošte</span><span class="sxs-lookup"><span data-stu-id="eb07d-102">Set up a multifunction device or application to send email</span></span>

<span data-ttu-id="eb07d-103">Informacije o dostupnim mogućnostima i upute potražite u članku [Postavljanje višefunkcijskog uređaja ili aplikacije za slanje e-pošte pomoću sustava Microsoft 365](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).</span><span class="sxs-lookup"><span data-stu-id="eb07d-103">To learn about your options and the steps, see [How to set up a multifunction device or application to send email using Microsoft 365](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).</span></span>
  
<span data-ttu-id="eb07d-104">**Napomena:** ako imate uređaj ili aplikaciju koji su nedavno prestali funkcionirati, imajte na umu da smo nedavno počeli s [onemogućivanjem šifriranja 3DES](https://docs.microsoft.com/microsoft-365/compliance/technical-reference-details-about-encryption), kao što smo i planirali.</span><span class="sxs-lookup"><span data-stu-id="eb07d-104">**Note:** If you have a device or application that recently stopped working, please note we have recently begun [disabling the 3DES cipher](https://docs.microsoft.com/microsoft-365/compliance/technical-reference-details-about-encryption) as planned.</span></span> <span data-ttu-id="eb07d-105">Da biste vidjeli zahvaćene uređaje, idite na izvješće [Klijenti SMTP provjere autentičnosti](https://protection.office.com/mailflow/dashboard).</span><span class="sxs-lookup"><span data-stu-id="eb07d-105">To see affected devices, go to the [SMTP Auth Clients report](https://protection.office.com/mailflow/dashboard).</span></span> <span data-ttu-id="eb07d-106">Uobičajene pogreške mogu biti slične ovima: pogreška provjere autentičnosti, pogreška TLS-a, pogreška algoritma za šifriranje, nepodudarnost algoritama ili prekid veze.</span><span class="sxs-lookup"><span data-stu-id="eb07d-106">Common errors could be similar to: Authentication failure/error, TLS failure/error, Cipher algorithm error, Algorithm mismatch, or Connection dropped.</span></span> <span data-ttu-id="eb07d-107">Da biste riješili problem napravite sljedeće:</span><span class="sxs-lookup"><span data-stu-id="eb07d-107">To resolve the issue:</span></span>

 - <span data-ttu-id="eb07d-108">**Windows Server 2003 IIS SMTP više neće funkcionirati – trebate noviju verziju sustava Windows.**</span><span class="sxs-lookup"><span data-stu-id="eb07d-108">**Windows Server 2003 IIS SMTP will no longer work – a newer version of Windows is required.**</span></span>  
 - <span data-ttu-id="eb07d-109">Obratite se proizvođaču aplikacije ili uređaja da biste saznali podržava li moderno šifriranje i postoji li pripadno ažuriranje.</span><span class="sxs-lookup"><span data-stu-id="eb07d-109">Please check with your application or device vendor to see if a modern cipher is supported or if there is an update.</span></span>
