---
title: Onemogućivanje vanjskih grupa
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: f7a1bbda3a54d2662bdfe21cda961c32456edb82
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47704120"
---
# <a name="how-to-disable-external-groups"></a>Onemogućivanje vanjskih grupa

Vanjska poruka servisa Yammer primjenjuje pravila prijenosa sustava Exchange (atrs), skup proaktivnih kontrola da bi se spriječilo zajedničko korištenje podataka o tvrtki. Da biste korisnicima ograničili Stvaranje vanjskih grupa, morate konfigurirati pravilo prijenosa sustava Exchange (ETR), a zatim konfigurirati Yammer da koristi pravilo prijenosa sustava Exchange da bi blokirao vanjsku razmjenu poruka.
  
Kada stvorite pravilo u centru za administratore sustava Exchange Online, slijedite ove korake da biste postavili ETR za primjenu u servisu Yammer:
  
- Prijavite se u Yammer kao ovjereni administrator, a zatim u **centru za administratore servisa Yammer**otvorite **Postavke C sadržaja i sigurnosne \> sigurnosti.**

- U odjeljku **vanjsko razmjenu poruka**odaberite **Nametni pravila prijenosa sustava Exchange Online (atrs) u servisu Yammer.**

- Odaberite **Spremi**.

Dodatne informacije potražite u članku [onemogućivanje vanjskih poruka u mreži servisa Yammer](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).
  