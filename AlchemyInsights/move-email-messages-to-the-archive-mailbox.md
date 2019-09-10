---
title: Premještanje poruka e-pošte u poštanski sandučić arhive
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
ms.openlocfilehash: 5592bc7d4566e3498c33bbf9488db7f46ec58842
ms.sourcegitcommit: 8864b5789d9905916039081b53530c7e6d8bc529
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/10/2019
ms.locfileid: "36822154"
---
# <a name="move-email-to-the-archive-mailbox"></a>Premještanje e-pošte u poštanski sandučić arhive

1. Provjerite je li omogućen **Poštanski sandučić arhive** . Ako ne, koristite korake u [ovom članku](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) da biste omogućili arhiviranje poštanskog sandučića.

2. Da biste automatski arhivirali poruke u poštanski sandučić arhive, oznaka zadržavanja s **premještavanjem u arhivsku** akciju mora biti postavljena da se **automatski primijeni na cijelu oznaku poštanskog sandučića (zadana)**. Pomoću koraka ovdje stvorite oznaku: [arhivirati zadanu oznaku](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).

3. Zatim u pravila zadržavanja dodajte oznaku **arhive** . U centru za administratore sustava Exchange odaberite **pravila zadržavanja** > Dodajte **oznaku Premjesti u arhivu** pravila > **Spremi**.

4. Sada [dodijelite pravila zadržavanja](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) određenom korisnikovom poštanskom sandučiću. Isto pravilo će se primijeniti i na **primarni** i **Arhiva** poštanski sandučić.

Možda će biti potrebno prisiliti pomoćnika za upravljane mape (MFA) da radi i Primijeni nove postavke na korisnički poštanski sandučić. Pokrenite sljedeću naredbu dok ste [spojeni na EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) da biste pokrenuli upravljani pomoćnik mape za određeni poštanski sandučić:
  
Start-ManagedFolderAssistant-identitet<name of the mailbox>

Za više informacija o postavljanju pravila arhive, pogledajte [Postavljanje pravila arhive i brisanja za poštanske sandučiće](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  