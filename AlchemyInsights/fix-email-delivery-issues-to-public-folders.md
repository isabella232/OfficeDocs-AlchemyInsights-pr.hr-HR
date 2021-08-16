---
title: Rješavanje problema s isporukom e-pošte u javne mape s omogućenom poštom
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
- "1956"
- "3500007"
ms.openlocfilehash: ff1400f694ae037a8658356af068b4c20b8fa9d9908dafedb90db7bb6859530f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54068804"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>Rješavanje problema s isporukom e-pošte u javne mape s omogućenom poštom

Ako vanjski pošiljatelji ne mogu slati poruke u javne mape s omogućenom e-poštom, a pošiljatelji prime pogrešku: nije moguće **pronaći (550 5.4.1),** provjerite je li domena e-pošte za javnu mapu konfigurirana kao interna domena za razmjenu umjesto mjerodavne domene:

1. Otvorite [centar Exchange administratora (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).

2. Idite **na Tijek pošte** \> **Prihvaćene domene**, odaberite prihvaćenu domenu, a zatim kliknite **Uređivanje**.

3. Na stranici svojstava koja će se otvoriti ako je vrsta domene postavljena na Mjerodavno **,** promijenite vrijednost u **Interni prijenosnik,** a zatim kliknite **Spremi**.

Ako vanjski pošiljatelji prime pogrešku nemate dozvolu **(550 5.7.13),** pokrenite sljedeću naredbu u programu [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) da biste vidjeli dozvole za anonimne korisnike u javnoj mapi:

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` Na primjer, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous` .

Da biste vanjskim korisnicima omogućili slanje e-pošte u tu javnu mapu, dodajte pristup createitems korisniku Anonimno. Na primjer, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems` .
