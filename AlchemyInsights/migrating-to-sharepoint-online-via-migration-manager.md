---
title: Migracija u SharePoint online putem upravitelja migracije
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "5300030"
- "3192"
ms.openlocfilehash: 5aebf7903670e74f616c8f151749d760caf1d642
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931871"
---
# <a name="migrating-to-sharepoint-online-via-migration-manager"></a><span data-ttu-id="8745f-102">Migracija u SharePoint online putem upravitelja migracije</span><span class="sxs-lookup"><span data-stu-id="8745f-102">Migrating to SharePoint Online via Migration Manager</span></span>

<span data-ttu-id="8745f-103">**Važno**: Mnogi korisnici sustava SharePoint Online i OneDrive pokreću poslovne ključne aplikacije na servis koji se izvodi u pozadini.</span><span class="sxs-lookup"><span data-stu-id="8745f-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="8745f-104">To obuhvaća migraciju sadržaja, sprječavanje gubitka podataka (DLP) i rješenja za sigurnosno kopiranje.</span><span class="sxs-lookup"><span data-stu-id="8745f-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="8745f-105">Tijekom tih presedana poduzimamo korake da bi servisi sustava SharePoint Online i servisi OneDrive ostali iznimno raspoloživi i pouzdani za korisnike koji više nego ikad ovise o servisu u udaljenim radnim scenarijima.</span><span class="sxs-lookup"><span data-stu-id="8745f-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="8745f-106">Na temelju podrške tog cilja implementirali smo čvršća restriktivna ograničenja na pozadinske aplikacije (migracija, DLP i rješenja sigurnosnih kopija) tijekom radnog dana.</span><span class="sxs-lookup"><span data-stu-id="8745f-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="8745f-107">Trebali biste očekivati da će te aplikacije tijekom tog vremena doseći ograničen protok.</span><span class="sxs-lookup"><span data-stu-id="8745f-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="8745f-108">No tijekom večeri i vikenda u regiji servis će biti spreman za obradu znatno većeg volumena zahtjeva iz pozadinske aplikacije.</span><span class="sxs-lookup"><span data-stu-id="8745f-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="8745f-109">**Upravitelj migracije**</span><span class="sxs-lookup"><span data-stu-id="8745f-109">**Migration Manager**</span></span>

<span data-ttu-id="8745f-110">Upravitelj migracije koji se nalazi u modernom centru za administratore sustava SharePoint vodi vas kroz postavljanje klijenata i stvaranje zadataka.</span><span class="sxs-lookup"><span data-stu-id="8745f-110">Located in the modern SharePoint Admin Center, the Migration Manager guides you through the setup of your clients and the creation of your tasks.</span></span> <span data-ttu-id="8745f-111">Možete odrediti globalne postavke sustava ili razina zadatka, pregledavati napredak cjelokupnog zadatka te preuzeti zbirne sažetke i izvješća na razini zadatka.</span><span class="sxs-lookup"><span data-stu-id="8745f-111">You can specify global or task-level settings, view all-up task progress, and download aggregated summary and task-level reports.</span></span>

- [<span data-ttu-id="8745f-112">Krenite s upraviteljem migracije</span><span class="sxs-lookup"><span data-stu-id="8745f-112">Get started with the Migration Manager</span></span>](https://docs.microsoft.com/sharepointmigration/mm-get-started)

- [<span data-ttu-id="8745f-113">Postavite klijente upravitelja migracije</span><span class="sxs-lookup"><span data-stu-id="8745f-113">Setup Migration Manager clients</span></span>](https://docs.microsoft.com/sharepointmigration/mm-setup-clients)

- [<span data-ttu-id="8745f-114">Postavke upravitelja migracija</span><span class="sxs-lookup"><span data-stu-id="8745f-114">Migration Manager Settings</span></span>](https://docs.microsoft.com/sharepointmigration/mm-settings)
