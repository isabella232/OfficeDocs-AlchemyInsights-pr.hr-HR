---
title: Problemi u razvoju aplikacija
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7754"
- "9004342"
ms.openlocfilehash: 652fd6431201380e8e96619f63ecac15a6704d4f
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974230"
---
# <a name="issues-developing-applications"></a><span data-ttu-id="1c564-102">Problemi u razvoju aplikacija</span><span class="sxs-lookup"><span data-stu-id="1c564-102">Issues developing applications</span></span>

<span data-ttu-id="1c564-103">Da biste otklonili poteškoće s najčešćih problema prilikom izgradnje aplikacija Azure Active Directory (AD), pročitajte sljedeće članke:</span><span class="sxs-lookup"><span data-stu-id="1c564-103">To troubleshoot the most common problems when building Azure Active Directory (AD) apps, see the following articles:</span></span>

- [<span data-ttu-id="1c564-104">Vidim poteškoće prilikom prijave u aplikacije pomoću preglednika Chrome</span><span class="sxs-lookup"><span data-stu-id="1c564-104">I am seeing trouble signing in to application(s) using Chrome browser only</span></span>](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications) 
- [<span data-ttu-id="1c564-105">Ne znam kako promijeniti zadane vrijednosti trajanja tokena za moju aplikaciju</span><span class="sxs-lookup"><span data-stu-id="1c564-105">I don't know how to change the token lifetime defaults for my application</span></span>](https://docs.microsoft.com/azure/active-directory/develop/registration-config-change-token-lifetime-how-to) 
- [<span data-ttu-id="1c564-106">Zbunjen sam o tome kako funkcionira suglasnost aplikacija</span><span class="sxs-lookup"><span data-stu-id="1c564-106">I am confused about how application consent works</span></span>](https://docs.microsoft.com/azure/active-directory/application-dev-consent-framework) 
- [<span data-ttu-id="1c564-107">Ne znam kako dodijeliti dozvole za svoju aplikaciju</span><span class="sxs-lookup"><span data-stu-id="1c564-107">I don't know how to grant permissions to my application</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent) 
- [<span data-ttu-id="1c564-108">Ne razumijem razliku između dozvola delegiranih i aplikacija</span><span class="sxs-lookup"><span data-stu-id="1c564-108">I don't understand the difference between delegated and application permissions</span></span>](https://docs.microsoft.com/azure/active-directory/develop/delegated-and-app-perms)

<span data-ttu-id="1c564-109">\***Kraj podrške za Azure Active Directory za biblioteku autentičnosti (ADAL) i Azure ad Graph API (AAD Graph)** _</span><span class="sxs-lookup"><span data-stu-id="1c564-109">\***End of support for Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph)** _</span></span>

- <span data-ttu-id="1c564-110">Počevši od 30 Lipanj, 2020, više nećemo dodavati nove značajke u biblioteku servisa Azure Active Directory za provjeru autentičnosti (ADAL) i API-ja za Azure AD Graph (AAD Graph).</span><span class="sxs-lookup"><span data-stu-id="1c564-110">Starting June 30th, 2020, we will no longer add any new features to Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph).</span></span> <span data-ttu-id="1c564-111">Nastavit ćemo pružati tehničku podršku i sigurnosno ažuriranje, ali više nećemo pružati ažuriranja značajki.</span><span class="sxs-lookup"><span data-stu-id="1c564-111">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>

- <span data-ttu-id="1c564-112">Počevši od 30 lipnja 2022, završit ćemo podršku za ADAL i AAD Graph i više neće pružati tehničku podršku ni Sigurnosno ažuriranje.</span><span class="sxs-lookup"><span data-stu-id="1c564-112">Starting June 30th, 2022, we will end support for ADAL and AAD Graph and will no longer provide technical support or security updates.</span></span> <span data-ttu-id="1c564-113">Kao rezultat tog stanja, slijede implikacije:</span><span class="sxs-lookup"><span data-stu-id="1c564-113">As a result of this condition, the following are the implications:</span></span>

    - <span data-ttu-id="1c564-114">Aplikacije koje koriste ADAL na postojećim verzijama OS-a nastavit će raditi nakon tog vremena, ali neće dobiti nikakvu tehničku podršku ni Sigurnosno ažuriranje.</span><span class="sxs-lookup"><span data-stu-id="1c564-114">Apps using ADAL on existing OS versions will continue to work after this time but will not get any technical support or security updates.</span></span>

    - <span data-ttu-id="1c564-115">Aplikacije koje koriste AAD Graph nakon tog vremena možda više neće primati odgovore iz krajnje točke AAD grafikona</span><span class="sxs-lookup"><span data-stu-id="1c564-115">Apps using AAD Graph after this time may no longer receive responses from the AAD Graph endpoint</span></span>

<span data-ttu-id="1c564-116">_ *Adal migracija*\*</span><span class="sxs-lookup"><span data-stu-id="1c564-116">_ *ADAL Migration*\*</span></span>

<span data-ttu-id="1c564-117">Ako koristite Microsoftove aplikacije, preporučujemo ažuriranje Microsoftove biblioteke za provjeru autentičnosti (MSAL), koja sadrži najnovije značajke i sigurnosno ažuriranje.</span><span class="sxs-lookup"><span data-stu-id="1c564-117">If you're using Microsoft apps, we recommend updating to the Microsoft Authentication Library (MSAL), which has the latest features and security updates.</span></span> <span data-ttu-id="1c564-118">Ta je preporuka u kontekstu programa Microsoft koji pokreće postupak migracije aplikacija u MSAL uz krajnji rok podrške.</span><span class="sxs-lookup"><span data-stu-id="1c564-118">This recommendation is in the context of Microsoft initiating the process of migrating its apps to MSAL by the end-of-support deadline.</span></span> 

<span data-ttu-id="1c564-119">Migracija Microsoftova aplikacija u MSAL jamči da će aplikacije imati koristi od aktualnih sigurnosti i poboljšanja značajki MSAL-a.</span><span class="sxs-lookup"><span data-stu-id="1c564-119">The migration by Microsoft of its apps to MSAL ensures that the apps benefit from MSAL's ongoing security and feature improvements.</span></span>

1. [<span data-ttu-id="1c564-120">Pročitajte najčešća pitanja o dodatku</span><span class="sxs-lookup"><span data-stu-id="1c564-120">Read the ADAL FAQ</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
2. [<span data-ttu-id="1c564-121">Informacije o migraciji aplikacija na temelju osnove platforme</span><span class="sxs-lookup"><span data-stu-id="1c564-121">Learn about how to migrate apps on a per-platform basis</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
3. <span data-ttu-id="1c564-122">Ako vam je potrebna pomoć u razumijevanju koja aplikacija koristi ADAL, preporučujemo vam da pregledate sve izvorne šifre aplikacija i, ako je moguće, dostupate do svih neovisnih proizvođača softvera (ISVs) ili davatelja aplikacija.</span><span class="sxs-lookup"><span data-stu-id="1c564-122">If you need help in understanding which of your apps use ADAL, we recommend you review all of your apps' source code and, if applicable, reach out to any independent software vendors (ISVs) or app providers.</span></span> <span data-ttu-id="1c564-123">Microsoftova podrška može vam pružiti i popis svih aplikacija koje nisu Microsoftove ADAL u vašem zakupcu.</span><span class="sxs-lookup"><span data-stu-id="1c564-123">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>

<span data-ttu-id="1c564-124">**Migracije grafikona AAD**</span><span class="sxs-lookup"><span data-stu-id="1c564-124">**AAD Graph Migration**</span></span>

<span data-ttu-id="1c564-125">Za aplikacije koje koriste AAD Graph, slijedite upute da biste migrirali aplikacije AAD Graph u Microsoft Graph:</span><span class="sxs-lookup"><span data-stu-id="1c564-125">For applications that are using AAD Graph, follow our guidance to migrate AAD Graph apps to Microsoft Graph:</span></span>

1. <span data-ttu-id="1c564-126">[Naš popis za migraciju sadrži točku početka](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span><span class="sxs-lookup"><span data-stu-id="1c564-126">[Our migration checklist provides a getting started point](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span></span> 
2. <span data-ttu-id="1c564-127">Portal za registraciju servisa Azure sadrži programe koje koristi AAD Graph.</span><span class="sxs-lookup"><span data-stu-id="1c564-127">Your Azure app registration portal shows which applications are using AAD Graph.</span></span> <span data-ttu-id="1c564-128">Preporučujemo da pregledate sve izvorne šifre aplikacija i, ako je primjenjivo, dođete do svih neovisnih proizvođača softvera (ISVs) ili davatelja aplikacija.</span><span class="sxs-lookup"><span data-stu-id="1c564-128">We recommend you review all of your apps' source code and, if applicable, reach out to any independent software vendors (ISVs) or app providers.</span></span> <span data-ttu-id="1c564-129">Microsoftova podrška omogućuje vam i informacije o korištenju AAD grafikona u vašem zakupcu.</span><span class="sxs-lookup"><span data-stu-id="1c564-129">Microsoft support can also provide you information on AAD Graph usage in your tenant.</span></span>







