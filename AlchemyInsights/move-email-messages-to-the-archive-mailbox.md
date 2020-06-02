---
title: Premještanje poruka e-pošte u poštanski sandučić Arhiva
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 35c11f1bfb7c61b28a64f0128c29ddf7b4fce939
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511032"
---
# <a name="move-email-to-the-archive-mailbox"></a>Premještanje e-pošte u poštanski sandučić arhive

1. Provjerite je li omogućen **poštanski sandučić arhive.** Ako nije, pomoću koraka u [ovom članku](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) omogućite poštanski sandučić arhive.

2. Da bi se poruke automatski arhivirale u poštanski sandučić arhive, oznaka zadržavanja s akcijom **Premjesti u arhiv** mora biti postavljena tako da se automatski primjenjuje na cijeli poštanski sandučić **(zadana) oznaka**. Slijedite korake ovdje da biste izradili oznaku: [Arhiviraj zadanu oznaku](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).

3. Zatim dodajte oznaku **Arhiva** u pravila zadržavanja. U centru za administratore sustava Exchange odaberite **Pravila zadržavanja** > dodati **oznaku Premjesti** u arhivu u pravila > **Spremi**.

4. Sada [dodijelite pravila zadržavanja](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) određenom korisničkom poštanskom sandučiću. Ista pravila primijenit će se i na poštanski sandučić **Primarna** i **arhiva.**

Možda će biti potrebno prisiliti pomoćnika za upravljane mape (MFA) da pokrene i primijeni nove postavke na poštanski sandučić korisnika. Pokrenite sljedeću naredbu dok [ste povezani s exo powershellom da](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) biste pokrenuli pomoćnika za upravljane mape za određeni poštanski sandučić:
  
Početni upravljani identitet pomoćnika -identitet<name of the mailbox>

Dodatne informacije o postavljanju pravila arhiviranja potražite [u odjeljku Postavljanje pravila arhiviranja i brisanja poštanskih sandučića](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  