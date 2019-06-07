---
title: Ispravite probleme DKIM Postava
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 4d6dadbcbf71fe6e9ea56d6a82a7d8ababdd38ef
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/07/2019
ms.locfileid: "34764911"
---
# <a name="fix-dkim-setup-issues"></a>Ispravite probleme DKIM Postava

Ako se pojave problemi omogućavanja DKIM za prilagođene domene, slijedite ove korake:

- Većinu problema Postava DKIM su povezani neispravna DNS zapisa. Provjerite je li ispravno oblikovani zapisom DKIM CNAME (**ne** TXT zapisu). Dodatne informacije potražite u ovoj [temi](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).

- Nakon što stvorite ili ažuriranje zapisa DKIM DNS na DNS domaćin usluge za domenu (obično vaše domene Registrator), pričekajte zapise DNS proširiti.

- Ako ne možete stvoriti zapise DKIM DNS u centru za administraciju, možete zamijeniti \<CustomDomain\> s prilagođene domene (na primjer, contoso.com) i pokrenuti ovu naredbu [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.
