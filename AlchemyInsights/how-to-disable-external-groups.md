---
title: Kako onemogućiti vanjske grupe
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: b2328ea85d3ff6ec722cc56d8a46395d8438f79c
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 10/25/2019
ms.locfileid: "36739485"
---
# <a name="how-to-disable-external-groups"></a>Kako onemogućiti vanjske grupe

Vanjska poruka tvrtke Yammer primjenjuje pravila razmjene sustava Exchange (ETRs), skup proaktivnih kontrola kako bi spriječio dijeljenje informacija o tvrtki. Kako bi se korisnici ograničili od stvaranja vanjskih grupa, morate konfigurirati pravilo sustava Exchange (ETR), a zatim konfigurirati Yammer da koristi pravilo Exchange transport za blokiranje vanjskih poruka.
  
Nakon što kreirate pravilo u centru za administraciju sustava Exchange Online, slijedite ove korake da biste postavili ETR za primjenu u servisu Yammer:
  
- Prijavite se na Yammer kao verificirani admin i u centru za **administraciju servisa Yammer**idite na C **sadržaj i sigurnosne \> sigurnosne postavke.**

- U odjeljku **vanjske poruke**odaberite **Provedba pravila sustava Exchange Online Exchange (etrs) u servisu Yammer.**

- Odaberite **Spremi**.

Za više informacija pogledajte [Onemogući vanjsku razmjenu poruka u Yammer mreži](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).
  