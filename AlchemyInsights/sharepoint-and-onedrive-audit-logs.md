---
title: Klasični Izvještaji zapisnika nadzora sustava SharePoint
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: daf79f8d75ccdff8ad54f0f307648a5832a6bb71
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47662200"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a><span data-ttu-id="12e0d-102">Zapisnici nadzora sustava SharePoint i servisa OneDrive</span><span class="sxs-lookup"><span data-stu-id="12e0d-102">SharePoint and OneDrive audit logs</span></span>

## <a name="sharepoint-classic-audit-logs"></a><span data-ttu-id="12e0d-103">Zapisi o reviziji sustava SharePoint Classic</span><span class="sxs-lookup"><span data-stu-id="12e0d-103">SharePoint classic Audit logs</span></span>

<span data-ttu-id="12e0d-104">SPO nasljeđeni nadzor migrirao je u jedinstveni zapisnik nadzora (UAL).</span><span class="sxs-lookup"><span data-stu-id="12e0d-104">SPO legacy auditing was migrated to Unified Audit Log (UAL).</span></span> <span data-ttu-id="12e0d-105">Sva će se SPO naslijeđena izvješća o reviziji sada powered putem UAL-a, a nasljeđene revizijske signale migrirali su u UAL.</span><span class="sxs-lookup"><span data-stu-id="12e0d-105">All SPO legacy audit reports will now be powered through UAL, and the legacy audit signals have been migrated to UAL.</span></span>

<span data-ttu-id="12e0d-106">Ključne promjene:</span><span class="sxs-lookup"><span data-stu-id="12e0d-106">Key changes:</span></span>

* <span data-ttu-id="12e0d-107">Podrezivanje nije dostupno kao mogućnost.</span><span class="sxs-lookup"><span data-stu-id="12e0d-107">Trimming is NOT available as a capability.</span></span>
* <span data-ttu-id="12e0d-108">Odabir određenih događaja za reviziju nije dostupan.</span><span class="sxs-lookup"><span data-stu-id="12e0d-108">Choosing specific events to audit is NOT available.</span></span> <span data-ttu-id="12e0d-109">Pogledajte [ovaj dokument](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance) radi potpunog popisa događaja koji se revidiraju na raspolaganju po zadanom.</span><span class="sxs-lookup"><span data-stu-id="12e0d-109">Refer to [this document](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance) for a complete list of audited events available by default.</span></span>
* <span data-ttu-id="12e0d-110">Mogućnost **mjesta** u odjeljku **Prilagođena izvješća** nije dostupna.</span><span class="sxs-lookup"><span data-stu-id="12e0d-110">The **Location** option under **Customized reports** is NOT available.</span></span>
* <span data-ttu-id="12e0d-111">Mogućnost **otvaranja ili preuzimanja dokumenata** nije dostupna.</span><span class="sxs-lookup"><span data-stu-id="12e0d-111">The **Opening or downloading documents** events option is NOT available.</span></span>

[<span data-ttu-id="12e0d-112">Konfiguriranje postavki nadzora za zbirku web-mjesta</span><span class="sxs-lookup"><span data-stu-id="12e0d-112">Configure Audit settings for a site collection</span></span>](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a><span data-ttu-id="12e0d-113">Moderno objedinjene zapisnike nadzora sustava SharePoint i OneDrive iz usklađenosti</span><span class="sxs-lookup"><span data-stu-id="12e0d-113">SharePoint and OneDrive Modern Unified Audit logs from compliance</span></span>

* [<span data-ttu-id="12e0d-114">Uključivanje/isključivanje objedinjenog nadzornog zapisivanja</span><span class="sxs-lookup"><span data-stu-id="12e0d-114">Turn on/off Unified Audit Logging</span></span>](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off) 

<span data-ttu-id="12e0d-115">U sustavu SharePoint ili na servisu OneDrive nije potrebna nijedna dodatna konfiguracija.</span><span class="sxs-lookup"><span data-stu-id="12e0d-115">No additional configuration is required within SharePoint or OneDrive.</span></span>

<span data-ttu-id="12e0d-116">Pomoću pretraživanja zapisnika nadzora potražite aktivnost datoteka, mapa, korisnika, dozvola:</span><span class="sxs-lookup"><span data-stu-id="12e0d-116">Use audit logging search to check activity of the file(s), folder(s), user(s), permissions:</span></span>

* [<span data-ttu-id="12e0d-117">Aktivnosti datoteka i stranica</span><span class="sxs-lookup"><span data-stu-id="12e0d-117">File and page activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)
* [<span data-ttu-id="12e0d-118">Aktivnosti u mapama</span><span class="sxs-lookup"><span data-stu-id="12e0d-118">Folder activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [<span data-ttu-id="12e0d-119">Zajedničko korištenje i pristup aktivnostima zahtjeva</span><span class="sxs-lookup"><span data-stu-id="12e0d-119">Sharing and access request activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [<span data-ttu-id="12e0d-120">Aktivnosti sinkronizacije</span><span class="sxs-lookup"><span data-stu-id="12e0d-120">Synchronization activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [<span data-ttu-id="12e0d-121">Aktivnosti administracije web-mjesta</span><span class="sxs-lookup"><span data-stu-id="12e0d-121">Site administration activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

<span data-ttu-id="12e0d-122">Dodatne informacije o dohvat tih događaja potražite [u članku pretraživanje zapisnika nadzora](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span><span class="sxs-lookup"><span data-stu-id="12e0d-122">For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>
