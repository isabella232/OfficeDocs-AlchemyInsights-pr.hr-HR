---
title: Došlo je do pogreške prilikom provjere pogrešaka programa Access token tijekom radne površine u analitici na dasci
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2536"
- "9000657"
ms.openlocfilehash: 45c6fb1a1632799a07c028c0791b6b8e77635293
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47783543"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a><span data-ttu-id="3bade-102">"Došlo je do pogreške pri provjeri valjanosti programa Access token" prilikom korištenja analitičkih podataka za stolna računala</span><span class="sxs-lookup"><span data-stu-id="3bade-102">"There was an error validating access token" error during Desktop Analytics onboarding</span></span>

<span data-ttu-id="3bade-103">Ta se pogreška obično primjećuje kada istekne token za provjeru autentičnosti.</span><span class="sxs-lookup"><span data-stu-id="3bade-103">This error is normally observed when the authentication token expires.</span></span> <span data-ttu-id="3bade-104">Obično osvježavanjem stranice osvježava token.</span><span class="sxs-lookup"><span data-stu-id="3bade-104">Usually, refreshing the page refreshes the token.</span></span> <span data-ttu-id="3bade-105">Međutim, taj problem može biti ustrajan ako postoje pravila uvjetnog pristupa koja se primjenjuju na račun koji se koristi za analitičke radne površine.</span><span class="sxs-lookup"><span data-stu-id="3bade-105">However, this issue can persist if there are any Conditional Access policies applied to the account being used to on-board Desktop Analytics.</span></span> <span data-ttu-id="3bade-106">Prijavite se u zapisnicima za Azure AD na portalu Azure da biste vidjeli postoje li neuspjele prijave za račun koji se koristi za analitiku za stolna računala.</span><span class="sxs-lookup"><span data-stu-id="3bade-106">You can review the Azure AD Sign In logs in the Azure Portal to see if there are any sign-in failures for the account being used for Desktop Analytics onboarding.</span></span>

<span data-ttu-id="3bade-107">Dodatne informacije o uvjetnom pristupu potražite u odjeljku [Planiranje implementacije uvjetnog pristupanja](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).</span><span class="sxs-lookup"><span data-stu-id="3bade-107">For more information about Conditional Access, visit [Plan your Conditional Access deployment](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).</span></span>