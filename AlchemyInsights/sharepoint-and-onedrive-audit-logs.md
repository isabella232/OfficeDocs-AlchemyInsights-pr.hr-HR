---
title: Klasična izvješća evidencije nadzornih zapisnika sustava SharePoint
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: be95034bea3c58a4fde96cfb0f9ba525e810758e
ms.sourcegitcommit: 24e8248b0f061a76af50bf566d7a13fc24d29d99
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 11/05/2019
ms.locfileid: "37992610"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a><span data-ttu-id="82d00-102">Zapisnici revizije sustava SharePoint i OneDrive</span><span class="sxs-lookup"><span data-stu-id="82d00-102">SharePoint and OneDrive audit logs</span></span>

## <a name="sharepoint-classic-audit-logs"></a><span data-ttu-id="82d00-103">SharePoint klasični dnevnici nadzora</span><span class="sxs-lookup"><span data-stu-id="82d00-103">SharePoint classic Audit logs</span></span>

<span data-ttu-id="82d00-104">U jedinstvenim revizijskim Evidijama (UAL).</span><span class="sxs-lookup"><span data-stu-id="82d00-104">SPO legacy auditing was migrated to Unified Audit Log (UAL).</span></span> <span data-ttu-id="82d00-105">Sva štena revizijska izvješća SPO-a sada će biti pokretana preko UAL-a, a naslijeđeni revizijski signali su premješteni u UAL.</span><span class="sxs-lookup"><span data-stu-id="82d00-105">All SPO legacy audit reports will now be powered through UAL, and the legacy audit signals have been migrated to UAL.</span></span>

<span data-ttu-id="82d00-106">Ključne promjene:</span><span class="sxs-lookup"><span data-stu-id="82d00-106">Key changes:</span></span>

* <span data-ttu-id="82d00-107">Obrezivanje nije dostupno kao mogućnost.</span><span class="sxs-lookup"><span data-stu-id="82d00-107">Trimming is NOT available as a capability.</span></span>
* <span data-ttu-id="82d00-108">Odabir specifičnih događaja za reviziju nije dostupan.</span><span class="sxs-lookup"><span data-stu-id="82d00-108">Choosing specific events to audit is NOT available.</span></span> <span data-ttu-id="82d00-109">Pogledajte [ovaj dokument](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) za potpuni popis revidiranih događaja dostupnih prema zadanim postavkama.</span><span class="sxs-lookup"><span data-stu-id="82d00-109">Refer to [this document](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) for a complete list of audited events available by default.</span></span>
* <span data-ttu-id="82d00-110">Opcija **lokacija** pod **prilagođenim izvješćima** nije dostupna.</span><span class="sxs-lookup"><span data-stu-id="82d00-110">The **Location** option under **Customized reports** is NOT available.</span></span>
* <span data-ttu-id="82d00-111">Mogućnost **otvaranja ili preuzimanja dokumenata** nije dostupna.</span><span class="sxs-lookup"><span data-stu-id="82d00-111">The **Opening or downloading documents** events option is NOT available.</span></span>

[<span data-ttu-id="82d00-112">Konfiguriranje postavki nadzora za zbirku web-mjesta</span><span class="sxs-lookup"><span data-stu-id="82d00-112">Configure Audit settings for a site collection</span></span>](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a><span data-ttu-id="82d00-113">Dnevnika programa SharePoint i OneDrive moderne jedinstvene revizije iz sukladnosti</span><span class="sxs-lookup"><span data-stu-id="82d00-113">SharePoint and OneDrive Modern Unified Audit logs from compliance</span></span>

* [<span data-ttu-id="82d00-114">Uključi/isključi objedinjeno bilježenje nadzora</span><span class="sxs-lookup"><span data-stu-id="82d00-114">Turn on/off Unified Audit Logging</span></span>](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off) 

<span data-ttu-id="82d00-115">U sustavu SharePoint ili servisu OneDrive nije potrebna dodatna konfiguracija.</span><span class="sxs-lookup"><span data-stu-id="82d00-115">No additional configuration is required within SharePoint or OneDrive.</span></span>

<span data-ttu-id="82d00-116">Korištenje pretraživanja zapisnika nadzora za provjeru aktivnosti datoteka, mapa, korisnika, dozvola:</span><span class="sxs-lookup"><span data-stu-id="82d00-116">Use audit logging search to check activity of the file(s), folder(s), user(s), permissions:</span></span>

* [<span data-ttu-id="82d00-117">Aktivnosti datoteka i stranica</span><span class="sxs-lookup"><span data-stu-id="82d00-117">File and page activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)
* [<span data-ttu-id="82d00-118">Aktivnosti mape</span><span class="sxs-lookup"><span data-stu-id="82d00-118">Folder activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [<span data-ttu-id="82d00-119">Korištenje aktivnosti zahtjeva za dijeljenje i pristup</span><span class="sxs-lookup"><span data-stu-id="82d00-119">Sharing and access request activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [<span data-ttu-id="82d00-120">Aktivnosti sinkronizacije</span><span class="sxs-lookup"><span data-stu-id="82d00-120">Synchronization activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [<span data-ttu-id="82d00-121">Aktivnosti administracije web-mjesta</span><span class="sxs-lookup"><span data-stu-id="82d00-121">Site administration activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

<span data-ttu-id="82d00-122">Dodatne informacije o dohvat tih događaja potražite [u pretraživanju zapisnika nadzora](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span><span class="sxs-lookup"><span data-stu-id="82d00-122">For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>
