---
title: Premještanje poruka e-pošte u poštanski sandučić Arhiva
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 7e72766f441e210a81fcfd6c07b1801f6c0474afb02a70edf2ad8dbb571f3d2a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53974949"
---
# <a name="move-email-to-the-archive-mailbox"></a>Premještanje e-pošte u arhivski poštanski sandučić

Ako želite da pokrenemo automatske provjere postavki navedenih u nastavku, odaberite gumb natrag <– pri vrhu ove stranice, a zatim unesite adresu e-pošte korisnika koji ima problema s premještanjem e-pošte u arhivski poštanski sandučić.

1. Provjerite je li **omogućen poštanski sandučić** Arhiva. Ako nije, slijedite korake u ovom [članku da biste](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) omogućili arhivski poštanski sandučić.

2. Da biste poruke automatski arhivirali u  arhivski poštanski sandučić, oznaka zadržavanja s akcijom Premjesti u arhiviranje mora se postaviti tako da se automatski primjenjuje na oznaku cijeli poštanski sandučić **(zadano).** Pomoću sljedećih koraka stvorite oznaku: [Arhiviraj zadanu oznaku](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).

3. Zatim dodajte oznaku **Arhiva pravilniku** o zadržavanju. U centru Exchange za administratore **odaberite Pravila** zadržavanja > dodajte oznaku **Premjesti u** arhiviranje u pravilnik > **Spremi**.

4. Sada [dodijelite pravilnik o zadržavanju](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) poštanskom sandučiću određenog korisnika. Isti će se pravilnik primijeniti i na poštanski sandučić **Primarno** i **arhiviranje.**

Možda će biti potrebno prisiliti pomoćnik za upravljane mape (MFA) da pokrene i primijeni nove postavke na korisnikov poštanski sandučić. Pokrenite sljedeću naredbu dok [ste povezani s ljuskom EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) da biste pokrenuli pomoćnik za upravljane mape za određeni poštanski sandučić:
  
Start-ManagedFolderAssistant -Identity <name of the mailbox>

Dodatne informacije o postavljanju pravilnika arhiviranja potražite u članku [Postavljanje pravilnika arhiviranja i brisanja poštanskih sandučića](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  