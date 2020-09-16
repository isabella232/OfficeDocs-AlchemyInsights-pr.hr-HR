---
title: Grupa šalji kao Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/19/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
ms.openlocfilehash: 51bd8a10c3da23941cc16d7ba860406f8477044a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47740143"
---
# <a name="send-as-microsoft-365-group"></a>Grupa šalji kao Microsoft 365

Možete dodijeliti dozvole Pošalji kao da biste određenim korisnicima dopustili da šalju poruke kao grupu Microsoft 365:  

1. Spojite se na PowerShell sustava Exchange Online.  

2. Izvršite sljedeću naredbu:  

    Dodavanje-RecipientPermission `<GroupName>` -trustee `<MailboxName>` -AccessRights SendAs

Dodatne informacije potražite u članku [Dopusti članovima da pošalju kao ili pošalju u ime grupe](https://docs.microsoft.com/microsoft-365/admin/create-groups/allow-members-to-send-as-or-send-on-behalf-of-group?view=o365-worldwide).