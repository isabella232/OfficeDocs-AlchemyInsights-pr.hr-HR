---
title: Promjena postavki ograničavanja EWS-a
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000752"
- "5653"
- "5760"
ms.openlocfilehash: f99bb449b542760c6c8d51ee399c774fbe36e3f7f40520b5eb23f39d9d7c08dd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53968369"
---
# <a name="changing-ews-throttling-settings"></a>Promjena postavki ograničavanja EWS-a

Pokrenite naš automatizirani test koji će vam omogućiti izmjenu pravilnika ograničavanja EWS-a tijekom trajanja migracije. Imajte na umu da će uvoz EWS-a i nakon toga biti ograničen na 150 mb po 5 minuta po poštanskom sandučiću. da biste postigli veće brzine propusnosti migracije, istodobno migrirati više korisnika.

Imajte na umu da promjene pravilnika ograničavanja EWS-a ne utječu na sljedeće vrste migracije (pomoću Microsoftovih alata): hibridni, posložni (RPC/HTTP), IMAP, G Suite, javna mapa ili PST servis za uvoz.