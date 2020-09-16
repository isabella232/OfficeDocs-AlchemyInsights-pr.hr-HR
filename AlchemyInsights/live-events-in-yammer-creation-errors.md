---
title: Pogreške stvaranja događaja uživo na servisu Yammer
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002495"
- "5112"
ms.openlocfilehash: 1b342b17e4b91804a75c46352f3ef7d7814bfcee
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47675434"
---
# <a name="live-events-in-yammer-creation-errors"></a><span data-ttu-id="973f5-102">Pogreške stvaranja događaja uživo na servisu Yammer</span><span class="sxs-lookup"><span data-stu-id="973f5-102">Live events in Yammer creation errors</span></span>

<span data-ttu-id="973f5-103">**Stvaranje događaja uživo na servisu Yammer**</span><span class="sxs-lookup"><span data-stu-id="973f5-103">**Yammer Live Event creation**</span></span>

<span data-ttu-id="973f5-104">U svakom će trenutku Yammer prikazati mogućnost stvaranja događaja uživo.</span><span class="sxs-lookup"><span data-stu-id="973f5-104">Yammer will show the option to create a live event at all times.</span></span> <span data-ttu-id="973f5-105">U nekim slučajevima korisnik možda neće ispuniti preduvjete za stvaranje događaja uživo i primit će pogrešku kada ga pokuša stvoriti.</span><span class="sxs-lookup"><span data-stu-id="973f5-105">In some cases, a user may not meet the prerequisites for creating a live event and receive an error when they attempt to create it.</span></span> <span data-ttu-id="973f5-106">U stavkama u nastavku nalaze se česti razlozi ovog problema te načini kako ga riješiti za krajnje korisnike.</span><span class="sxs-lookup"><span data-stu-id="973f5-106">The items below cover common reasons for this problem and provide ways to resolve it for end users.</span></span>

<span data-ttu-id="973f5-107">**Tko može stvarati događaje uživo**</span><span class="sxs-lookup"><span data-stu-id="973f5-107">**Who can create live events**</span></span>
- <span data-ttu-id="973f5-108">Licenca za Office 365 Enterprise E1, E3 ili E5 ili licenca za Office 365 A3 ili A5.</span><span class="sxs-lookup"><span data-stu-id="973f5-108">An Office 365 Enterprise E1, E3, or E5 license or an Office 365 A3 or A5 license.</span></span>
- <span data-ttu-id="973f5-109">Dozvola za stvaranje događaja uživo u centru za administratore aplikacije Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="973f5-109">Permission to create live events in Microsoft Teams admin center.</span></span>
- <span data-ttu-id="973f5-110">Dozvola za stvaranje događaja uživo u servisu Microsoft Stream (za događaje stvorene s pomoću vanjske aplikacije ili uređaja za emitiranje).</span><span class="sxs-lookup"><span data-stu-id="973f5-110">Permission to create live events in Microsoft Stream (for events produced using an external broadcasting app or device).</span></span>
- <span data-ttu-id="973f5-111">Puno timsko članstvo u tvrtki ili ustanovi (korisnik ne može biti gost niti dolaziti iz druge tvrtke ili ustanove).</span><span class="sxs-lookup"><span data-stu-id="973f5-111">Full team membership in the org (can’t be a guest or from another org).</span></span>
- <span data-ttu-id="973f5-112">Zakazivanje privatnih sastanaka, dijeljenje zaslona i IP dijeljenje videozapisa, uključeni u pravilniku za sastanke aplikacije Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="973f5-112">Private meeting scheduling, screensharing, and IP video sharing, turned on in Team meeting policy.</span></span>

<span data-ttu-id="973f5-113">**Pravilnici o stvaranju događaja uživo**</span><span class="sxs-lookup"><span data-stu-id="973f5-113">**Live event creation policies**</span></span>

<span data-ttu-id="973f5-114">Yammer slijedi pravilnike o događajima uživo koji su postavljeni u klijentu sustava Office 365 za Microsoft Stream.</span><span class="sxs-lookup"><span data-stu-id="973f5-114">Yammer follows the Live Event policies set in your Office 365 tenant for Stream.</span></span> <span data-ttu-id="973f5-115">Svatko u vašoj tvrtki ili ustanovi može po zadanom stvoriti događaj uživo.</span><span class="sxs-lookup"><span data-stu-id="973f5-115">By default, everyone in your organization can create a live event.</span></span> <span data-ttu-id="973f5-116">Administratori mogu [mijenjati tu postavku, što može onemogućiti korisnicima stvaranja događaja uživo](https://docs.microsoft.com/stream/live-event-administration#enabling-and-restricting-users-to-creating).</span><span class="sxs-lookup"><span data-stu-id="973f5-116">Administrators may [make changes to this setting which may prevent users from creating a live event](https://docs.microsoft.com/stream/live-event-administration#enabling-and-restricting-users-to-creating).</span></span> <span data-ttu-id="973f5-117">Važno je provjeriti imaju li korisnici dozvole za stvaranje događaja uživo ako dobiju pogrešku pravilnika.</span><span class="sxs-lookup"><span data-stu-id="973f5-117">It is important to check that users have permissions to create live events if they receive a policy error.</span></span>
