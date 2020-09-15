---
title: 'Pogreška: pravila na ovom računalu ne podudaraju se'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: c2feb6da651d8b3eb7af6a057335b28d26f9e7f6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690955"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a>Pogreška: pravila na ovom računalu ne podudaraju se

Da biste vidjeli ažurirani status tog poznatog problema, pročitajte članak [pravila na ovom računalu ne podudaraju se s pravilima u sustavu Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)

Tim za Outlook implementirao je popravak u Međuaplikaciji 12928,10000. Popravak je već brzo uključen u Insider i bit će na mjesečnom kanalu krajem lipnja 2020. Kada završite s ispravnom izgradnjom, možda ćete dobiti upit "koja pravila želite zadržati" posljednji put. Kada se to od vas zatraži, odaberite poslužitelj, a zatim se vratite u Outlook i ponovno omogućite onemogućena pravila.

Dok popravak ne bude dostupan, upotrijebite sljedeće zaobilazno rješenje:

**Zaobilazno rješenje**: u nedavnim izvješćima došlo je do problema za one koji su stvorili samo klijentska pravila u radnoj površini programa Outlook. Ako i dalje pokrenete problem, razmotrite brisanje pravila, a zatim stvaranje i uređivanje pravila samo u aplikaciji OWA (Outlook Web App) dok se problem ne riješi.

Ako ne možete ručno izbrisati pravila, možete pokrenuti naredbu programa Outlook prilikom pokretanja programa Outlook pokretanjem Outlook.exe/cleanrules. Time ćete izbrisati i pravila klijenta i poslužitelja. Izbrisat će sva pravila za sve račune u profilu programa Outlook. Ta je naredba dodatno dokumentirana u članku prekidača naredbenog retka.

