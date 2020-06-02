---
title: Rješavanje problema s dkim postavljanjem
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
ms.openlocfilehash: 8195b0e3fada6da033b2d95b1fc6600e7fa3341e
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506766"
---
# <a name="fix-dkim-setup-issues"></a>Rješavanje problema s dkim postavljanjem

Ako imate problema s omogućivanjem DKIM-a za prilagođenu domenu, slijedite ove korake:

- Većina DKIM problema s postavljanjem povezana je s netočnim DNS zapisima. Provjerite je li DKIM CNAME zapis **(ne** TXT zapis) ispravno oblikovan. Dodatne informacije potražite u ovoj [temi](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).

- Nakon što stvorite ili ažurirate DKIM DNS zapise na servisu hostiranja DNS-a za svoju domenu (obično registrar domene), pričekajte da se DNS zapisi šire.

- Ako ne možete stvoriti DKIM DNS zapise u centru za administratore, možete zamijeniti \<CustomDomain\> prilagođenom domenom (na primjer, contoso.com) i pokrenuti ovu naredbu u [powershellu sustava Exchange Online](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true` .
