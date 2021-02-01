---
title: Problemi s bibliotekama za provjeru autentičnosti
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004333"
- "7731"
ms.openlocfilehash: ab4ffbc78a7cadd8acee3c98eaa5f3323da9c7e3
ms.sourcegitcommit: 7e6d89f47eca1babf5aeba4995bceccd990c3963
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 01/28/2021
ms.locfileid: "50063581"
---
# <a name="issues-with-authentication-libraries"></a><span data-ttu-id="bab66-102">Problemi s bibliotekama za provjeru autentičnosti</span><span class="sxs-lookup"><span data-stu-id="bab66-102">Issues with Authentication Libraries</span></span>

1. <span data-ttu-id="bab66-103">[Biblioteke za provjeru autentičnosti Microsoftove platforme za dokumente](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) popisuju Microsoftove podržane i kompatibilne biblioteke klijenta i middleware-a.</span><span class="sxs-lookup"><span data-stu-id="bab66-103">[Microsoft identity platform authentication libraries](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) lists Microsoft-supported and compatible client and middleware libraries.</span></span>
2. <span data-ttu-id="bab66-104">Biblioteka programa Microsoft Authentication (MSAL) podržava nekoliko [tokova provjere autentičnosti](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows) za korištenje u različitim scenarijima aplikacija.</span><span class="sxs-lookup"><span data-stu-id="bab66-104">The Microsoft Authentication Library (MSAL) supports several [authentication flows](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows) for use in different application scenarios.</span></span>
3. <span data-ttu-id="bab66-105">Da biste provjerili autentičnost i nabavili tokene, inicijalizirajte novu javnu ili povjerljivu klijentske aplikacije u kodu.</span><span class="sxs-lookup"><span data-stu-id="bab66-105">To authenticate and acquire tokens, you initialize a new public or confidential client application in your code.</span></span> <span data-ttu-id="bab66-106">Prilikom inicijalizacije klijentske aplikacije u biblioteci Microsoft Authentication (MSAL) možete postaviti nekoliko mogućnosti konfiguracije.</span><span class="sxs-lookup"><span data-stu-id="bab66-106">You can set several configuration options when you initialize the client app in the Microsoft Authentication Library (MSAL).</span></span> <span data-ttu-id="bab66-107">Dodatne informacije potražite u članku [mogućnosti konfiguracije aplikacije](https://docs.microsoft.com/azure/active-directory/develop/msal-client-application-configuration).</span><span class="sxs-lookup"><span data-stu-id="bab66-107">To learn more, see [Application configuration options](https://docs.microsoft.com/azure/active-directory/develop/msal-client-application-configuration).</span></span>

<span data-ttu-id="bab66-108">**Kraj podrške za Azure Active Directory za biblioteku autentičnosti (ADAL) i Azure AD Graph API (AAD Graph)**</span><span class="sxs-lookup"><span data-stu-id="bab66-108">**End of support for Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph)**</span></span>

<span data-ttu-id="bab66-109">**Počevši od 30 lipnja 2020**, više nećemo dodavati nove značajke u AD Graph Adal i Azure.</span><span class="sxs-lookup"><span data-stu-id="bab66-109">**Starting June 30th, 2020**, we will no longer add any new features to ADAL and Azure AD Graph.</span></span> <span data-ttu-id="bab66-110">I dalje ćemo pružati tehničku podršku i sigurnosna ažuriranja, ali više nećemo pružati ažuriranja značajki.</span><span class="sxs-lookup"><span data-stu-id="bab66-110">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>

<span data-ttu-id="bab66-111">**Počevši od 30 lipnja 2022**, završit ćemo podršku za Adal i Azure ad Graph i više neće pružati tehničku podršku ni Sigurnosno ažuriranje.</span><span class="sxs-lookup"><span data-stu-id="bab66-111">**Starting June 30th, 2022**, we will end support for ADAL and Azure AD Graph and will no longer provide technical support or security updates.</span></span>

<span data-ttu-id="bab66-112">Aplikacije koje koriste ADAL na postojećim verzijama OS-a nastavit će raditi nakon tog vremena, ali neće *dobiti nikakvu tehničku podršku ni Sigurnosno ažuriranje*.</span><span class="sxs-lookup"><span data-stu-id="bab66-112">Apps using ADAL on existing OS versions will continue to work after this time but will not *get any technical support or security updates*.</span></span>

<span data-ttu-id="bab66-113">Aplikacije koje koriste Azure AD Graph nakon tog vremena možda više neće primati odgovore iz krajnjih točaka Azure AD Graph.</span><span class="sxs-lookup"><span data-stu-id="bab66-113">Apps using Azure AD Graph after this time may no longer receive responses from the Azure AD Graph endpoint.</span></span>

<span data-ttu-id="bab66-114">**ADAL migracija**</span><span class="sxs-lookup"><span data-stu-id="bab66-114">**ADAL Migration**</span></span>

<span data-ttu-id="bab66-115">Preporučujemo ažuriranje na [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview) koja ima najnovije značajke i sigurnosna ažuriranja.</span><span class="sxs-lookup"><span data-stu-id="bab66-115">We recommend updating to the [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), which has the latest features and security updates.</span></span>

<span data-ttu-id="bab66-116">Ako koristite Microsoftove aplikacije, znajte da je Microsoft u postupku migracije svojih aplikacija u MSAL uz krajnji rok za potporu, čime će se osigurati da koristi MSAL-ove trajne sigurnosti i poboljšanja značajki.</span><span class="sxs-lookup"><span data-stu-id="bab66-116">If you are using Microsoft apps, know that Microsoft is in the process of migrating its applications to MSAL by the end-of-support deadline, ensuring they will benefit from MSAL's ongoing security and feature improvements.</span></span>

<span data-ttu-id="bab66-117">Dodatne informacije potražite u članku:</span><span class="sxs-lookup"><span data-stu-id="bab66-117">For more information, see:</span></span>

1. [<span data-ttu-id="bab66-118">Pročitajte najčešća pitanja vezana za ADAL</span><span class="sxs-lookup"><span data-stu-id="bab66-118">Read the ADAL FAQ</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [<span data-ttu-id="bab66-119">Saznajte kako migrirati aplikacije na platformu</span><span class="sxs-lookup"><span data-stu-id="bab66-119">Learn about how to migrate apps on a per-platform basis</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. <span data-ttu-id="bab66-120">Ako vam je potrebna pomoć u razumijevanju koje aplikacije koriste ADAL, preporučujemo vam da pregledate sve izvorne šifre aplikacija i ako je primjenjivo, obratite se svim pružateljima programa ISVs ili aplikacije.</span><span class="sxs-lookup"><span data-stu-id="bab66-120">If you need help understanding which of your apps use ADAL, we recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="bab66-121">Microsoftova podrška također vam može pružiti popis svih aplikacija koje nisu Microsoftove ADAL u vašem klijentu.</span><span class="sxs-lookup"><span data-stu-id="bab66-121">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>

<span data-ttu-id="bab66-122">**Migracija grafikona AAD**</span><span class="sxs-lookup"><span data-stu-id="bab66-122">**AAD Graph Migration**</span></span>

<span data-ttu-id="bab66-123">Za aplikacije koje koriste Azure AD Graph, slijedite upute da biste [migrirali aplikacije Azure ad Graph u Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview).</span><span class="sxs-lookup"><span data-stu-id="bab66-123">For applications that are using Azure AD Graph, follow our guidance to [migrate Azure AD Graph apps to Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview).</span></span>

1. [<span data-ttu-id="bab66-124">Naš popis za migraciju sadrži točku početka.</span><span class="sxs-lookup"><span data-stu-id="bab66-124">Our migration checklist provides a getting started point.</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)
2. <span data-ttu-id="bab66-125">Vaš portal za registraciju Azure aplikacija prikazuje koje aplikacije koriste AAD Graph.</span><span class="sxs-lookup"><span data-stu-id="bab66-125">Your Azure app registration portal shows which applications are using AAD Graph.</span></span> <span data-ttu-id="bab66-126">Preporučujemo da pregledate izvorni kod svih aplikacija i ako je primjenjivo obratite se svim ISV-ovima ili davateljima aplikacija.</span><span class="sxs-lookup"><span data-stu-id="bab66-126">We recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="bab66-127">Microsoftova podrška može vam pružiti i popis svih korištenja AAD grafikona u vašem zakupcu.</span><span class="sxs-lookup"><span data-stu-id="bab66-127">Microsoft support can also provide you with a list of all AAD Graph usage in your tenant.</span></span>
3. <span data-ttu-id="bab66-128">Da bi aplikacija pristupio podacima u programu Microsoft Graph, korisnik ili administrator mora mu dodijeliti ispravne dozvole putem postupka pristanka.</span><span class="sxs-lookup"><span data-stu-id="bab66-128">For your app to access data in Microsoft Graph, the user or administrator must grant it the correct permissions via a consent process.</span></span> <span data-ttu-id="bab66-129">[Referenca dozvola za Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) prikazuje popise dozvola povezanih sa svakim glavnim skupom programa Microsoft Graph Apis.</span><span class="sxs-lookup"><span data-stu-id="bab66-129">The [Microsoft Graph permissions reference](https://docs.microsoft.com/graph/permissions-reference) lists the permissions associated with each major set of Microsoft Graph APIs.</span></span> <span data-ttu-id="bab66-130">Nudi i upute za korištenje dozvola.</span><span class="sxs-lookup"><span data-stu-id="bab66-130">It also provides guidance about how to use the permissions.</span></span>
