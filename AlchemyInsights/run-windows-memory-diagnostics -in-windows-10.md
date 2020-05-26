---
title: Pokretanje dijagnostike memorije u sustavu Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002959"
- "5661"
ms.openlocfilehash: 3fedc52d02f1f70743429d0313eda0361306c3f3
ms.sourcegitcommit: 18b080c2a5d741af01ec589158effc35ea7cf449
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 05/19/2020
ms.locfileid: "44357311"
---
# <a name="run-windows-memory-diagnostics-in-windows-10"></a>Pokretanje dijagnostike memorije u sustavu Windows 10

Ako se Sustav Windows i aplikacije na PC-ju ruše, smrzavaju ili djeluju na nestabilan način, možda imate problema s memorijom PC-ja (RAM-om). Možete pokrenuti dijagnostiku memorije sustava Windows da biste provjerili ima li problema s RAM-om PC-ja.

U okvir pretraživanja na programskoj traci upišite **dijagnostika memorije,** a zatim odaberite **Dijagnostika memorije sustava Windows**. 

Da biste pokrenuli dijagnostiku, PC se mora ponovno pokrenuti. Imate mogućnost odmah ponovno gimnastike (spremite svoj rad i zatvorite otvorene dokumente i e-mailove) ili zakažite automatsko pokretanje dijagnostike prilikom sljedećeg ponovnog pokretanja računala:

![Dijagnostika memorije u sustavu Windows](media/windows-memory-diagnostic.png)

Kada se PC ponovno pokrene, **dijagnostički alat za memoriju sustava Windows** automatski će se pokrenuti. Status i napredak prikazat će se tijekom pokretanja dijagnostike, a imate mogućnost otkazivanja dijagnostike tako da pritisnete **tipku ESC** na tipkovnici.

Kada se dijagnostika dovrši, Windows će se normalno pokrenuti.
Odmah nakon ponovnog pokretanja, kada se pojavi radna površina, pojavit će se obavijest (pored ikone **Akcijskog centra** na programskoj traci) da biste naznačili jesu li pronađene pogreške u memoriji. Na primjer:

Evo ikone akcijskog centra: ![Ikona akcijskog centra](media/action-center-icon.png) 

I oglednu obavijest: ![Nema pogrešaka u memoriji](media/no-memory-errors.png)

Ako ste propustili obavijest, možete odabrati ikonu **Akcijskog centra** na programskoj traci za prikaz **akcijskog centra** i prikaz popisa obavijesti koji se može pomicati.

Da biste pregledali detaljne informacije, u okvir za pretraživanje na programskoj traci upišite **događaj,** a zatim odaberite **Preglednik događaja**. U lijevom oknu **preglednika događaja**idite na **Windows Logs > System**. U desnom oknu skenirajte popis dok gledate stupac **Izvor** dok ne vidite događaje s izvornom vrijednošću **MemoryDiagnostics-Results**. Označite svaki takav događaj i pogledajte informacije o rezultatima u okviru na kartici **Općenito** ispod popisa.
