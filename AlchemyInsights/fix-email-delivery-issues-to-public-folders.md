---
title: Rješavanje problema s isporukom e-pošte u javne mape omogućene za poštu
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.assetid: ''
ms.openlocfilehash: e261fe60843555fa45927b0a6b36e1ccf79fb028
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716344"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>Rješavanje problema s isporukom e-pošte u javne mape omogućene za poštu

Ako vanjski pošiljatelji ne mogu slati poruke u javne mape omogućene za poštu, a pošiljatelji primaju pogrešku: **nije moguće pronaći (550 5.4.1)**, provjerite je li domena e-pošte za javnu mapu konfigurirana kao interna domena prijenosa umjesto autoritativne domene:

1. Otvorite [centar za administratore sustava Exchange (EAC).](https://docs.microsoft.com/Exchange/exchange-admin-center)

2. Idite na **Tijek** \> pošte **Prihvaćene domene**, odaberite prihvaćenu domenu, a zatim kliknite **Uredi**.

3. Na stranici svojstava koja se otvori, ako je vrsta domene postavljena na **Autoritativni**, promijenite vrijednost **u Unutarnji relej,** a zatim kliknite **Spremi**.

Ako vanjski pošiljatelji prime pogrešku **koju nemate dozvolu (550 5.7.13),** pokrenite sljedeću naredbu u [sustavu Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) da biste vidjeli dozvole za anonimne korisnike u javnoj mapi:

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous`Na primjer. `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`

Da biste vanjskim korisnicima omogućili slanje e-pošte u ovu javnu mapu, dodajte pristup CreateItems izravno korisniku Anonymous. Na primjer. `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`
