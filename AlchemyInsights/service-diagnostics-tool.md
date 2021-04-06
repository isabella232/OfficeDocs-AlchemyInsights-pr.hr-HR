---
title: Alat za dijagnostiku servisa za virtualnu radnu površinu sustava Windows
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9004219"
- "10873"
ms.openlocfilehash: dfa59c86508c8658c880f4f3f21a002524e909d1
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/05/2021
ms.locfileid: "51595516"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a>Alat za dijagnostiku servisa za virtualnu radnu površinu sustava Windows

Windows Virtual Desktop (WVD) nudi dijagnostički alat koji administratorima omogućuje prepoznavanje pogrešaka putem jednog sučelja. Taj alat zapisuje podatke vezane uz dijagnostiku svaki put kada WVD koristi netko kome je dodijeljena WVD uloga. Svaki zapisnik sadrži informacije o ulozi WVD-a uključenoj u aktivnost, porukama o pogreškama koje se prikazuju tijekom sesije te podacima o klijentu i korisniku. Analitika zapisnika servisa Azure može se konfigurirati tako da bilježi zapisnik aktivnosti koji je stvorio dijagnostički alat na sljedeći način:

1. Stvorite radni prostor analitike zapisnika pomoću [portala Azure ili](https://go.microsoft.com/fwlink/?linkid=2129500) [komponente Azure PowerShell.](https://go.microsoft.com/fwlink/?linkid=2129501)

1. [Povežite računala sa sustavom Windows sa servisom Azure Monitor](https://go.microsoft.com/fwlink/?linkid=2129913). Nabavite ID radnog prostora i primarni ključ radnog prostora. Čarobnjaku za postavljanje potrebni su ti podaci da bi agent pravilno konfigurirao i kako bi mogao komunicirati sa servisom Azure Monitor.

1. [Gurnite dijagnostičke podatke u radni prostor](https://go.microsoft.com/fwlink/?linkid=2128284). Dijagnostičke podatke s WVD klijenta možete prenjeti u analitiku zapisnika za radni prostor.

1. [Prepoznajte i dijagnosticirajte probleme](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell) koji su interni ili vanjski u odnosu na WVD.

Dodatne informacije o konfiguraciji alata za dijagnostiku servisa za WVD potražite u članku Korištenje analitike zapisnika za značajku dijagnostike.