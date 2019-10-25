---
title: Antispam-5.7.23
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: 9c9bc2d04fb8efaa5e75194b4ca09316d24e018e
ms.sourcegitcommit: 07b47d7f3ca191363e6bc84140e8e01524d6f08e
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 10/24/2019
ms.locfileid: "37682066"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Popravak problema isporuke e-pošte za kôd pogreške 5.7.23

Provjerite SPF DNS zapis za svoju domenu na javno dostupnom SPF ili DNS zapisu za provjeru na webu.

Provjerite je li pošta u izlaznim porukama identificirana kao spam od strane sustava Office 365 i preusmjeren kroz [skup visokih rizika](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages). Poruke u bazenu velike rizike dostave neće proći SPF provjere i stoga neće biti prihvaćena od strane odredišne organizacije e-pošte.

Ako se problem nastavi pojavljivati, možda ćete morati kontaktirati admin host pošte na koji pokušavate poslati e-poštu. Zabilježite detaljnu vanjsku grešku dostupnu u poruci napuštanja početne stranice.  Office 365 podrška možda neće moći dodatno pomoći.