---
title: Ikona kalendara ne prikazuje se u klijentu sustava Teams
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
- "9001219"
- "4375"
ms.openlocfilehash: 6a3f02b69d160c7dce68ed03df59c0d7d1f32f0f
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819945"
---
# <a name="calendar-icon-not-showing-in-teams-client"></a><span data-ttu-id="bde47-102">Ikona kalendara ne prikazuje se u klijentu sustava Teams</span><span class="sxs-lookup"><span data-stu-id="bde47-102">Calendar icon not showing in Teams client</span></span>

<span data-ttu-id="bde47-103">Kartica kalendar u sustavu Teams zahtijeva pristup poštanskom sandučiću sustava Exchange pomoću web-servisa sustava Exchange.</span><span class="sxs-lookup"><span data-stu-id="bde47-103">The Calendar Tab in Teams requires access to an Exchange mailbox via Exchange Web Services.</span></span> <span data-ttu-id="bde47-104">Poštanski sandučić sustava Exchange može biti mrežni ili lokalni.</span><span class="sxs-lookup"><span data-stu-id="bde47-104">The Exchange mailbox can be Online or On-Premises.</span></span> <span data-ttu-id="bde47-105">Za mrežne korisnike kojima se ne prikazuje kartica Kalendar provjerite jesu li [licencirani za poštanski sandučić sustava Exchange Online i je li poštanski sandučić omogućen](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).</span><span class="sxs-lookup"><span data-stu-id="bde47-105">For Online users who do not see the Calendar Tab, make sure they [are licensed for an Exchange Online mailbox and the mailbox is enabled](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).</span></span>

<span data-ttu-id="bde47-106">Ako korisnik ima valjani poštanski sandučić u sustavu Exchange Online, no i dalje ne može vidjeti karticu Kalendar, možda nailazite na problem s mrežom.</span><span class="sxs-lookup"><span data-stu-id="bde47-106">If the user has a valid mailbox in Exchange Online, but still cannot see the Calendar tab, you may be experiencing a network issue.</span></span> <span data-ttu-id="bde47-107">Koristite [Microsoftov analizator za daljinsko povezivanje](https://testconnectivity.microsoft.com/) i pokrenite **testiranja povezivanja sustava Microsoft Exchange Web Services** za zahvaćenog korisnika.</span><span class="sxs-lookup"><span data-stu-id="bde47-107">Use the [Microsoft Remote Connectivity Analyzer](https://testconnectivity.microsoft.com/) and run the **Microsoft Exchange Web Services Connectivity Tests** for the impacted user.</span></span>

<span data-ttu-id="bde47-108">Napokon provjerite aplikacije [Teams – pravilnike o postavljanju aplikacija](https://admin.teams.microsoft.com/policies/app-setup) da biste osigurali da aplikacija Kalendar nije uklonjena iz pravilnika koji je primijenjen na korisnika (najvjerojatnije **Global (zadano na razini tvrtke ili ustanove)**.</span><span class="sxs-lookup"><span data-stu-id="bde47-108">Finally check the [Teams Apps – App setup policies](https://admin.teams.microsoft.com/policies/app-setup) to ensure the Calendar app has not been removed from the policy applied to the user (most likely the **Global (Org-wide default)**.</span></span>

<span data-ttu-id="bde47-109">Ako su vaši korisnici lokalni, morate provjeriti je li vaša hibridna konfiguracija zdrava.</span><span class="sxs-lookup"><span data-stu-id="bde47-109">If your users are homed On-Premises, you need to confirm your Hybrid configuration is healthy.</span></span> <span data-ttu-id="bde47-110">Otklanjanje poteškoća pomoću [Čarobnjaka za hibridne konfiguracije](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent).</span><span class="sxs-lookup"><span data-stu-id="bde47-110">Use the [Hybrid Configuration Wizard](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) to troubleshoot.</span></span>

<span data-ttu-id="bde47-111">Imajte na umu da [sustav Teams zahtijeva Exchange 2016 CU3 ili napredniju verziju](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).</span><span class="sxs-lookup"><span data-stu-id="bde47-111">Note that [Teams requires Exchange 2016 CU3 or higher](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).</span></span>
