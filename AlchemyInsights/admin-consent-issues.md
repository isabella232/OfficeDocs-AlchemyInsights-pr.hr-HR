---
title: Problemi s pristankom za administratore
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
- "9004354"
- "7786"
ms.openlocfilehash: 6154b4b9cce51be3271cb25132f409319d8da14b
ms.sourcegitcommit: 113b802081101de70810fc73938ea92f7518d8c6
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 01/18/2021
ms.locfileid: "49900822"
---
# <a name="admin-consent-issues"></a><span data-ttu-id="e93cf-102">Problemi s pristankom za administratore</span><span class="sxs-lookup"><span data-stu-id="e93cf-102">Admin consent issues</span></span>

1. <span data-ttu-id="e93cf-103">Omogući [tijek rada pristanka](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-admin-consent-workflow) administratora da biste korisnicima dopustili zahtjev za administratorom izravno na zaslonu pristanak.</span><span class="sxs-lookup"><span data-stu-id="e93cf-103">Enable the [admin consent workflow](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-admin-consent-workflow) to allow users to request administrator approval directly from the consent screen.</span></span>

1. <span data-ttu-id="e93cf-104">Ako vam se u postupku pristanka prikazuje neočekivana pogreška, u ovom se članku radi otklanjanja poteškoća: [neočekivano pogreške prilikom izvođenja pristanka na aplikaciju](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).</span><span class="sxs-lookup"><span data-stu-id="e93cf-104">If you or your application's users are seeing unexpected errors during the consent process, see this article for troubleshooting steps: [Unexpected error when performing consent to an application](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).</span></span>

1. <span data-ttu-id="e93cf-105">Saznajte više o [pristanku za administratore na Microsoftovoj platformi identiteta](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent), kako funkcionira [upit za suglasnost](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent) i kako [procijeniti zahtjev za pristanak administratora na razini korisnika](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent).</span><span class="sxs-lookup"><span data-stu-id="e93cf-105">Learn more about [Admin consent on the Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent), how the [consent prompt](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent) works, and how to [evaluate a request for tenant-wide admin consent](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent).</span></span>

1. <span data-ttu-id="e93cf-106">Aplikacije koje se integriraju sa platformom Microsoftova identiteta slijede model autorizacije koji korisnicima i administratorima omogućuje kontrolu nad načinom pristupa podacima.</span><span class="sxs-lookup"><span data-stu-id="e93cf-106">Applications that integrate with Microsoft identity platform follow an authorization model that gives users and administrators control over how data can be accessed.</span></span> <span data-ttu-id="e93cf-107">Implementacija modela autorizacije ažurirana je na krajnjoj točki platforme Microsoftova identiteta i mijenja način interakcije aplikacije s Microsoftovu platformom Identity.</span><span class="sxs-lookup"><span data-stu-id="e93cf-107">The implementation of the authorization model has been updated on the Microsoft identity platform endpoint, and it changes how an app must interact with the Microsoft identity platform.</span></span> <span data-ttu-id="e93cf-108">Pogledajte [dozvole i pristanak u krajnjoj točki platforme Microsoftova identiteta](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent) za pregled ovog modela autorizacije, uključujući dosege, dozvole i pristanak.</span><span class="sxs-lookup"><span data-stu-id="e93cf-108">See [Permissions and consent in the Microsoft identity platform endpoint](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent) for an overview of this authorization model, including scopes, permissions, and consent.</span></span>