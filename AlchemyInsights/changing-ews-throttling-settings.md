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
ms.openlocfilehash: 16916d5f16f763d87ce0d5ef830e741279c9f4df
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51818028"
---
# <a name="changing-ews-throttling-settings"></a>Promjena postavki ograničavanja EWS-a

Pokrenite naš automatizirani test koji će vam omogućiti izmjenu pravilnika ograničavanja EWS-a tijekom trajanja migracije. Imajte na umu da će uvoz EWS-a i nakon toga biti ograničen na 150 mb po 5 minuta po poštanskom sandučiću. da biste postigli veće brzine propusnosti migracije, istodobno migrirati više korisnika.

Imajte na umu da promjene pravilnika ograničavanja EWS-a ne utječu na sljedeće vrste migracije (pomoću Microsoftovih alata): hibridni, posložni (RPC/HTTP), IMAP, G Suite, javna mapa ili PST servis za uvoz.