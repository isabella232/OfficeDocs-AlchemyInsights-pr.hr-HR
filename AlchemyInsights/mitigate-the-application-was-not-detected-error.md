---
title: Ublažavanje pogreške "Aplikacija nije otkrivena"
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000171"
- "1712"
ms.openlocfilehash: e07c6b128a39f1fb1c998d051aafe72205d8cbee
ms.sourcegitcommit: 82155846ce771c18050e6113d6c199b34a1504ff
ms.translationtype: HT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/24/2020
ms.locfileid: "43810476"
---
# <a name="mitigate-the-application-was-not-detected-error"></a><span data-ttu-id="50647-102">Ublažavanje pogreške "Aplikacija nije otkrivena"</span><span class="sxs-lookup"><span data-stu-id="50647-102">Mitigate "The application was not detected" error</span></span>

<span data-ttu-id="50647-103">Pogreška prilikom instalacije aplikacije koja glasi "Aplikacija nije otkrivena nakon uspješnog dovršetka instalacije", koju prijavljuje Intune, može se pojaviti u svim većim OS-ovima (Windows, iOS i Android).</span><span class="sxs-lookup"><span data-stu-id="50647-103">The app installation error, “The application was not detected after installation completed successfully,” reported by Intune, may occur on all major OS platforms (Windows, iOS and Android).</span></span>

<span data-ttu-id="50647-104">Najčešći su scenariji koji generiraju tu pogrešku sljedeći:</span><span class="sxs-lookup"><span data-stu-id="50647-104">The most common scenarios that generate this error include:</span></span>

- <span data-ttu-id="50647-105">Aplikacija je nakon početne implementacije ažurirana izvan servisa Intune (iz trgovine aplikacija drugog proizvođača).</span><span class="sxs-lookup"><span data-stu-id="50647-105">The app has been updated outside of Intune (from a third-party app store) after the initial deployment.</span></span> <span data-ttu-id="50647-106">Primjerice, neke aplikacije kao što je Google Chrome mogu provoditi automatska ažuriranja.</span><span class="sxs-lookup"><span data-stu-id="50647-106">For example some applications such as Google Chrome may perform auto updates.</span></span>
- <span data-ttu-id="50647-107">Korisnik je deinstalirao aplikaciju nakon inicijalne instalacije.</span><span class="sxs-lookup"><span data-stu-id="50647-107">A user has uninstalled the app after the initial install.</span></span>

<span data-ttu-id="50647-108">Da biste ublažili taj problem, najprije izvršite pregled uređaja na kojima se on pojavljuje i utvrdite scenarij u kojem dolazi do pogreške.</span><span class="sxs-lookup"><span data-stu-id="50647-108">To mitigate this issue, first perform a review of the affected devices to determine the scenario in which the error occurs.</span></span>

- <span data-ttu-id="50647-109">Ako se aplikacija ažurirala izvan servisa Intune, implementacija aplikacije može se postaviti tako da ignorira verziju aplikacije.</span><span class="sxs-lookup"><span data-stu-id="50647-109">If the app has been updated outside of Intune, the app deployment can be set to ignore the application version.</span></span> <span data-ttu-id="50647-110">Da biste to učinili, u odjeljku **Konfiguracija aplikacije > Informacije o aplikaciji** postavite **Zanemari verziju aplikacije** na **Da**.</span><span class="sxs-lookup"><span data-stu-id="50647-110">To do so, under **App Configuration > App Information**, set **Ignore App** version to **Yes**.</span></span>
- <span data-ttu-id="50647-111">Prilikom ciljanja klijenata može biti primjereno implementirati aplikaciju kao "obaveznu" i osigurati implementaciju najnovije verzije.</span><span class="sxs-lookup"><span data-stu-id="50647-111">When targeting the client, it may be appropriate to deploy the application as “required,” and to ensure that the latest version is deployed.</span></span>
- <span data-ttu-id="50647-112">Umjesto toga na platformi iOS može se koristiti funkcija **automatskog ažuriranja** povezana s programom Apple Volume Purchase, koja se može konfigurirati za automatsko ažuriranje na nove verzije aplikacija čim one postanu dostupne.</span><span class="sxs-lookup"><span data-stu-id="50647-112">Alternatively, on the iOS platform, it is possible to use the **autoupdate** functionality associated with the Apple Volume Purchase Program, which can be configured to automatically update to new application versions as they become available.</span></span>

<span data-ttu-id="50647-113">Dodatne informacije o otklanjanju poteškoća s instalacijom aplikacija potražite u članku [Otklanjanje poteškoća s instalacijom aplikacija](https://docs.microsoft.com/intune/troubleshoot-app-install).</span><span class="sxs-lookup"><span data-stu-id="50647-113">For more information about troubleshooting app installation issues, please see [Troubleshoot app installation issues](https://docs.microsoft.com/intune/troubleshoot-app-install).</span></span>
