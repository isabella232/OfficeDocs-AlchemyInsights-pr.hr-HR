---
title: Jedan korisnik koji ne vidi dodatke u programu Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.openlocfilehash: 1f547c3f593b3256bd44f518aacbc36ed1c4c848
ms.sourcegitcommit: a05276bd623466ad211e1f8d9f0c616672dd3640
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 07/16/2020
ms.locfileid: "45197767"
---
# <a name="single-user-not-seeing-add-ins-in-outlook"></a>Jedan korisnik koji ne vidi dodatke u programu Outlook

Korisnik može biti dio uloge koja nema ispravan parametar AppsForOfficeEnabled. Pokrenite ovaj cmdlet da biste saznali je li ispravna uloga povezana s korisnikom:

Get-ManagementRoleAssignment -RoleAssignee user@domain.com-Delegiranje $false | Oblikovanje-tablica -Auto uloga,RoleAssigneeName,RoleAssigneeType

Dodatne informacije [potražite u odjeljku Određivanje administratora i korisnika koji mogu instalirati dodatke za Outlook i upravljati njima](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).
