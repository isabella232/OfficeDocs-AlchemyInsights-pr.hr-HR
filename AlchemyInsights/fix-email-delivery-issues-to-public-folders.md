---
title: Rješavanje problema s isporučenjem e-pošte javnim mapama s omogućenim e-poštom
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
ms.openlocfilehash: 74a26306766ed7952a3bbbcb06f1f0113a113024
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 10/06/2020
ms.locfileid: "48366456"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>Rješavanje problema s isporučenjem e-pošte javnim mapama s omogućenim e-poštom

Ako vanjski pošiljatelji ne mogu slati poruke u javne mape koje su omogućene za e-poštu, a pošiljatelji primaju pogrešku: **nije ga moguće pronaći (550 je)**, provjerite je li domena e-pošte za javnu mapu konfigurirana kao domena za interni prijenos, a ne autoritativna domena:

1. Otvorite [centar za administratore sustava Exchange (AAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).

2. Otvorite domene koje su prihvaćene za **tijek pošte** \> **Accepted domains**, odaberite prihvaćenu domenu, a zatim kliknite **Uredi**.

3. Na stranici svojstva koja se otvara, ako je vrsta domene postavljena na **autoritativna**, promijenite vrijednost u **interni prijenos** , a zatim kliknite **Spremi**.

Ako vanjski pošiljatelji dobiju pogrešku koja nema **dozvolu (550 5.7.13)**, pokrenite sljedeću naredbu u komponenti [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) da biste vidjeli dozvole za anonimne korisnike u javnoj mapi:

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` Na primjer, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous` .

Da biste vanjskim korisnicima dopustili slanje e-pošte u tu javnu mapu, dodajte mogućnost pristupa CreateItems izravno korisniku anonimnom. Na primjer, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems` .
