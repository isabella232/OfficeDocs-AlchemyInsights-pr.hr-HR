---
title: Ispravite probleme isporuke e-pošte javne mape
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.assetid: ''
ms.openlocfilehash: f7b5e5a230d26870d5e95e8762b5874f73723c6d
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36525089"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>Ispravite probleme isporuke e-pošte javne mape

Ako vanjskih pošiljatelja nije moguće slati poruke pošte omogućeno javne mape i pošiljatelji pogrešci: **ne može se pronaći (550 5.4.1)**, provjerite domena e-pošte za javnu mapu konfiguriran kao Interna preusmjeravanja domene umjesto programa Mjerodavne domene:

1. Otvorili [Centar za administraciju sustava Exchange (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).

2. Idi na **Protok e-pošte** \> **domena prihvaćeno**, odaberite domenom prihvaćene, a zatim kliknite **Uređivanje**.

3. U svojstvima stranice da otvara ako je vrsta domene za **Authoritative**, promijenite vrijednost **Interna preusmjeravanja** i kliknite **Spremi**.

Vanjskih pošiljatelja primanje pogreška **nemate dozvolu (550 5.7.13)**, pokrenite sljedeću naredbu u [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) da biste vidjeli dozvole za anonimne korisnike u javnu mapu:

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous`Na primjer, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.

Dopustiti vanjskim korisnicima da šalju e-pošte javne mape, dodajte CreateItems access desno korisnik anonimno. Na primjer, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.
