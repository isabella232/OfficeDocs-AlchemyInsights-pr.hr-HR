---
title: Problem s povezivanjem servisa AAD za zdravlje
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004649"
- "8427"
ms.openlocfilehash: f5624069a2e96fde8aed08965ca6b753f3aad1e8
ms.sourcegitcommit: 5763fedfd5dd459249c81cdbb4af34181a757bd5
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481152"
---
# <a name="problem-with-aad-connect-health"></a><span data-ttu-id="f7627-102">Problem s povezivanjem servisa AAD za zdravlje</span><span class="sxs-lookup"><span data-stu-id="f7627-102">Problem with AAD Connect Health</span></span>

- <span data-ttu-id="f7627-103">Provjerite jeste li ovlašteni za izvršavanje operacije.</span><span class="sxs-lookup"><span data-stu-id="f7627-103">Ensure you are authorized to perform the operation.</span></span> <span data-ttu-id="f7627-104">Globalni administratori imaju pristup prema zadanim postavkama.</span><span class="sxs-lookup"><span data-stu-id="f7627-104">Global Admins have access by default.</span></span> <span data-ttu-id="f7627-105">Uz to, pomoću [kontrole pristupa temeljene na ulogama](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) možete delegirati dozvolu za registraciju suradnika.</span><span class="sxs-lookup"><span data-stu-id="f7627-105">Additionally, you can use [Role Based Access Control](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) to delegate registration permission to Contributor.</span></span>
- <span data-ttu-id="f7627-106">Provjerite jesu li obavezne krajnje točke omogućene i nije li blokirana zbog vatrozida.</span><span class="sxs-lookup"><span data-stu-id="f7627-106">Ensure the required endpoints are enabled, and not blocked due to firewall.</span></span> <span data-ttu-id="f7627-107">Pojedinosti potražite u članku [Preduvjeti](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).</span><span class="sxs-lookup"><span data-stu-id="f7627-107">For details, see [requirements](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).</span></span>
- <span data-ttu-id="f7627-108">Registracija može propasti zbog odlazne komunikacije koja je izložena SSL inspekciji putem mrežnog sloja.</span><span class="sxs-lookup"><span data-stu-id="f7627-108">Registration can fail due to outbound communication being subjected to SSL inspection by the network layer.</span></span>
- <span data-ttu-id="f7627-109">Provjerite jeste li potvrdili postavke obavijesti o zdravlju za Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="f7627-109">Make sure you have verified the notification settings for Azure AD Connect Health.</span></span> <span data-ttu-id="f7627-110">Pregledajte postavku.</span><span class="sxs-lookup"><span data-stu-id="f7627-110">Please review your setting.</span></span> <span data-ttu-id="f7627-111">Ovaj [vodič](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) može vam pomoći da razumijete kako konfigurirati postavke obavijesti za obavijesti o zdravlju servisa Azure ad Connect.</span><span class="sxs-lookup"><span data-stu-id="f7627-111">This [guide](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) can help you understand how to configure the notification settings for Azure AD Connect health notifications.</span></span>
- <span data-ttu-id="f7627-112">Da biste saznali više o izvješću o sinkronizaciji programa AAD Connect i kako ga preuzeti, pročitajte članak [izvješće o sinkronizaciji razina objekta](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).</span><span class="sxs-lookup"><span data-stu-id="f7627-112">To learn more about the AAD Connect Health sync report and how to download it, see [Object level synchronization report](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).</span></span>

<span data-ttu-id="f7627-113">Da biste otklonili poteškoće s aplikacijom AAD Connect zdravstvene obavijesti, slijedite [upute za otklanjanje poteškoća za AAD povežite upozorenja o svježini podataka](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) i najčešća pitanja, pročitajte članak [zajednički AAD Connect pitanja o zdravstvenoj instalaciji](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).</span><span class="sxs-lookup"><span data-stu-id="f7627-113">To troubleshoot AAD Connect Health alerts, follow [the troubleshooting guide for AAD Connect Health data freshness alerts](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) and for commonly asked questions, see [Common AAD Connect Health installation questions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).</span></span>
