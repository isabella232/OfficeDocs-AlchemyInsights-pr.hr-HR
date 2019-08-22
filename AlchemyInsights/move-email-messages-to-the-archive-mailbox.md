---
title: Premještanje poruka e-pošte arhiva poštanskog sandučića
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: ce52df446fc4c23c06476e8836ade6a6810d158f
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36548995"
---
# <a name="move-email-to-the-archive-mailbox"></a>Premjesti e-pošta poštanski sandučić arhiva

1. Potvrdite da je **arhiviranje poštanski sandučić** je omogućeno. Ako nije, slijedite korake u [ovom članku](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) da biste omogućili arhiva poštanski sandučić.

2. Za arhiviranje poruka automatski u poštanski sandučić arhiva zadržavanja oznaka s akcijom **premjestiti za arhiviranje** mora biti postavljen da **automatski primijeniti oznaka cijeli sandučić (zadano)**. Ovdje koristite korake za stvaranje oznaka: [arhiva zadana oznaka](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fdocs.microsoft.com%2Fen-us%2Foffice365%2Fsecuritycompliance%2Fset-up-an-archive-and-deletion-policy-for-mailboxes%23create-a-custom-archive-default-policy-tag&data=04%7C01%7Cstephow%40microsoft.com%7C89934e16dbd84ebdef6708d6b319b348%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636893320296576506%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C-1&sdata=UibWi%2BtrO3ITZ6iF%2FtKQj5JyxzEb9Mu9frBJPT6FNFI%3D&reserved=0).

3. Dalje, dodajte oznaku **arhiva** pravila zadržavanja. U centru za administraciju Exchange odaberite **Pravila zadržavanja** > dodavanje **Premještanje arhiva oznaku** > pravila **spremiti**.

4. Sada [dodijeliti pravila zadržavanja](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) poštanski sandučić određenog korisnika. Ista pravila primijenit će se na **primarni** i poštanski sandučić **arhiva** .

Možda će biti potrebno da biste prisilili na upravljana mapa pomoćnika (MFA) za pokretanje i primijeniti nove postavke u korisnički poštanski sandučić. Pokrenite sljedeću naredbu tijekom [povezani EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) za pokretanje upravljanih Pomoćnik za mape za određene poštanski sandučić:
  
Start ManagedFolderAssistant-identitet<name of the mailbox>

Za dodatne informacije o postavljanju pravila arhiviranja pogledajte [Postavljanje arhiva i brisanje pravila za poštanske sandučiće](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  