---
title: Rješavanje problema s postavljanjem DKIM-a
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 5a613321ed79e657350ec4d19b1f07ac0a091b227a8268c793a10edd9990d41f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53945923"
---
# <a name="fix-dkim-setup-issues"></a>Rješavanje problema s postavljanjem DKIM-a

Ako imate problema s omogućivanjem DKIM-a za prilagođenu domenu, slijedite korake u nastavku:

- Većina problema s postavljanjem DKIM-a povezana je s netočnim DNS zapisima. Provjerite je li DKIM CNAME **zapis** (a ne TXT zapis) pravilno oblikovan. Dodatne informacije potražite u ovoj [temi](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).

- Kada stvorite ili ažurirate DKIM DNS zapise na servisu za hostiranje DNS-a za svoju domenu (obično registrar domene), pričekajte da se DNS zapisi šire.

- Ako U centru za administratore ne možete stvoriti DKIM DNS zapise, možete je zamijeniti prilagođenom domenom (npr. contoso.com) i pokrenuti tu naredbu \<CustomDomain\> [u Exchange Online PowerShell:](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true` .
