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
ms.openlocfilehash: af5b3c76b82db13bc89c917247e41fa1d8779b68
ms.sourcegitcommit: d5bf97a0bf0547f36b6da9684ce9f16a13a7749e
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/20/2019
ms.locfileid: "37068015"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a><span data-ttu-id="46690-102">Zapisnici revizije sustava SharePoint i OneDrive</span><span class="sxs-lookup"><span data-stu-id="46690-102">SharePoint and OneDrive audit logs</span></span>

<span data-ttu-id="46690-103">**Dnevnika programa SharePoint i OneDrive moderne jedinstvene revizije iz sukladnosti**</span><span class="sxs-lookup"><span data-stu-id="46690-103">**SharePoint and OneDrive Modern Unified Audit logs from compliance**</span></span>

- [<span data-ttu-id="46690-104">Uključi/isključi objedinjeno bilježenje nadzora</span><span class="sxs-lookup"><span data-stu-id="46690-104">Turn on/off Unified Audit Logging</span></span>](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off) 

<span data-ttu-id="46690-105">U sustavu SharePoint ili servisu OneDrive nije potrebna dodatna konfiguracija.</span><span class="sxs-lookup"><span data-stu-id="46690-105">No additional configuration is required within SharePoint or OneDrive.</span></span>

- <span data-ttu-id="46690-106">Korištenje pretraživanja zapisnika nadzora za provjeru aktivnosti datoteka, mapa, korisnika, dozvola:</span><span class="sxs-lookup"><span data-stu-id="46690-106">Use audit logging search to check activity of the file(s), folder(s), user(s), permissions:</span></span>

    - [<span data-ttu-id="46690-107">Aktivnosti datoteka i stranica</span><span class="sxs-lookup"><span data-stu-id="46690-107">File and page activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)
    - [<span data-ttu-id="46690-108">Aktivnosti mape</span><span class="sxs-lookup"><span data-stu-id="46690-108">Folder activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
    - [<span data-ttu-id="46690-109">Korištenje aktivnosti zahtjeva za dijeljenje i pristup</span><span class="sxs-lookup"><span data-stu-id="46690-109">Sharing and access request activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
    - [<span data-ttu-id="46690-110">Aktivnosti sinkronizacije</span><span class="sxs-lookup"><span data-stu-id="46690-110">Synchronization activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
    - [<span data-ttu-id="46690-111">Aktivnosti administracije web-mjesta</span><span class="sxs-lookup"><span data-stu-id="46690-111">Site administration activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)
- <span data-ttu-id="46690-112">Dodatne informacije o dohvat tih događaja potražite [u pretraživanju zapisnika nadzora](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span><span class="sxs-lookup"><span data-stu-id="46690-112">For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>

<span data-ttu-id="46690-113">**SharePoint klasični dnevnici nadzora**</span><span class="sxs-lookup"><span data-stu-id="46690-113">**SharePoint classic Audit logs**</span></span>

<span data-ttu-id="46690-114">Migrirati SPO naslijeđene revizije na Unified nadzorni zapisnik (UAL).</span><span class="sxs-lookup"><span data-stu-id="46690-114">We migrated SPO legacy auditing to Unified Audit Log (UAL).</span></span> <span data-ttu-id="46690-115">To u biti znači da će se sva bila koja su naslijeđena revizijska izvješća sada moći prenositi preko UAL-a, a naslijeđeni revizijski signali su premješteni u UAL.</span><span class="sxs-lookup"><span data-stu-id="46690-115">This essentially means that all SPO legacy audit reports will now be powered through UAL, and the legacy audit signals have been migrated to UAL.</span></span>

<span data-ttu-id="46690-116">Ključne promjene:</span><span class="sxs-lookup"><span data-stu-id="46690-116">Key changes:</span></span>

- <span data-ttu-id="46690-117">Skraćivanje kao mogućnost nije dostupno.</span><span class="sxs-lookup"><span data-stu-id="46690-117">Trimming as a capability is NOT available.</span></span>
- <span data-ttu-id="46690-118">Odjeljak u kojem odaberete specifične događaje za reviziju nije dostupan.</span><span class="sxs-lookup"><span data-stu-id="46690-118">The section where you choose specific events to audit is NOT available.</span></span> <span data-ttu-id="46690-119">Molimo pogledajte [ovaj dokument](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) za potpuni popis revidiranih događaja dostupnih prema zadanim postavkama.</span><span class="sxs-lookup"><span data-stu-id="46690-119">Please refer to [this document](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) for a complete list of audited events available by default.</span></span>
- <span data-ttu-id="46690-120">Opcija "lokacija" pod **prilagođenim izvješćima** nije dostupna.</span><span class="sxs-lookup"><span data-stu-id="46690-120">The "Location" option under **Customized reports** is NOT available.</span></span> 
- <span data-ttu-id="46690-121">Događaji "otvaranje ili preuzimanje dokumenata" nisu dostupni.</span><span class="sxs-lookup"><span data-stu-id="46690-121">“Opening or downloading documents” events is NOT available.</span></span> 

