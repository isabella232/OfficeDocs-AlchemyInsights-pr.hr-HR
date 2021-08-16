---
title: Prilikom dodavanja dodataka u programu Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5892"
- "6700008"
ms.openlocfilehash: 5e5f881ad72d2a0f76c8659d6b1044bf6a18464fa8d65c079e44eb1a2afd4431
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54065384"
---
# <a name="multiple-users-get-access-denied-error-while-adding-add-ins-in-outlook"></a>Prilikom dodavanja dodataka u programu Outlook

Možete odrediti koji administratori u tvrtki ili ustanovi imaju dozvole za instalaciju dodataka i upravljanje njima za Outlook. Možete odrediti i koji korisnici u tvrtki ili ustanovi imaju dozvolu za instalaciju dodataka i upravljanje njima za vlastitu upotrebu.

Detalje potražite u članku [Određivanje administratora i korisnika koji mogu instalirati](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins)dodatke i upravljati njima za Outlook .

Da biste provjerili jeste li korisniku uspješno dodijelili dozvole, zamijenite nazivom uloge koju želite potvrditi i pokrenite sljedeću <Role Name> naredbu u Exchange Online PowerShell:

Get-ManagementRoleAssignment -Role " <Role Name> " -GetEffectiveUsers

U ovom se primjeru prikazuje kako provjeriti kome ste dodijelili dozvole za instalaciju dodataka iz trgovine Office za organizaciju.

PowerShell

-Role "Org Marketplace Apps" -GetEffectiveUsers

U rezultatima, Get-ManagementRoleAssignment, pregledajte stavke u stupcu Učinkoviti korisnici.

Detaljne informacije o sintaksi i parametrima potražite u [članku Get-ManagementRoleAssignment](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment).
 