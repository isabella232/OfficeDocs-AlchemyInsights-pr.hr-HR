---
title: Premještanje poruka e-pošte u arhivski poštanski sandučić
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
ms.openlocfilehash: 61d0b1a58fff6655b745bb9d39e8384f0a543336
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47799772"
---
# <a name="move-email-to-the-archive-mailbox"></a>Premještanje e-pošte u arhivski poštanski sandučić

Ako želite da pokrenete automatske provjere za navedene postavke, odaberite gumb natrag < – pri vrhu ove stranice, a zatim unesite adresu e-pošte korisnika koji ima problema s premještanjem e-pošte u arhivski poštanski sandučić.

1. Potvrdite da je omogućen **arhivski poštanski sandučić** . Ako ne, slijedite upute u [ovom članku](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) da biste omogućili arhivski poštanski sandučić.

2. Da biste automatski arhivirali poruke u arhivski poštanski sandučić, oznaka zadržavanja s akcijom **Premjesti u arhiviranje** mora biti postavljena tako da se **automatski primjenjuje na cijeli poštanski sandučić (zadana) oznaka**. Koristite korake ovdje da biste stvorili oznaku: [Arhiviraj zadanu oznaku](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).

3. Zatim dodajte oznaku **arhive** u pravilnik o zadržavanju. U centru za administratore sustava Exchange odaberite **pravila zadržavanja** > Dodajte **oznaku Premjesti u arhivu** da bi se pravila > **Spremi**.

4. Sada [dodijelite pravilnik o zadržavanju](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) za poštanski sandučić određenog korisnika. Isto pravilo primijenit će se i na **primarni** i **arhivski** poštanski sandučić.

Možda će biti potrebno prisiliti pomoćnika za upravljanu mapu (MFA) da pokreće i Primijeni nove postavke na korisnikov poštanski sandučić. Pokrenite sljedeću naredbu dok ste [povezani s programom EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) da biste pokrenuli pomoćnik za upravljane mape za određeni poštanski sandučić:
  
Start-ManagedFolderAssistant-Identity <name of the mailbox>

Dodatne informacije o postavljanju pravilnika arhiviranja potražite [u članku Postavljanje pravilnika o arhiviranju i brisanju za poštanske sandučiće](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  