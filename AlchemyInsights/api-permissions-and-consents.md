---
title: API dozvole i pristanak
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
- "7756"
ms.openlocfilehash: c99e5e2e8fb9bcc88e5221890ed9c28ed9e7d0c8
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974259"
---
# <a name="api-permissions-and-consent"></a><span data-ttu-id="b3a93-102">API dozvole i pristanak</span><span class="sxs-lookup"><span data-stu-id="b3a93-102">API permissions and consent</span></span>

<span data-ttu-id="b3a93-103">Aplikacije koje se integriraju sa platformom Microsoftova identiteta slijede model autorizacije koji korisnicima i administratorima omogućuje kontrolu nad načinom pristupa podacima.</span><span class="sxs-lookup"><span data-stu-id="b3a93-103">Applications that integrate with Microsoft identity platform follow an authorization model that gives users and administrators control over how data can be accessed.</span></span> <span data-ttu-id="b3a93-104">Implementacija modela autorizacije ažurirana je na krajnjoj točki Microsoftove identifikacijske platforme.</span><span class="sxs-lookup"><span data-stu-id="b3a93-104">The implementation of the authorization model has been updated on the Microsoft identity platform endpoint.</span></span> <span data-ttu-id="b3a93-105">Mijenja način interakcije aplikacije s Microsoftovu platformom Identity.</span><span class="sxs-lookup"><span data-stu-id="b3a93-105">It changes how an app must interact with the Microsoft identity platform.</span></span> <span data-ttu-id="b3a93-106">[Dozvole i pristanak u krajnjoj točki platforme Microsoft Identity](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) obuhvaća osnovne koncepte ovog modela autorizacije, uključujući dosege, dozvole i pristanak.</span><span class="sxs-lookup"><span data-stu-id="b3a93-106">[Permissions and consent in the Microsoft identity platform endpoint](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) covers the basic concepts of this authorization model, including scopes, permissions, and consent.</span></span>

<span data-ttu-id="b3a93-107">[Okvir za suglasnost servisa Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) olakšava razvijanje web-mjesta i izvornih klijentskih aplikacija za više korisnika.</span><span class="sxs-lookup"><span data-stu-id="b3a93-107">The [Azure Active Directory (Azure AD) consent framework](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) makes it easy to develop multi-tenant web and native client applications.</span></span> <span data-ttu-id="b3a93-108">Te aplikacije omogućuju prijavu za korisničke račune iz stanara Azure AD koji se razlikuje od onog u kojem je aplikacija registrirana.</span><span class="sxs-lookup"><span data-stu-id="b3a93-108">These applications allow sign-in by user accounts from an Azure AD tenant that's different from the one where the application is registered.</span></span> <span data-ttu-id="b3a93-109">Možda će morati pristupati i web-API-Jima, kao što je Microsoft Graph API (da biste pristupili Azure AD, Intune i Services u programu Microsoft 365) i drugim API-Jima sustava Microsoft Services, uz vlastite web-API-je.</span><span class="sxs-lookup"><span data-stu-id="b3a93-109">They may also need to access web APIs such as the Microsoft Graph API (to access Azure AD, Intune, and services in Microsoft 365) and other Microsoft services' APIs, in addition to your own web APIs.</span></span>

