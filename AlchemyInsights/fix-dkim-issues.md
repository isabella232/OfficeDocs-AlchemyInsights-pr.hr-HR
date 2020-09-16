---
title: Rješavanje problema s postavljanjem programa DEKIM
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
ms.openlocfilehash: 35e8023d26fe26211e27521ceb8751d2d7fc7a21
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47744942"
---
# <a name="fix-dkim-setup-issues"></a>Rješavanje problema s postavljanjem programa DEKIM

Ako naiđete na probleme s omogućivanjem servisa DEKIM za prilagođenu domenu, slijedite sljedeće korake:

- Većina problema s postavljanjem programa di odnosi se na pogrešne DNS zapise. Provjerite je li deformator CNAME zapisa (**ne** TXT zapis) pravilno oblikovan. Dodatne informacije potražite u ovoj [temi](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).

- Kada stvorite ili ažurirate svoj DNS zapise u servisu DNS za hostiranje domene (tipično, registrar domene), pričekajte da se DNS zapisi propagiraju.

- Ako ne možete stvoriti DKIM DNS zapise u centru za administratore, možete zamijeniti \<CustomDomain\> prilagođenu domenu (na primjer, contoso.com) i pokrenuti ovu naredbu u komponenti [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true` .
