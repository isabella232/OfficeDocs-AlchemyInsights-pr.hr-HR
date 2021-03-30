---
title: Aplikacija za provjeru autentičnosti
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003252"
- "9909"
ms.openlocfilehash: 67331a9661ee67c4a861feb1a4292255a4d37133
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/29/2021
ms.locfileid: "51404365"
---
# <a name="authentication-app"></a><span data-ttu-id="b5e68-102">Aplikacija za provjeru autentičnosti</span><span class="sxs-lookup"><span data-stu-id="b5e68-102">Authentication app</span></span>

<span data-ttu-id="b5e68-103">Ako ste globalni administrator, možete brzo saznati što se dogodilo ili dijagnosticirati probleme vezane uz prijavu korisnika pomoću dijagnostike [za prijavu.](https://ms.portal.azure.com/microsoft.onmicrosoft.com?loginHint=shhada@microsoft.com#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)</span><span class="sxs-lookup"><span data-stu-id="b5e68-103">If you are a Global Admin, you can quickly find out what happened or diagnose problems related to user-sign in by using the [Sign-in Diagnostics](https://ms.portal.azure.com/microsoft.onmicrosoft.com?loginHint=shhada@microsoft.com#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span></span>

1. <span data-ttu-id="b5e68-104">Pokrenite dijagnostiku klikom na gumb["Pokreni](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)dijagnostiku".</span><span class="sxs-lookup"><span data-stu-id="b5e68-104">Start the diagnostics by clicking "[Launch Diagnostic](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)" button.</span></span> 
1. <span data-ttu-id="b5e68-105">Pronađite događaj koji želite analizirati tako da unesete pojedinosti o korisniku, aplikaciji, vremenu prijave, ID-u zahtjeva ili ID-u korelacije.</span><span class="sxs-lookup"><span data-stu-id="b5e68-105">Find the event to analyze by entering in the details you have about the user, application, time of sign-in, request Id, or correlation Id.</span></span>
1. <span data-ttu-id="b5e68-106">Pregledajte dijagnostičke rezultate koji prikazuju pojedinosti o tome što se dogodilo i koje akcije možete poduzeti da biste unijeli promjene, ako su potrebne neke promjene.</span><span class="sxs-lookup"><span data-stu-id="b5e68-106">Review the diagnostic results showing the details of what happened and what actions you can take to make changes, if any changes are needed.</span></span>

<span data-ttu-id="b5e68-107">**Provjerite scenarij koji je primjenjiv:**</span><span class="sxs-lookup"><span data-stu-id="b5e68-107">**Check the scenario that is applicable:**</span></span>

1. <span data-ttu-id="b5e68-108">Ako korisnik ne prima push obavijest u aplikaciji Microsoft Authenticator, provjerite nisu li prikazani pod blokiranim korisnicima MFA-om, kao što je opisano u [članku Blokiraj i deblokiraj korisnike](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span><span class="sxs-lookup"><span data-stu-id="b5e68-108">If a user is not getting a push notification in the Microsoft Authenticator app, verify they are not shown under the MFA blocked users as described in [Block and unblock users](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span></span>
1. <span data-ttu-id="b5e68-109">Ako korisnik nije blokiran za MFA, ali ne prima push obavijest, može otvoriti aplikaciju Microsoft Authenticator, koja će povući zahtjeve za odobrenje na čekanju.</span><span class="sxs-lookup"><span data-stu-id="b5e68-109">If the user is not blocked for MFA but does not receive a push notification, they can open the Microsoft Authenticator app, which will pull the pending approval requests.</span></span>
1. <span data-ttu-id="b5e68-110">Kao alternativni način prijave korisnik može i kliknuti Prijava na drugi način i odabrati korištenje koda za provjeru valjanosti iz mobilne aplikacije.</span><span class="sxs-lookup"><span data-stu-id="b5e68-110">As an alternative sign-in method, the user can also click on Sign in another way and choose use a verification code from my mobile app.</span></span>
1. <span data-ttu-id="b5e68-111">Aplikacija Microsoft Authenticator jedina je dostupna metoda za mnoge korisnike.</span><span class="sxs-lookup"><span data-stu-id="b5e68-111">The Microsoft Authenticator App is the only available method for many users.</span></span> <span data-ttu-id="b5e68-112">[Dodatne informacije o sigurnosnim zadanim postavkama](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)potražite u najčešćim pitanjima o aplikaciji [Authenticator](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-faq) da biste saznali najčešća pitanja i kako ih riješiti.</span><span class="sxs-lookup"><span data-stu-id="b5e68-112">[Learn more about security defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults), check [Authenticator App FAQ](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-faq) for commonly asked questions and how to resolve them.</span></span>
 
<span data-ttu-id="b5e68-113">**Preporučeni videozapisi**</span><span class="sxs-lookup"><span data-stu-id="b5e68-113">**Recommended Videos**</span></span>

<span data-ttu-id="b5e68-114">[Postavljanje aplikacije Authenticator na novom telefonu (2min).](https://go.microsoft.com/fwlink/?linkid=2158163&clcid=0x409)</span><span class="sxs-lookup"><span data-stu-id="b5e68-114">[How to set up Authenticator App on a new phone (2min)](https://go.microsoft.com/fwlink/?linkid=2158163&clcid=0x409).</span></span>
