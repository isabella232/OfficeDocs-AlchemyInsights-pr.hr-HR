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
ms.openlocfilehash: b77573e9d94195e1f0ef4a1566c45a30d53b7e68e502aeb834e2ca5b9e6c5c76
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53981105"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a>Pogreška: pravila na ovom računalu ne odgovaraju

Da biste vidjeli ažurirani status tog poznatog problema, pogledajte članak Pravila na ovom računalu ne odgovaraju [pravilima na servisu Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)

Tim Outlook implementiran je popravak u međuverziji 12928.10000. Popravak se već nalazi u programu Insider Fast i krajem lipnja 2020. idite na Mjesečni kanal. Kada popravite međuverziju, možda će vam se po posljednji put pojaviti upit "Koja pravila želite zadržati". Kada se to od vas zatraži, odaberite Poslužitelj, a zatim se vratite u Outlook i ponovno omogućite sva onemogućena pravila.

Dok popravak ne bude dostupan, upotrijebite sljedeće zaobilazno rješenje:

**Zaobilazno** rješenje: u nedavnim izvješćima pojavio se problem za one koji su stvorili samo klijentska pravila Outlook stolna računala. Ako naiđete na problem, razmislite o brisanju pravila, a zatim pravila stvarajte i uređujte samo u aplikaciji OWA (Outlook Web App) dok se problem ne riješi.

Ako pravila ne možete ručno izbrisati, možete pokrenuti naredbu Outlook kada pokrenete Outlook pokretanjem Outlook.exe /cleanrules. Time ćete izbrisati i pravila klijenta i poslužitelja. Izbrisat će se sva pravila za sve račune u Outlook profilu. Ta je naredba dodatno dokumentirana u članku s prebacivanjem naredbenog retka.

