---
title: Dozvole kalendara
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800009"
- "611"
ms.openlocfilehash: 78f27014c60badc801212177dd455ef2a0de5a9e
ms.sourcegitcommit: 722e9a0ed058cb1eab2dd053be2418b60f7d4aac
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/23/2020
ms.locfileid: "44862038"
---
# <a name="calendar-permissions"></a>Dozvole kalendara

Korisnici mogu promijeniti vlastite dozvole kalendara s programom Outlook na webu ili drugim klijentima, ali kao administrator možda ćete morati istražiti.  
S cmdletom Exchange PowerShell prikazat će vam dozvolu za korisnikov kalendar:

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

Dodatne informacije potražite u sljedećim informacijama:

- [Get-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [Set-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [Dodatak-MailboxFolderPermission](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

Dozvole kalendara koriste se u zajedničkom korištenju kalendara da biste vidjeli više informacija o zajedničkom korištenju kalendara programa Outlook, pogledajte ove članke:

- [Zajedničko korištenje kalendara programa Outlook s drugim osobama](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [Zajedničko korištenje kalendara u programu Outlook na webu za tvrtke](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

Da biste otklonili poteškoće s dozvolom kalendara, možete koristiti alat [pomoćnika za podršku i oporavak.](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f)