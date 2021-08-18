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
ms.openlocfilehash: 4139f47f40a89069521aaa1a3e4fdab56e9e27a2096ae0ad099be827f60d51fc
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54090986"
---
# <a name="troubleshoot-mdatp-installation-problems-on-a-mac"></a>Otklanjanje poteškoća s instalacijom MDATP-a na Macu

Ako ručna instalacija ne uspije, **na stranici sa** sažetkom čarobnjaka za instalaciju prikazuje se sljedeća pogreška:

"Došlo je do pogreške tijekom instalacije. Instalacijski program naišao je na pogrešku zbog koje instalacija nije uspijevala. Zatražite pomoć od proizvođača softvera."

Za implementacije MDM-a na stranici se prikazuje i generička pogreška instalacije.

Premda krajnjim korisnicima ne prikazujemo točne pogreške, zadržavamo datoteku zapisnika s tijekom instalacije u **programu /Library/Logs/Microsoft/mdatp/install.log.** Svaka se sesija instalacije prilaže ovoj datoteci zapisnika. Da biste izlazni samo zadnju instalacijsku sesiju, koristite `sed` .

Dodatne informacije potražite u članku Otklanjanje [poteškoća s instalacijom za Microsoft Defender ATP za Mac](https://go.microsoft.com/fwlink/?linkid=2144615).
