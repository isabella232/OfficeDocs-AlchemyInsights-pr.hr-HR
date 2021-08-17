---
title: Dozvole za kalendar
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800009"
- "611"
ms.openlocfilehash: 4bf7680a422f096401f0a87bccd1b8dd11f4489f882bcc06864e37d6a248438c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54046096"
---
# <a name="calendar-permissions"></a>Dozvole za kalendar

Korisnici mogu promijeniti vlastite dozvole za kalendar Outlook na webu ili drugim klijentima, ali kao administrator možda ćete morati i istražiti.  
Cmdlet Exchange komponente PowerShell pokazat će vam dozvolu za korisnikov kalendar:

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

Da biste vidjeli dodatne informacije, pogledajte sljedeće:

- [Get-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [Set-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [Add-MailboxFolderPermission](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

Dozvole kalendara koriste se za zajedničko korištenje kalendara da biste vidjeli dodatne informacije o zajedničkom korištenju kalendara Outlook, pogledajte ove članke:

- [Zajedničko korištenje kalendara programa Outlook s drugim osobama](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [Zajedničko korištenje kalendara Outlook na webu za tvrtke](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

Da biste otklonili poteškoće s dozvolom za [kalendar, možete koristiti pomoćnik za podršku i oporavak alat.](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f)