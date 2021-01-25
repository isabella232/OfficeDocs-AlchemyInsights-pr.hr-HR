---
title: Problemi u razvoju aplikacija s API-Jima
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004343"
- "7755"
ms.openlocfilehash: 26d732819b64efa4fb84da44cc2a279368aa28b0
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974263"
---
# <a name="issues-developing-applications-with-apis"></a><span data-ttu-id="7cdb5-102">Problemi u razvoju aplikacija s API-Jima</span><span class="sxs-lookup"><span data-stu-id="7cdb5-102">Issues developing applications with APIs</span></span>

<span data-ttu-id="7cdb5-103">Da biste započeli korištenje API-ja za Azure Active Directory, pogledajte [priručnik za Azure ad Graph](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) (brz početak rada) ili pogledajte [dokumentaciju o referenci API-ja za interaktivne Azure ad Graph](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog).</span><span class="sxs-lookup"><span data-stu-id="7cdb5-103">To begin using the Azure Active Directory Graph API, see the [Azure AD Graph API quickstart guide](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) , or view the [interactive Azure AD Graph API reference documentation](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog).</span></span>

<span data-ttu-id="7cdb5-104">**Kraj podrške za Azure Active Directory za biblioteku autentičnosti (ADAL) i Azure AD Graph API (AAD Graph)**</span><span class="sxs-lookup"><span data-stu-id="7cdb5-104">**End of support for Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph)**</span></span>

<span data-ttu-id="7cdb5-105">**Počevši od 30 lipnja 2020**, više nećemo dodavati nove značajke u AD Graph Adal i Azure.</span><span class="sxs-lookup"><span data-stu-id="7cdb5-105">**Starting June 30th, 2020**, we will no longer add any new features to ADAL and Azure AD Graph.</span></span> <span data-ttu-id="7cdb5-106">Nastavit ćemo pružati tehničku podršku i sigurnosno ažuriranje, ali više nećemo pružati ažuriranja značajki.</span><span class="sxs-lookup"><span data-stu-id="7cdb5-106">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>

<span data-ttu-id="7cdb5-107">**Počevši od 30 lipnja 2022**, završit ćemo podršku za Adal i Azure ad Graph i više neće pružati tehničku podršku ni Sigurnosno ažuriranje.</span><span class="sxs-lookup"><span data-stu-id="7cdb5-107">**Starting June 30th, 2022**, we will end support for ADAL and Azure AD Graph and will no longer provide technical support or security updates.</span></span>

<span data-ttu-id="7cdb5-108">Aplikacije koje koriste ADAL na postojećim verzijama OS-a nastavit će raditi nakon tog vremena, ali neće dobiti nikakvu tehničku podršku ni Sigurnosno ažuriranje.</span><span class="sxs-lookup"><span data-stu-id="7cdb5-108">Apps using ADAL on existing OS versions will continue to work after this time but will not get any technical support or security updates.</span></span>

<span data-ttu-id="7cdb5-109">Aplikacije koje koriste Azure AD Graph nakon tog vremena možda više neće primati odgovore iz krajnjih točaka Azure AD Graph.</span><span class="sxs-lookup"><span data-stu-id="7cdb5-109">Apps using Azure AD Graph after this time may no longer receive responses from the Azure AD Graph endpoint.</span></span>

<span data-ttu-id="7cdb5-110">**ADAL migracija**</span><span class="sxs-lookup"><span data-stu-id="7cdb5-110">**ADAL Migration**</span></span>

<span data-ttu-id="7cdb5-111">Preporučujemo ažuriranje [Microsoftove biblioteke za provjeru autentičnosti (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), koja sadrži najnovije značajke i sigurnosno ažuriranje.</span><span class="sxs-lookup"><span data-stu-id="7cdb5-111">We recommend updating to the [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), which has the latest features and security updates.</span></span>

<span data-ttu-id="7cdb5-112">Ako koristite Microsoftove aplikacije, znajte da je Microsoft u postupku migracije svojih aplikacija u MSAL uz krajnji rok za potporu, čime će se osigurati da koristi MSAL-ove trajne sigurnosti i poboljšanja značajki.</span><span class="sxs-lookup"><span data-stu-id="7cdb5-112">If you're using Microsoft apps, know that Microsoft is in the process of migrating its applications to MSAL by the end-of-support deadline, ensuring they'll benefit from MSAL's ongoing security and feature improvements.</span></span>

1. <span data-ttu-id="7cdb5-113">[Pročitajte najčešća pitanja o dodatku](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span><span class="sxs-lookup"><span data-stu-id="7cdb5-113">[Read the ADAL FAQ](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span></span>
1. <span data-ttu-id="7cdb5-114">[Saznajte kako migrirati aplikacije na osnovi po platformi](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span><span class="sxs-lookup"><span data-stu-id="7cdb5-114">[Learn about how to migrate apps on a per-platform basis](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span></span>
1. <span data-ttu-id="7cdb5-115">Ako vam je potrebna pomoć u razumijevanju koje aplikacije koriste ADAL, preporučujemo vam da pregledate sve izvorne šifre aplikacija i ako je primjenjivo, obratite se svim pružateljima programa ISVs ili aplikacije.</span><span class="sxs-lookup"><span data-stu-id="7cdb5-115">If you need help understanding which of your apps use ADAL, we recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="7cdb5-116">Microsoftova podrška može vam pružiti i popis svih aplikacija koje nisu Microsoftove ADAL u vašem zakupcu.</span><span class="sxs-lookup"><span data-stu-id="7cdb5-116">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>

<span data-ttu-id="7cdb5-117">**Migracije grafikona AAD**</span><span class="sxs-lookup"><span data-stu-id="7cdb5-117">**AAD Graph Migration**</span></span>

<span data-ttu-id="7cdb5-118">Za aplikacije koje koriste Azure AD Graph, slijedite upute da biste migrirali [aplikacije Azure ad Graph u Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="7cdb5-118">For applications that are using Azure AD Graph, follow our guidance to migrate [Azure AD Graph apps to Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true).</span></span>

1. <span data-ttu-id="7cdb5-119">[Naš popis za migraciju sadrži točku početka](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span><span class="sxs-lookup"><span data-stu-id="7cdb5-119">[Our migration checklist provides a getting started point](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span></span> 
1. <span data-ttu-id="7cdb5-120">Portal za registraciju servisa Azure sadrži programe koje koristi AAD Graph.</span><span class="sxs-lookup"><span data-stu-id="7cdb5-120">Your Azure app registration portal shows which applications are using AAD Graph.</span></span> <span data-ttu-id="7cdb5-121">Preporučujemo vam da pregledate sve izvorne šifre aplikacija, a ako je primjenjivo, obratite se svim pružateljima programa ISVs ili aplikacije.</span><span class="sxs-lookup"><span data-stu-id="7cdb5-121">We recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="7cdb5-122">Microsoftova podrška može vam pružiti i popis svih korištenja AAD grafikona u vašem zakupcu.</span><span class="sxs-lookup"><span data-stu-id="7cdb5-122">Microsoft support can also provide you with a list of all AAD Graph usage in your tenant.</span></span>
1. <span data-ttu-id="7cdb5-123">Da bi aplikacija pristupio podacima u programu Microsoft Graph, korisnik ili administrator mora mu dodijeliti ispravne dozvole putem postupka pristanka.</span><span class="sxs-lookup"><span data-stu-id="7cdb5-123">For your app to access data in Microsoft Graph, the user or administrator must grant it the correct permissions via a consent process.</span></span> <span data-ttu-id="7cdb5-124">[Referenca dozvola za Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) prikazuje popise dozvola povezanih sa svakim glavnim skupom programa Microsoft Graph Apis.</span><span class="sxs-lookup"><span data-stu-id="7cdb5-124">The [Microsoft Graph permissions reference](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) lists the permissions associated with each major set of Microsoft Graph APIs.</span></span> <span data-ttu-id="7cdb5-125">Nudi i upute za korištenje dozvola.</span><span class="sxs-lookup"><span data-stu-id="7cdb5-125">It also provides guidance about how to use the permissions.</span></span>
