---
title: Oslobađanje prostora na disku u sustavu Windows 10
ms.author: pebaum
author: pebaum
manager: dansimp
ms.date: 03/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9771"
- "9774"
- "9005390"
- "9005403"
ms.openlocfilehash: 2313636307bfddce2810c2d4c4ce9e3b407a7bdf
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: HT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/02/2021
ms.locfileid: "51505348"
---
# <a name="free-up-drive-space-in-windows-10"></a>Oslobađanje prostora na disku u sustavu Windows 10

Evo dvije mogućnosti za oslobađanje prostora na disku u sustavu Windows:

- Oslobađanje prostora na disku u sustavu Windows 10.
- Oslobodite prostor za ažuriranja sustava Windows 10 pomoću vanjskog uređaja za pohranu.

Ako nakon čišćenja diska i dalje imate malo prostora na disku, moguće je da se vaša privremena mapa brzo puni aplikacijskim datotekama (.appx) koje upotrebljava Microsoft Store. Za rješavanje ovog problema ponovo postavite Store, očistite njegovu predmemoriju te pokrenite alat za otklanjanje poteškoća sustava Windows Update. Provjerite je li Microsoft Store zatvoren prije nego što nastavite s ovim koracima.

**Korak 1: Ponovo postavite Microsoft Store**

**Napomena** Ovo trajno briše podatke aplikacije na uređaju, uključujući vaše preferencije i pojedinosti o prijavi.

1. Odaberite **Start** > **Postavke** > **Aplikacije** > **Aplikacije & značajke**.

1. Na popisu aplikacija pronađite i odaberite Microsoft Store.

1. Odaberite **Dodatne mogućnosti**.

1. Pomaknite se prema dolje i odaberite **Ponovo postavi**, a zatim **Potvrdi ponovno postavljanje**.

**Korak 2: očisti predmemoriju aplikacije Microsoft Store**

1. Pritisnite tipku s logotipom sustava Windows i slovo R da biste otvorili dijaloški okvir Pokreni.

1. Upišite wsreset.exe i odaberite **U redu**.

1. Otvara se prazan prozor naredbenog retka. Nakon otprilike 10 sekundi, prozor se zatvara i Store se automatski otvara.

**Korak 3: ponovo postavite Windows Update**

1. Odaberite **Start** > **Postavke** > **Ažuriranje & Sigurnost** > **Otklanjanje poteškoća**.

1. Pomaknite se prema dolje i odaberite **Windows Update** s popisa, i odaberite **Pokreni alat za otklanjanje poteškoća**.

1. Ponovo pokrenite računalo i provjerite pojavljuje li se i dalje problem.

