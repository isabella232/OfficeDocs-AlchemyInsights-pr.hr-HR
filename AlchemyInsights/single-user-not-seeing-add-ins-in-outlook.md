---
title: Jedan korisnik koji ne prikazuje dodatke u programu Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.openlocfilehash: 8c99b443a2d83f3ac24362d63cd6363a66a81393
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47719657"
---
# <a name="single-user-not-seeing-add-ins-in-outlook"></a>Jedan korisnik koji ne prikazuje dodatke u programu Outlook

Korisnik može biti dio uloge koja nema ispravni parametar AppsForOfficeEnabled. Pokrenite ovaj cmdlet da biste saznali je li ispravna uloga povezana s korisnikom:

Get-Managelmentroledodjeljivanje-Rojesignee user@domain.com-deleating $false | Format-table-auto uloga, Rojesigneename, Rojesigneetype

Dodatne informacije potražite u članku [određivanje administratora i korisnika koji mogu instalirati dodatke za Outlook i upravljati njima](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).
