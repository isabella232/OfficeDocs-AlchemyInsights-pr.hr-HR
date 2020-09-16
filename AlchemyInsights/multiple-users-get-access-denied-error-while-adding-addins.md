---
title: Prilikom dodavanja dodataka u programu Outlook više je korisnika došlo do odbijanja programa Access
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
ms.openlocfilehash: 611a4df473458abc0ab0c65442f2141763f7b868
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47724355"
---
# <a name="multiple-users-get-access-denied-error-while-adding-add-ins-in-outlook"></a>Prilikom dodavanja dodataka u programu Outlook više je korisnika došlo do odbijanja programa Access

Možete odrediti koji administratori u tvrtki ili ustanovi imaju dozvole za instalaciju i upravljanje dodacima za Outlook. Možete i odrediti koje korisnike u tvrtki ili ustanovi imaju dozvolu za instalaciju i upravljanje dodacima za vlastitu upotrebu.

Pojedinosti potražite u članku [određivanje administratora i korisnika koji mogu instalirati dodatke za Outlook i upravljati njima](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).

Da biste potvrdili da ste uspješno dodijelili dozvole za korisnika, zamijenite <Role Name> naziv uloge koju želite provjeriti, a zatim pokrenite sljedeću naredbu u komponenti Exchange Online PowerShell:

Get-Managementroledodjeljivanje-uloga " <Role Name> "-geteffectiveusers

U ovom se primjeru prikazuje kako potvrditi kome ste dodijelili dozvole za instalaciju dodataka iz trgovine sustava Office za tvrtku ili ustanovu.

PowerShell

-Uloga "aplikacije tvrtke org Marketplace"-GetEffectiveUsers

U rezultatima Get-Managelmentroledodjela Pregledajte unose u stupcu efektivni korisnici.

Detaljne informacije o sintaksi i parametrima potražite [u članku Get-Managelmentrolezadatak](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment).
 