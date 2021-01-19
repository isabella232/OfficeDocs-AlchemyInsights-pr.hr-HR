---
title: Otklanjanje poteškoća s korisničkim pristajanjem
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004353"
- "7785"
ms.openlocfilehash: 7249bafe1b047c66d9351a79f1782cfcc1a936a1
ms.sourcegitcommit: 7b213fd5e8a3fdb5c602673dc194d576d372ac96
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 01/18/2021
ms.locfileid: "49900839"
---
# <a name="troubleshoot-user-consent"></a><span data-ttu-id="7340e-102">Otklanjanje poteškoća s korisničkim pristajanjem</span><span class="sxs-lookup"><span data-stu-id="7340e-102">Troubleshoot user consent</span></span>

1. <span data-ttu-id="7340e-103">Možete konfigurirati način na koji krajnji korisnici mogu pristati na aplikacije putem portala Azure ili komponente PowerShell.</span><span class="sxs-lookup"><span data-stu-id="7340e-103">You can configure how end-users consent to applications through the Azure Portal or PowerShell.</span></span> <span data-ttu-id="7340e-104">Dodatne informacije potražite u članku [Postavke pristanka korisnika](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) .</span><span class="sxs-lookup"><span data-stu-id="7340e-104">See [User consent settings](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) for more information.</span></span>
1. <span data-ttu-id="7340e-105">Administrator može koristiti i [Microsoft Graph API](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) za odobravanje pristanka na delegirane dozvole u ime jednog korisnika.</span><span class="sxs-lookup"><span data-stu-id="7340e-105">An administrator can also use the [Microsoft Graph API](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) to grant consent to delegated permissions on behalf of a single user.</span></span> <span data-ttu-id="7340e-106">Dodatne informacije potražite u članku [dohvaćanje programa Access u ime korisnika](https://docs.microsoft.com/graph/auth-v2-user).</span><span class="sxs-lookup"><span data-stu-id="7340e-106">For more information, see [Get access on behalf of a user](https://docs.microsoft.com/graph/auth-v2-user).</span></span>
1. <span data-ttu-id="7340e-107">[Pogreške prilikom pristanka korisnika](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error): u ovom se članku opisuju pogreške koje se mogu pojaviti tijekom postupka pristanka na aplikaciju.</span><span class="sxs-lookup"><span data-stu-id="7340e-107">[User Consent Errors](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error): this article discusses errors that can occur during the process of consenting to an application.</span></span> <span data-ttu-id="7340e-108">Ako otklanjate poteškoće s neočekivanim odobrenjem koje ne sadrže poruke o pogrešci, pročitajte članak [scenariji provjere autentičnosti za Azure ad](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).</span><span class="sxs-lookup"><span data-stu-id="7340e-108">If you are troubleshooting unexpected consent prompts that do not contain any error messages, see [Authentication Scenarios for Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).</span></span>