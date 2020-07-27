---
title: Više korisnika dobiva pogrešku odbijen pristup prilikom dodavanja dodataka u programu Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5892"
- "6700008"
ms.openlocfilehash: 624d880c535b7d8888b676ff23c774c6d138a75a
ms.sourcegitcommit: 07e56267dedfc4cec1143072c791670cbf81186b
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 07/24/2020
ms.locfileid: "45423360"
---
# <a name="multiple-users-get-access-denied-error-while-adding-add-ins-in-outlook"></a>Više korisnika dobiva pogrešku odbijen pristup prilikom dodavanja dodataka u programu Outlook

Možete odrediti koji administratori u tvrtki ili ustanovi imaju dozvole za instalaciju dodataka i upravljanje njima za Outlook. Možete odrediti i koji korisnici u vašoj tvrtki ili ustanovi imaju dozvolu za instalaciju dodataka i upravljanje njima za vlastitu upotrebu.

Pojedinosti potražite [u članku Određivanje administratora i korisnika koji mogu instalirati dodatke za Outlook i upravljati njima](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).

Da biste provjerili jeste li uspješno dodijelili dozvole korisniku, <Role Name> zamijenite nazivom uloge koju želite provjeriti i pokrenite sljedeću naredbu u dodatku PowerShell sustava Exchange Online:

Get-ManagementRoleAssignment -Uloga " <Role Name> " -GetEffectiveUsers

Ovaj primjer pokazuje kako provjeriti kome ste dodijelili dozvole za instalaciju dodataka iz Office trgovine za tvrtku ili ustanovu.

Powershell

-Uloga "Org Marketplace Apps" -GetEffectiveUsers

U rezultatima, Get-ManagementRoleAssignment, pregledajte stavke u stupcu Učinkoviti korisnici.

Detaljne informacije o sintaksi i parametrima [potražite u odjeljku Get-ManagementRoleAssignment](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment).
 