---
title: Postavljanje preglednika Microsoft Edge kao zadanog preglednika na uređaju sa sustavom macOS
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10362"
- "9006005"
ms.openlocfilehash: 5318c7d20ee7091e162e566cd2b4ebf5d255915b
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/30/2021
ms.locfileid: "51491360"
---
# <a name="set-microsoft-edge-as-the-default-browser-on-a-macos-device"></a><span data-ttu-id="63fb5-102">Postavljanje preglednika Microsoft Edge kao zadanog preglednika na uređaju sa sustavom macOS</span><span class="sxs-lookup"><span data-stu-id="63fb5-102">Set Microsoft Edge as the default browser on a macOS device</span></span>

<span data-ttu-id="63fb5-103">Pomoću jedne od ova dva načina postavite Microsoft Edge kao zadani preglednik:</span><span class="sxs-lookup"><span data-stu-id="63fb5-103">Use one of these two methods to set Microsoft Edge as the default browser:</span></span>

<span data-ttu-id="63fb5-104">Prvi način: flash uređaj sa slikom sustava macOS na kojoj je Microsoft Edge već postavljen kao zadani preglednik.</span><span class="sxs-lookup"><span data-stu-id="63fb5-104">Method 1: Flash the device with an image of macOS where Microsoft Edge has already been set as the default browser.</span></span>

<span data-ttu-id="63fb5-105">Drugi način: postavite pravilnik DefaultBrowserSettingEnabled tako da od korisnika zatraži postavljanje preglednika Microsoft Edge kao zadanog preglednika.</span><span class="sxs-lookup"><span data-stu-id="63fb5-105">Method 2: Set the DefaultBrowserSettingEnabled policy to prompt the user to set Microsoft Edge as the default browser.</span></span>

<span data-ttu-id="63fb5-106">Oba načina korisniku omogućuju promjenu zadanog preglednika.</span><span class="sxs-lookup"><span data-stu-id="63fb5-106">Either method allows a user to change the default browser.</span></span> <span data-ttu-id="63fb5-107">Zato preporučujemo implementaciju pravilnika DefaultBrowserSettingEnabled čak i ako ste koristili 1. metodu.</span><span class="sxs-lookup"><span data-stu-id="63fb5-107">For this reason, we recommend that you deploy the DefaultBrowserSettingEnabled policy even if you used method 1.</span></span> <span data-ttu-id="63fb5-108">Ako korisnik promijeni zadani preglednik nakon primjene pravilnika, pravilnik će od korisnika zatražiti da vrati zadani preglednik na Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="63fb5-108">If a user changes the default browser after the policy is deployed, the policy prompts the user to set the default browser back to Microsoft Edge.</span></span>
