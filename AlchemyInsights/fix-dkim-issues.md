---
title: Rješavanje problema s DKIM postavljanjem
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: d725eb0d46dcbf1b5b6d77ca9f59fcafa5298bf1
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43717554"
---
# <a name="fix-dkim-setup-issues"></a>Rješavanje problema s DKIM postavljanjem

Ako naiđete na probleme s omogućivanjem DKIM-a za prilagođenu domenu, slijedite ove korake:

- Većina DKIM problema s postavljanjem povezana je s netočnim DNS zapisima. Provjerite je li DKIM CNAME zapis **(ne** TXT zapis) ispravno oblikovan. Dodatne informacije potražite u ovoj [temi](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).

- Nakon stvaranja ili ažuriranja DKIM DNS zapisa na servisu za hostiranje DNS-a za svoju domenu (obično registraru domene), pričekajte da se DNS zapisi propagire.

- Ako ne možete stvoriti DKIM DNS zapise u centru \<za\> administratore, CustomDomain možete zamijeniti prilagođenom domenom (na `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`primjer, contoso.com) i pokrenuti ovu naredbu u programu Exchange Online [PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): .
