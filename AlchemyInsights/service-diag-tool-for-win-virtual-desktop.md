---
title: Alat za dijagnostiku servisa za Windows Virtual Desktop
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
ms.openlocfilehash: c2e6f7fbcddc6721425840e87202a165cdb22664
ms.sourcegitcommit: 87bf574162e536003164ff9af50005c5a7dce601
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 12/14/2020
ms.locfileid: "49677173"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a>Alat za dijagnostiku servisa za Windows Virtual Desktop

Windows Virtual Desktop (WVD) nudi dijagnostički alat koji administratorima omogućuje prepoznavanje pogrešaka putem jednog sučelja. Ovaj alat zapisuje informacije vezane uz dijagnostiku ako je netko dodijelio ulogu WVD-a. Svaki zapisnik sadrži informacije o ulozi WVD-a uključenih u aktivnost, porukama o pogreškama koje se prikazuju tijekom sesije te informacije o klijentu i korisniku. Analitička evidencija Azure može se konfigurirati tako da snimi zapisnik aktivnosti koje je kreirao dijagnostički alat. Evo i kako:

1. Stvorite radni prostor analitike zapisnika uz [portal Azure](https://go.microsoft.com/fwlink/?linkid=2129500) ili [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).
1. [Povežite računala sa sustavom Windows s monitorom Azure](https://go.microsoft.com/fwlink/?linkid=2129913). Nabavite ID radnog prostora i primarni ključ radnog prostora. Čarobnjaku za postavljanje potrebne su te informacije da bi pravilno konfigurirali agenta i da bi se osiguralo da može komunicirati s monitorom Azure.
1. [Gurnite dijagnoziranje podataka u radni prostor](https://go.microsoft.com/fwlink/?linkid=2128284). Dijagnostičke podatke iz servisa WVD možete pritisnuti u analitiku zapisnika za radni prostor.
1. [Identificiranje i dijagnosticiranje problema](https://go.microsoft.com/fwlink/?linkid=2128338) koji su interni ili vanjski u odnosu na wvd.

Dodatne informacije o konfiguriranju alata za dijagnostiku servisa za WVD potražite [u članku Korištenje analitičke analize za značajku dijagnostike](https://go.microsoft.com/fwlink/?linkid=2128084).
