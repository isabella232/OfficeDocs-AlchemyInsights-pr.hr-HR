---
title: Korisničke pogreške prilikom prijave
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7790"
- "9004355"
ms.openlocfilehash: 05bd31cb4afecf1342e040eecd9e58cd38bd8d49
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 01/18/2021
ms.locfileid: "49900791"
---
# <a name="user-sign-in-errors"></a><span data-ttu-id="2743c-102">Korisničke pogreške prilikom prijave</span><span class="sxs-lookup"><span data-stu-id="2743c-102">User sign-in errors</span></span>

<span data-ttu-id="2743c-103">**Rješavanje problema s Dijagnosticiom za prijavu**</span><span class="sxs-lookup"><span data-stu-id="2743c-103">**Resolve problems with the Sign-in Diagnostic**</span></span>

<span data-ttu-id="2743c-104">Da biste otkrili uzrok ili dijagnosticirali poteškoće povezane s korisničkim prijavom, učinite sljedeće:</span><span class="sxs-lookup"><span data-stu-id="2743c-104">To detect the cause or diagnose problems related to user sign-in, perform the following steps:</span></span>

1. <span data-ttu-id="2743c-105">Pokrenite [dijagnostiku za prijavu](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span><span class="sxs-lookup"><span data-stu-id="2743c-105">Launch the [Sign-in Diagnostic](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span></span>
2. <span data-ttu-id="2743c-106">Pronađite događaj za analizu unosom pojedinosti koje imate o korisniku, aplikaciji, vremenu prijave, ID-u zahtjeva ili ID-u korelacije.</span><span class="sxs-lookup"><span data-stu-id="2743c-106">Find the event to analyze by entering the details you have about the user, application, time of sign in, request Id, or correlation Id.</span></span>
3. <span data-ttu-id="2743c-107">Pregledajte rezultate dijagnostičkih prikaza s pojedinostima o tome što se dogodilo i koje akcije možete poduzeti da biste unijeli promjene, ako su potrebne promjene.</span><span class="sxs-lookup"><span data-stu-id="2743c-107">Review the diagnostic results showing the details of what happened and what actions you can take to make changes, if any changes are needed.</span></span>

<span data-ttu-id="2743c-108">**Tražite informacije o kodovima pogrešaka AADSTS koji se vraćaju iz servisa za sigurnost tokena za Azure Active Directory (Azure AD)?**</span><span class="sxs-lookup"><span data-stu-id="2743c-108">**Looking for information about the AADSTS error codes that are returned from the Azure Active Directory (Azure AD) security token service (STS)?**</span></span> <span data-ttu-id="2743c-109">Pročitajte [ovaj članak](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) da biste pronašli AADSTS opise pogrešaka, ispravke i nekoliko predloženih zaobilaznih rješenja</span><span class="sxs-lookup"><span data-stu-id="2743c-109">Read [this article](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) to find AADSTS error descriptions, fixes, and some suggested workarounds</span></span>