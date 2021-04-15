---
title: 'Pogreška: pravila na ovom računalu ne odgovaraju'
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: c46eb856baafbef9bc3b7fa34a0258ef16923fb8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51782944"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a>Pogreška: pravila na ovom računalu ne odgovaraju

Da biste vidjeli ažurirani status tog poznatog problema, [pogledajte članak Pravila na ovom računalu ne](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0) odgovaraju pravilima u sustavu Microsoft Exchange

Tim za Outlook implementiran je popravak u međuverziji 12928.10000. Popravak se već nalazi u programu Insider Fast i krajem lipnja 2020. idite na Mjesečni kanal. Kada popravite međuverziju, možda će vam se po posljednji put pojaviti upit "Koja pravila želite zadržati". Kada se to od vas zatraži, odaberite Poslužitelj, a zatim se vratite u Outlook i ponovno omogućite sva onemogućena pravila.

Dok popravak ne bude dostupan, upotrijebite sljedeće zaobilazno rješenje:

**Zaobilazno** rješenje: u nedavnim izvješćima pojavio se problem za one koji su stvorili samo klijentska pravila u programu Outlook za stolna računala. Ako naiđete na problem, razmislite o brisanju pravila, a zatim pravila stvarajte i uređujte samo u aplikaciji OWA (Outlook Web App) dok se problem ne riješi.

Ako ne možete ručno izbrisati pravila, prilikom pokretanja programa Outlook možete pokrenuti naredbu programa Outlook pokretanjem Outlook.exe /cleanrules. Time ćete izbrisati i pravila klijenta i poslužitelja. Izbrisat će sva pravila za sve račune u profilu programa Outlook. Ta je naredba dodatno dokumentirana u članku s prebacivanjem naredbenog retka.

