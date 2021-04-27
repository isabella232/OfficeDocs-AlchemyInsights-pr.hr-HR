---
title: Otklanjanje poteškoća s uvozom PST-a
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1800027"
- "1225"
ms.openlocfilehash: 5065b9895954371e4298c98e8aadb67ba8f140fd
ms.sourcegitcommit: c977687a7dd03288a9ba396cf2a48ea384d72634
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52059807"
---
# <a name="troubleshooting-pst-import-issues"></a><span data-ttu-id="e4144-102">Otklanjanje poteškoća s uvozom PST-a</span><span class="sxs-lookup"><span data-stu-id="e4144-102">Troubleshooting PST import issues</span></span>

- <span data-ttu-id="e4144-103">Ako uvozite unutar samog klijenta programa Outlook, pogledajte rješavanje [problema prilikom uvoza .pst datoteke programa Outlook](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).</span><span class="sxs-lookup"><span data-stu-id="e4144-103">If you are importing within the Outlook client itself, see [Fix problems importing an Outlook .pst file](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).</span></span>

- <span data-ttu-id="e4144-104">Ako koristite servis za uvoz i zapela je, imajte na umu da svaka PST datoteka koju prenesete na mjesto za pohranu na servisu Azure ne smije biti veća od 20 GB.</span><span class="sxs-lookup"><span data-stu-id="e4144-104">If you are using Import Service and it's stuck, note that each PST file that you upload to the Azure Storage location should be no larger than 20GB.</span></span> <span data-ttu-id="e4144-105">PST datoteke veće od 20 GB mogu utjecati na performanse postupka uvoza PST-a.</span><span class="sxs-lookup"><span data-stu-id="e4144-105">PST files larger than 20GB may impact the performance of the PST import process.</span></span> <span data-ttu-id="e4144-106">Dodatne informacije o otklanjanju poteškoća sa zapelim zadacima [potražite u članku Problemi koji utječu na zadatke uvoza PST-a](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job).</span><span class="sxs-lookup"><span data-stu-id="e4144-106">For more information troubleshooting stuck jobs, see [Issues that affect PST import jobs](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job).</span></span>

- <span data-ttu-id="e4144-107">Ako želite provjeriti status određenog posla uvoza, koristite [Get-MailboxImportRequest -batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest).</span><span class="sxs-lookup"><span data-stu-id="e4144-107">If you want to verify the status of a specific Import job, use [Get-MailboxImportRequest -batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest).</span></span>

- <span data-ttu-id="e4144-108">Potpune pojedinosti o servisu za uvoz potražite u članku Pregled uvoza PST datoteka [tvrtke ili ustanove.](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="e4144-108">For full details on the import service, see [Overview of importing your organization's PST files](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide).</span></span>
