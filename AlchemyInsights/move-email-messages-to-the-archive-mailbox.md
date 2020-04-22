---
title: Premještanje poruka e-pošte u poštanski sandučić Arhive
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
ms.openlocfilehash: a5ad81e97df0ed5c337a622126173df94af80bb8
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713638"
---
# <a name="move-email-to-the-archive-mailbox"></a>Premještanje e-pošte u arhivski poštanski sandučić

1. Provjerite je li poštanski **sandučić arhive** omogućen. Ako nije, slijedite korake u [ovom članku](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) da biste omogućili poštanski sandučić arhive.

2. Da biste automatski arhivirali poruke u arhivski poštanski sandučić, oznaka zadržavanja s akcijom **Premjesti u arhivu** mora se automatski **primijeniti na cijelu oznaku poštanskog sandučića (zadano).** Slijedite korake ovdje da biste izradili oznaku: [Arhiviraj zadanu oznaku](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).

3. Zatim dodajte oznaku **Arhivu** u pravila zadržavanja. U centru za administratore sustava Exchange odaberite **Pravila zadržavanja** > **dodajte oznaku Premjesti u arhivu** u pravilo > **Spremi**.

4. Sada [dodijelite pravila zadržavanja](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) poštanskom sandučiću određenog korisnika. Ista pravila primijenit će se i na poštanski sandučić **Primarni** i **Arhiva.**

Možda će biti potrebno prisiliti pomoćnika za upravljane mape (MFA) da pokrene i primijeni nove postavke na korisnikov poštanski sandučić. Pokrenite sljedeću naredbu dok [ste povezani s EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) da biste pokrenuli pomoćnika za upravljane mape za određeni poštanski sandučić:
  
Pomoćnik za početnu mapu –identitet<name of the mailbox>

Dodatne informacije o postavljanju pravila arhiviranja [potražite u odjeljku Postavljanje pravila arhiviranja i brisanja za poštanske sandučiće](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  