---
title: Antispam-5.7.23
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: ecbce4f0077dc9acab63575c19d40c0675a406ac
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47717317"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Rješavanje problema s isporučenjem e-pošte za kod pogreške 5.7.23

Provjerite SPF DNS zapis za svoju domenu na javno dostupnom alatu SPF ili DNS zapis na webu.

Provjerite nije li Microsoftova poruka bila označena kao neželjena pošta i preusmjerena putem [bazena visokog rizika](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages). Poruke u bazenu visokog rizika neće proći SPF provjere i stoga ga neće prihvatiti odredišna tvrtka ili ustanova za e-poštu.

Ako se problem i dalje pojavljuje, možda ćete se morati obratiti administratoru glavnog računala za poštu na koji pokušavate poslati e-poštu. Primjetite detaljnu vanjsku pogrešku dostupnu u poruci o odskakanje. Microsoftova podrška možda neće moći dodatno pomoći.
