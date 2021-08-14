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
ms.openlocfilehash: 549af832f9c58db1cdd8fbe80b8b5bd2aba9bd937f33116806a9391cbc9a5d4c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53972411"
---
# <a name="troubleshooting-pst-import-issues"></a>Otklanjanje poteškoća s uvozom PST-a

- Ako uvozite unutar samog klijenta Outlook, pogledajte rješavanje [problema prilikom uvoza .pst Outlook .pst datoteke.](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e)

- Ako koristite servis za uvoz i zapela je, imajte na umu da svaka PST datoteka koju prenesete na mjesto za pohranu na servisu Azure ne smije biti veća od 20 GB. PST datoteke veće od 20 GB mogu utjecati na performanse postupka uvoza PST-a. Dodatne informacije o otklanjanju poteškoća sa zapelim zadacima [potražite u članku Problemi koji utječu na zadatke uvoza PST-a](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job).

- Ako želite provjeriti status određenog posla uvoza, koristite [Get-MailboxImportRequest -batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest).

- Potpune pojedinosti o servisu za uvoz potražite u članku Pregled uvoza PST datoteka [tvrtke ili ustanove.](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide)
