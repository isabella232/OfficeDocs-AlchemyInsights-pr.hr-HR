---
title: Alat za dijagnostiku servisa za Windows virtualnu radnu površinu
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003893"
- "6947"
ms.openlocfilehash: 58688e3216ba6777b1a4f76095bd39c81a2d2a8294e06b6bc61c7134f6d589f9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54052378"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a>Alat za dijagnostiku servisa za Windows virtualnu radnu površinu

Windows Virtualna radna površina (WVD) nudi dijagnostički alat koji administratorima omogućuje prepoznavanje pogrešaka putem jednog sučelja. Taj alat zapisuje podatke vezane uz dijagnostiku svaki put kada WVD koristi netko kome je dodijeljena WVD uloga. Svaki zapisnik sadrži informacije o ulozi WVD-a uključenoj u aktivnost, porukama o pogreškama koje se prikazuju tijekom sesije te podacima o klijentu i korisniku. Analitika zapisnika servisa Azure može se konfigurirati tako da snima zapisnik aktivnosti koji je stvorio dijagnostički alat. Evo i kako:

1. Stvorite radni prostor analitike zapisnika pomoću [portala Azure ili](https://go.microsoft.com/fwlink/?linkid=2129500) [komponente Azure PowerShell.](https://go.microsoft.com/fwlink/?linkid=2129501)
1. [Povezivanje Windows računala na Azure Monitor](https://go.microsoft.com/fwlink/?linkid=2129913). Nabavite ID radnog prostora i primarni ključ radnog prostora. Čarobnjaku za postavljanje potrebni su ti podaci da bi agent pravilno konfigurirao i kako bi mogao komunicirati sa servisom Azure Monitor.
1. [Gurnite dijagnostičke podatke u radni prostor](https://go.microsoft.com/fwlink/?linkid=2128284). Dijagnostičke podatke s WVD klijenta možete prenjeti u analitiku zapisnika za radni prostor.
1. [Prepoznajte i dijagnosticirajte probleme koji](https://go.microsoft.com/fwlink/?linkid=2128338) su interni ili vanjski u odnosu na WVD.

Dodatne informacije o konfiguraciji alata za dijagnostiku servisa za WVD potražite u članku [Korištenje analitike zapisnika za značajku dijagnostike](https://go.microsoft.com/fwlink/?linkid=2128084).
