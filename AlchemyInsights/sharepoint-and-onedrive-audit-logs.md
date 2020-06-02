---
title: Klasična izvješća zapisnika nadzora sustava SharePoint
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 0aedb549f11db54d3cd480671fb0767c60680ad3
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44509592"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a><span data-ttu-id="1fb85-102">Zapisnici nadzora sustava SharePoint i OneDrive</span><span class="sxs-lookup"><span data-stu-id="1fb85-102">SharePoint and OneDrive audit logs</span></span>

## <a name="sharepoint-classic-audit-logs"></a><span data-ttu-id="1fb85-103">Klasični zapisnici nadzora sustava SharePoint</span><span class="sxs-lookup"><span data-stu-id="1fb85-103">SharePoint classic Audit logs</span></span>

<span data-ttu-id="1fb85-104">Naslijeđeno nadziranje SPO-a migrirao je u Objedinjeni zapisnik nadzora (UAL).</span><span class="sxs-lookup"><span data-stu-id="1fb85-104">SPO legacy auditing was migrated to Unified Audit Log (UAL).</span></span> <span data-ttu-id="1fb85-105">Sva SPO naslijeđena revizijska izvješća sada će se pokretati putem UAL-a, a naslijeđeni revizijski signali migrirali su u UAL.</span><span class="sxs-lookup"><span data-stu-id="1fb85-105">All SPO legacy audit reports will now be powered through UAL, and the legacy audit signals have been migrated to UAL.</span></span>

<span data-ttu-id="1fb85-106">Ključne promjene:</span><span class="sxs-lookup"><span data-stu-id="1fb85-106">Key changes:</span></span>

* <span data-ttu-id="1fb85-107">Podrezivanje nije dostupno kao mogućnost.</span><span class="sxs-lookup"><span data-stu-id="1fb85-107">Trimming is NOT available as a capability.</span></span>
* <span data-ttu-id="1fb85-108">Odabir određenih događaja za reviziju NIJE dostupan.</span><span class="sxs-lookup"><span data-stu-id="1fb85-108">Choosing specific events to audit is NOT available.</span></span> <span data-ttu-id="1fb85-109">Pogledajte [ovaj dokument](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance) za potpuni popis revidiranih događaja dostupnih prema zadanim postavkama.</span><span class="sxs-lookup"><span data-stu-id="1fb85-109">Refer to [this document](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance) for a complete list of audited events available by default.</span></span>
* <span data-ttu-id="1fb85-110">Mogućnost **Lokacija** u **odjeljku Prilagođena izvješća** nije dostupna.</span><span class="sxs-lookup"><span data-stu-id="1fb85-110">The **Location** option under **Customized reports** is NOT available.</span></span>
* <span data-ttu-id="1fb85-111">Mogućnost **Otvaranje ili preuzimanje događaja dokumenata** NIJE dostupna.</span><span class="sxs-lookup"><span data-stu-id="1fb85-111">The **Opening or downloading documents** events option is NOT available.</span></span>

[<span data-ttu-id="1fb85-112">Konfiguriranje postavki nadzora za zbirku web-mjesta</span><span class="sxs-lookup"><span data-stu-id="1fb85-112">Configure Audit settings for a site collection</span></span>](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a><span data-ttu-id="1fb85-113">Zapisnici sustava SharePoint i OneDrive modernog objedinjenog nadzora iz usklađenosti</span><span class="sxs-lookup"><span data-stu-id="1fb85-113">SharePoint and OneDrive Modern Unified Audit logs from compliance</span></span>

* [<span data-ttu-id="1fb85-114">Uključivanje/isključivanje objedinjenog zapisivanja nadzora</span><span class="sxs-lookup"><span data-stu-id="1fb85-114">Turn on/off Unified Audit Logging</span></span>](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off) 

<span data-ttu-id="1fb85-115">U sustavu SharePoint ili OneDrive nije potrebna dodatna konfiguracija.</span><span class="sxs-lookup"><span data-stu-id="1fb85-115">No additional configuration is required within SharePoint or OneDrive.</span></span>

<span data-ttu-id="1fb85-116">Koristite pretraživanje zapisivanja nadzora da biste provjerili aktivnost datoteka, mapa, korisnika, dozvola:</span><span class="sxs-lookup"><span data-stu-id="1fb85-116">Use audit logging search to check activity of the file(s), folder(s), user(s), permissions:</span></span>

* [<span data-ttu-id="1fb85-117">Aktivnosti datoteka i stranica</span><span class="sxs-lookup"><span data-stu-id="1fb85-117">File and page activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)
* [<span data-ttu-id="1fb85-118">Aktivnosti mape</span><span class="sxs-lookup"><span data-stu-id="1fb85-118">Folder activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [<span data-ttu-id="1fb85-119">Dijeljenje i pristup aktivnosti zahtjeva</span><span class="sxs-lookup"><span data-stu-id="1fb85-119">Sharing and access request activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [<span data-ttu-id="1fb85-120">Aktivnosti sinkronizacije</span><span class="sxs-lookup"><span data-stu-id="1fb85-120">Synchronization activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [<span data-ttu-id="1fb85-121">Aktivnosti administracije web-mjesta</span><span class="sxs-lookup"><span data-stu-id="1fb85-121">Site administration activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

<span data-ttu-id="1fb85-122">Dodatne informacije o dohvaćanju tih događaja potražite [u odjeljku Pretraživanje zapisnika nadzora](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span><span class="sxs-lookup"><span data-stu-id="1fb85-122">For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>
