---
title: Problemi s uvjetnim pristupom
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
- "9004349"
- "7768"
ms.openlocfilehash: 7c20b26e3a038dc4392684ca410eba97cec2df30
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 01/27/2021
ms.locfileid: "50014747"
---
# <a name="conditional-access-issues"></a><span data-ttu-id="06dfb-102">Problemi s uvjetnim pristupom</span><span class="sxs-lookup"><span data-stu-id="06dfb-102">Conditional access issues</span></span>

<span data-ttu-id="06dfb-103">**Rješavanje problema s Dijagnosticiom za prijavu**</span><span class="sxs-lookup"><span data-stu-id="06dfb-103">**Resolve problems with the Sign-in Diagnostic**</span></span>

<span data-ttu-id="06dfb-104">Možete brzo saznati što se dogodilo ili dijagnosticirati poteškoće povezane s korisničkim prijavom pomoću [dijagnostike za prijavu](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom):</span><span class="sxs-lookup"><span data-stu-id="06dfb-104">You can quickly find out what happened or diagnose problems related to user sign-in by using the [Sign-in Diagnostic](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom):</span></span>

1. <span data-ttu-id="06dfb-105">Pokrenite dijagnostiku za prijavu.</span><span class="sxs-lookup"><span data-stu-id="06dfb-105">Launch the Sign-in Diagnostic.</span></span>
1. <span data-ttu-id="06dfb-106">Pronađite događaj za analizu unosom u detalje koje imate o korisniku, aplikaciji, vremenu prijave, ID-u zahtjeva ili ID-u korelacije.</span><span class="sxs-lookup"><span data-stu-id="06dfb-106">Find the event to analyze by entering in the details you have about the user, application, time of sign-in, request Id, or correlation Id.</span></span>
1. <span data-ttu-id="06dfb-107">Pregledajte rezultate dijagnostičkih prikaza s pojedinostima o tome što se dogodilo i koje akcije možete poduzeti da biste unijeli promjene (ako su potrebne promjene).</span><span class="sxs-lookup"><span data-stu-id="06dfb-107">Review the diagnostic results showing the details of what happened and what actions you can take to make changes (if any changes are needed).</span></span>

<span data-ttu-id="06dfb-108">**Koraci za otklanjanje poteškoća s prijavom**</span><span class="sxs-lookup"><span data-stu-id="06dfb-108">**Steps to Troubleshoot a Sign-In**</span></span> 

1. <span data-ttu-id="06dfb-109">Idite na stranicu za prijavu na Azure AD.</span><span class="sxs-lookup"><span data-stu-id="06dfb-109">Navigate to the Azure AD Sign-in page.</span></span>
1. <span data-ttu-id="06dfb-110">Filtriranje prijava prema korisniku, vremenskom rasponu, aplikaciji, statusu, klijentskoj aplikaciji i tako dalje.</span><span class="sxs-lookup"><span data-stu-id="06dfb-110">Filter sign-ins by user, time range, application, status, client app, and so on.</span></span>
1. <span data-ttu-id="06dfb-111">Odaberite događaj prijave i prikažite karticu uvjetni pristup da biste vidjeli koja su pravila vrednovana.</span><span class="sxs-lookup"><span data-stu-id="06dfb-111">Select a sign-in event and view the Conditional Access tab to see which policies were evaluated.</span></span>
1. <span data-ttu-id="06dfb-112">Kliknite redak pravilnika da biste pogledali detalje o politici i razumjeli zašto se primjenjuje.</span><span class="sxs-lookup"><span data-stu-id="06dfb-112">Click on the row of a policy to view the policy details and understand why it applied.</span></span>

<span data-ttu-id="06dfb-113">**Alati za otklanjanje poteškoća s Pravilnikom o uvjetnom pristupu**</span><span class="sxs-lookup"><span data-stu-id="06dfb-113">**Tools to troubleshoot a Conditional Access policy**</span></span>

- <span data-ttu-id="06dfb-114">Način rada samo za izvješća omogućuje procjenu pravilnika bez ometanja korisnika.</span><span class="sxs-lookup"><span data-stu-id="06dfb-114">Report-only mode lets you evaluate a policy without impacting users.</span></span>
- <span data-ttu-id="06dfb-115">Alat što-ako vam omogućuje simulaciju događaja prijave i pogledajte koja se pravila primjenjuju.</span><span class="sxs-lookup"><span data-stu-id="06dfb-115">What-if tool lets you simulate sign-in events and see which policies apply.</span></span>
- <span data-ttu-id="06dfb-116">Radna knjiga uvida i izvješćivanja prikazuje utjecaj svakog pravilnika u stvarnom vremenu.</span><span class="sxs-lookup"><span data-stu-id="06dfb-116">Insights and reporting workbook displays real-time impact of each policy.</span></span>

<span data-ttu-id="06dfb-117">**Osnovna pravila zaštite**</span><span class="sxs-lookup"><span data-stu-id="06dfb-117">**Baseline Protection Policies**</span></span>

<span data-ttu-id="06dfb-118">Osnovna pravila zaštite su deprecated.</span><span class="sxs-lookup"><span data-stu-id="06dfb-118">Baseline Protection policies have been deprecated.</span></span> <span data-ttu-id="06dfb-119">Oni se više ne provode i uskoro će biti uklonjeni iz portala Azure.</span><span class="sxs-lookup"><span data-stu-id="06dfb-119">They are no longer being enforced and will soon be removed from Azure portal.</span></span> <span data-ttu-id="06dfb-120">Preporučujemo omogućavanje [sigurnosnih zadanih postavki](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span><span class="sxs-lookup"><span data-stu-id="06dfb-120">We recommend enabling [security defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span></span>

<span data-ttu-id="06dfb-121">Dodatne informacije o uvjetnom pristupu potražite u članku:</span><span class="sxs-lookup"><span data-stu-id="06dfb-121">For more information on Conditional Access see:</span></span>

<span data-ttu-id="06dfb-122">[Najbolje prakse za uvjetni pristup u servisu Azure Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Uvjeti u uvjetnom pristupu](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Kontrole u uvjetnom pristupu](https://docs.microsoft.com/azure/active-directory/conditional-access/controls)  
 [Mjesta u uvjetnom pristupu](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)</span><span class="sxs-lookup"><span data-stu-id="06dfb-122">[Best practices for conditional access in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices) 
[Conditions in Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices) 
[Controls in Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/controls) 
[Locations in Conditional Access ](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)</span></span>
