---
title: Otklanjanje poteškoća s instalacijom MDATP-a na Macu
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 4b03361666f950a2010e4c4d8e78d156438d9e90
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/09/2021
ms.locfileid: "50692860"
---
# <a name="troubleshoot-mdatp-installation-problems-on-a-mac"></a>Otklanjanje poteškoća s instalacijom MDATP-a na Macu

Ako Ručna instalacija ne uspije, na stranici **sažetka** čarobnjaka za instalaciju prikazat će se sljedeća pogreška:

"Prilikom instalacije došlo je do pogreške. Instalacijski program naišao je na pogrešku koja je uzrokovala neuspjeh instalacije. Zatražite pomoć od proizvođača softvera. "

Na stranici implementacije MDM-a stranica prikazuje i generički neuspjeh instalacije.

Iako ne prikazujemo točne pogreške krajnjim korisnicima, držimo datoteku zapisnika s napretkom instalacije u **/Library/logs/Microsoft/mdatp/install.log**. Svaka instalacija sesije dodaje se u ovu datoteku zapisnika. Da biste mogli obaviti samo zadnju sesiju instalacije, koristite `sed` .

Dodatne informacije potražite u članku [Otklanjanje poteškoća s instalacijom za Microsoft Defender ATP za Mac](https://go.microsoft.com/fwlink/?linkid=2144615).
