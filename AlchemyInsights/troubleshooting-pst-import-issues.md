---
title: Otklanjanje poteškoća s uvozom PST-a
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1800027"
- "1225"
ms.openlocfilehash: 58fdd509fae5e87bf5ae72db5d8926c4367cdd64
ms.sourcegitcommit: 87aa36e3ff4835efb120a320c5169bfa77199ec4
ms.translationtype: HT
ms.contentlocale: hr-HR
ms.lasthandoff: 05/01/2020
ms.locfileid: "43991152"
---
# <a name="troubleshooting-pst-import-issues"></a><span data-ttu-id="d7361-102">Otklanjanje poteškoća s uvozom PST-a</span><span class="sxs-lookup"><span data-stu-id="d7361-102">Troubleshooting PST import issues</span></span>

- <span data-ttu-id="d7361-103">Ako uvozite unutar vlastitog klijenta programa Outlook, pročitajte odjeljak [Rješavanje problema prilikom uvoza .pst datoteke programa Outlook](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).</span><span class="sxs-lookup"><span data-stu-id="d7361-103">If you are importing within the Outlook client itself, please see [Fix problems importing an Outlook .pst file](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).</span></span>

- <span data-ttu-id="d7361-104">Ako koristite servis za uvoz koji je zaglavljen, imajte na umu da svaka PST datoteka koju prenosite na mjesto pohrane Azure ne bi smjela biti veća od 20 GB.</span><span class="sxs-lookup"><span data-stu-id="d7361-104">If you are using Import Service and it is stuck, please note that each PST file that you upload to the Azure Storage location should be no larger than 20 GB.</span></span> <span data-ttu-id="d7361-105">PST datoteke veće od 20 GB mogu utjecati na izvođenje postupka uvoza u PST-u.</span><span class="sxs-lookup"><span data-stu-id="d7361-105">PST files larger than 20 GB may impact the performance of the PST import process.</span></span>

- <span data-ttu-id="d7361-106">Ako želite provjeriti stanje određenog zadatka uvoza, možete koristiti [Get-MailboxImportRequest-naziv serije](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest).</span><span class="sxs-lookup"><span data-stu-id="d7361-106">If you want to verify the status of a specific Import job, you can use [Get-MailboxImportRequest -batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest).</span></span>

- <span data-ttu-id="d7361-107">Da biste saznali više o servisu za uvoz, pročitajte [Pregled uvoza PST datoteka u tvrtki ili ustanovi](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="d7361-107">For full details on the import service, please see [Overview of importing your organization's PST files](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide).</span></span>
