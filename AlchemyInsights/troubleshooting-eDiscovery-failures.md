---
title: 1490 – otklanjanje poteškoća – Rediscovery – pogreške
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1490"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: ff28f96d64ec14980e9a47b630246b394faf4610
ms.sourcegitcommit: fbe6925797cab0b38172386f1b059dc122e452a4
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/25/2020
ms.locfileid: "48277817"
---
# <a name="troubleshoot-content-search-errors"></a><span data-ttu-id="df3d7-102">Otklanjanje poteškoća s pretraživanjem sadržaja</span><span class="sxs-lookup"><span data-stu-id="df3d7-102">Troubleshoot Content Search errors</span></span>

<span data-ttu-id="df3d7-103">Nailazite li na probleme s pretraživanjem sadržaja ili neuspjehom prilikom izvoza rezultata pretraživanja?</span><span class="sxs-lookup"><span data-stu-id="df3d7-103">Are you experiencing problems with Content Search or getting failures when you export search results?</span></span>

<span data-ttu-id="df3d7-104">Na primjer, primate li sljedeće prilikom izvođenja pretraživanja?</span><span class="sxs-lookup"><span data-stu-id="df3d7-104">For example, are you receiving the following when running searches?</span></span>

- <span data-ttu-id="df3d7-105">CS008 ili CS012 pogreške</span><span class="sxs-lookup"><span data-stu-id="df3d7-105">CS008 or CS012 errors</span></span>

- <span data-ttu-id="df3d7-106">Pogreške zauzetosti poslužitelja/prekoračenja ograničenja</span><span class="sxs-lookup"><span data-stu-id="df3d7-106">Server busy/timeout errors</span></span>

- <span data-ttu-id="df3d7-107">Došlo je do pogreške u aplikaciji</span><span class="sxs-lookup"><span data-stu-id="df3d7-107">Application error occurred</span></span>

<span data-ttu-id="df3d7-108">Ako pretražujete ili izvozite rezultate iz velikog broja poštanskih sandučića (iznad 100.000 poštanskih sandučića), dobivate li pogreške u izvozu?</span><span class="sxs-lookup"><span data-stu-id="df3d7-108">Or when searching or exporting results from a large number of mailboxes (over 100,000 mailboxes), are you getting export errors?</span></span>

<span data-ttu-id="df3d7-109">Da biste pronašli ove vrste pogrešaka, pokušajte pokušati potražiti mjesta sadržaja koja nisu uspjela.</span><span class="sxs-lookup"><span data-stu-id="df3d7-109">For these types of errors, retry the search for the content locations that have failed.</span></span> <span data-ttu-id="df3d7-110">Dodatne informacije potražite u  [ovom članku](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) .</span><span class="sxs-lookup"><span data-stu-id="df3d7-110">See  [this article](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) for more information.</span></span>

<span data-ttu-id="df3d7-111">Ako izvozite više od 100K poštanskih sandučića, morat ćete koristiti sljedeću PowerShell da biste preuzeli rezultate izvoza:  [Izvoz rezultata iz više od 100k poštanskih sandučića](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span><span class="sxs-lookup"><span data-stu-id="df3d7-111">If you are exporting more than 100K mailboxes, you will need to use the following Powershell to download the Export results:  [Exporting results from more than 100K mailboxes](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span></span>
