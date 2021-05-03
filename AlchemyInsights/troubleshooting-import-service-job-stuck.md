---
title: Otklanjanje poteškoća s zaglavljenim poslom servisa za uvoz
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/27/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7907"
- "9003046"
ms.openlocfilehash: 987383037f843d347477c0becc859c663736a676
ms.sourcegitcommit: c977687a7dd03288a9ba396cf2a48ea384d72634
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52124810"
---
# <a name="troubleshooting-import-service-job-stuck"></a><span data-ttu-id="958c7-102">Otklanjanje poteškoća s zaglavljenim poslom servisa za uvoz</span><span class="sxs-lookup"><span data-stu-id="958c7-102">Troubleshooting Import Service job stuck</span></span>

<span data-ttu-id="958c7-103">Ako nailazite na probleme s zaglavljenim ili neuspješnim zadacima servisa uvoza, pregledajte i pokušajte sljedeće:</span><span class="sxs-lookup"><span data-stu-id="958c7-103">If you are experiencing issues with Import service jobs stuck or failing, examine and try the following:</span></span>

- <span data-ttu-id="958c7-104">Pregledajte veličinu PST datoteke.</span><span class="sxs-lookup"><span data-stu-id="958c7-104">Review the size of of the PST file.</span></span> <span data-ttu-id="958c7-105">Maksimalna preporučena veličina PST datoteke za uvoz je 20 GB.</span><span class="sxs-lookup"><span data-stu-id="958c7-105">The maximum recommended size of a PST file for import is 20GB.</span></span>

- <span data-ttu-id="958c7-106">Ako sumnjate da ste preskočili stavke zbog oštećenja, pokrenite Scanpst.exe dijagnosticiranje i ispravljanje pogrešaka u PST datotekama.</span><span class="sxs-lookup"><span data-stu-id="958c7-106">If you suspect skipped items due to corruption, run Scanpst.exe to diagnose and fix errors in PST files.</span></span>

- <span data-ttu-id="958c7-107">Ako vam se tijekom uvoza prikazuje pogreška "MapiExceptionShutoffQuotaExceeded", provjerite ima li ciljni poštanski sandučić dovoljan kapacitet za uvoz željenih PST datoteka.</span><span class="sxs-lookup"><span data-stu-id="958c7-107">If you see a "MapiExceptionShutoffQuotaExceeded" error during import, make sure the target mailbox has sufficient capacity to import the desired PST files.</span></span>

<span data-ttu-id="958c7-108">Dodatne informacije o otklanjanju poteškoća s uvozom PST-a potražite u članku Otklanjanje [poteškoća s zadacima uvoza PST-a.](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job)</span><span class="sxs-lookup"><span data-stu-id="958c7-108">For more information on troubleshooting PST import job issues, see [Troubleshoot issues with PST import jobs](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job).</span></span>

<span data-ttu-id="958c7-109">Informacije o ispravljanju problema prilikom uvoza PSTs-ova u Outlook potražite u članku Rješavanje problema s [uvozom .pst Outlook (microsoft.com)](https://support.microsoft.com/topic/fix-problems-importing-an-outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e?ui=en-us&rs=en-us&ad=us).</span><span class="sxs-lookup"><span data-stu-id="958c7-109">For information about how to fix issues when importing PSTs into Outlook, see [Fix problems importing an Outlook .pst file (microsoft.com)](https://support.microsoft.com/topic/fix-problems-importing-an-outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e?ui=en-us&rs=en-us&ad=us).</span></span>