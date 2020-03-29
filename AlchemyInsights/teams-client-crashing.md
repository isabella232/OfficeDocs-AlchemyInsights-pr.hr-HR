---
title: Klijent za Teams se ruši?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002323"
- "4512"
ms.openlocfilehash: ce37b260d126f876d2b6177515bd8a7c3874ef2c
ms.sourcegitcommit: d02e2b73aa7d0453d7baca1ea5a186cf6081d022
ms.translationtype: HT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/27/2020
ms.locfileid: "43030539"
---
# <a name="teams-client-crashing"></a><span data-ttu-id="3166e-102">Klijent za Teams se ruši?</span><span class="sxs-lookup"><span data-stu-id="3166e-102">Teams client crashing?</span></span>

<span data-ttu-id="3166e-103">Ako vam se klijent za Teams ruši, pokušajte sljedeće:</span><span class="sxs-lookup"><span data-stu-id="3166e-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="3166e-104">Ako koristite Teams za stolna računala, [provjerite je li program u potpunosti ažuriran](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="3166e-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="3166e-105">Provjerite jesu li dostupni svi [URL-ovi i rasponi adresa sustava Office 365](https://docs.microsoft.com/microsoftteams/connectivity-issues).</span><span class="sxs-lookup"><span data-stu-id="3166e-105">Make sure all the [Office 365 URL's and address ranges](https://docs.microsoft.com/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="3166e-106">Prijavite se pomoću administratorskog računa i na [nadzornoj ploči stanja servisa](https://docs.microsoft.com/office365/enterprise/view-service-health) provjerite da nema prekida ili degradacije servisa.</span><span class="sxs-lookup"><span data-stu-id="3166e-106">Log in with your admin account and check your [Service Health Dashboard](https://docs.microsoft.com/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

 - <span data-ttu-id="3166e-107">Kao zadnji korak možete pokušati očistiti predmemoriju klijenta za Teams:</span><span class="sxs-lookup"><span data-stu-id="3166e-107">As a last step, you can attempt to clear your Teams client cache:</span></span>

    1.  <span data-ttu-id="3166e-108">Izađite iz klijenta za Microsoft Teams za računala.</span><span class="sxs-lookup"><span data-stu-id="3166e-108">Fully exit the Microsoft Teams desktop client.</span></span> <span data-ttu-id="3166e-109">Možete desnom tipkom miša kliknuti **Teams** u području palete na programskoj traci te kliknuti **Zatvori** ili pokrenuti upravitelj zadataka i u potpunosti ubiti proces.</span><span class="sxs-lookup"><span data-stu-id="3166e-109">You can right-click **Teams** from the Icon Tray and click **Quit**, or run Task Manager and fully kill the process.</span></span>

    2.  <span data-ttu-id="3166e-110">Otvorite Eksplorer za datoteke i upišite %appdata%\Microsoft\teams.</span><span class="sxs-lookup"><span data-stu-id="3166e-110">Go to File Explorer, and type in %appdata%\Microsoft\teams.</span></span>

    3.  <span data-ttu-id="3166e-111">Kad otvorite taj direktorij, vidjet ćete neke od ovih mapa:</span><span class="sxs-lookup"><span data-stu-id="3166e-111">Once in the directory, you'll see a few of the following folders:</span></span>

         - <span data-ttu-id="3166e-112">Iz mape **Application Cache** otvorite Cache i izbrišite sve datoteke na mjestu  predmemorije: %appdata%\Microsoft\teams\application cache\cache.</span><span class="sxs-lookup"><span data-stu-id="3166e-112">From within **Application Cache**, go to Cache and delete any of the files in the Cache location:  %appdata%\Microsoft\teams\application cache\cache.</span></span>

        - <span data-ttu-id="3166e-113">Iz mape **Blob_storage** izbrišite sve datoteke: %appdata%\Microsoft\teams\ blob_storage.</span><span class="sxs-lookup"><span data-stu-id="3166e-113">From within **Blob_storage**, delete all files: %appdata%\Microsoft\teams\blob_storage.</span></span>

        - <span data-ttu-id="3166e-114">Iz mape **Cache** izbrišite sve datoteke: %appdata%\Microsoft\teams\Cache.</span><span class="sxs-lookup"><span data-stu-id="3166e-114">From within **Cache**, delete all files: %appdata%\Microsoft\teams\Cache.</span></span>

        - <span data-ttu-id="3166e-115">Iz mape **databases** izbrišite sve datoteke: %appdata%\Microsoft\teams\databases.</span><span class="sxs-lookup"><span data-stu-id="3166e-115">From within **databases**, delete all files: %appdata%\Microsoft\teams\databases.</span></span>

        - <span data-ttu-id="3166e-116">Iz mape **GPUCache** izbrišite sve datoteke: %appdata%\Microsoft\teams\GPUcache.</span><span class="sxs-lookup"><span data-stu-id="3166e-116">From within **GPUCache**, delete all files: %appdata%\Microsoft\teams\GPUcache.</span></span>

        - <span data-ttu-id="3166e-117">Iz mape **IndexedDB** izbrišite .db datoteku: %appdata%\Microsoft\teams\IndexedDB.</span><span class="sxs-lookup"><span data-stu-id="3166e-117">From within **IndexedDB**, delete the .db file: %appdata%\Microsoft\teams\IndexedDB.</span></span>

        - <span data-ttu-id="3166e-118">Iz mape **Local storage** izbrišite sve datoteke: %appdata%\Microsoft\teams\Local Storage.</span><span class="sxs-lookup"><span data-stu-id="3166e-118">From within **Local Storage**, delete all files: %appdata%\Microsoft\teams\Local Storage.</span></span>

        - <span data-ttu-id="3166e-119">Na kraju iz mape **tmp** izbrišite sve datoteke: %appdata%\Microsoft\teams\tmp.</span><span class="sxs-lookup"><span data-stu-id="3166e-119">Lastly, from within **tmp**, delete any file: %appdata%\Microsoft\teams\tmp.</span></span>

    4. <span data-ttu-id="3166e-120">Ponovno pokrenite klijent za Teams.</span><span class="sxs-lookup"><span data-stu-id="3166e-120">Restart your Teams client.</span></span>
