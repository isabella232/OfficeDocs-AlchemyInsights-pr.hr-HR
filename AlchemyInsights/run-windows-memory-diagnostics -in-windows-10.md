---
title: Pokretanje dijagnostike memorije sustava Windows u sustavu Windows 10
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002959"
- "5661"
ms.openlocfilehash: ff8f80b3df4e3809e844195128f4d99cbc4667be
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826659"
---
# <a name="run-windows-memory-diagnostics-in-windows-10"></a>Pokretanje dijagnostike memorije sustava Windows u sustavu Windows 10

Ako se Windows i aplikacije na PC-ju rušiju, smrzavaju ili djeluju na nestabilan način, možda imate problema s memorijom PC-ja (RAM-om). Da biste provjerili ima li problema s RAM-om PC-ja, pokrenite dijagnostiku memorije sustava Windows.

U okvir za pretraživanje na programskoj traci upišite **dijagnostika** memorije , a zatim odaberite **Dijagnostika memorije u sustavu Windows**. 

Da biste pokrenuli dijagnostiku, PC se mora ponovno pokrenuti. Imate mogućnost da se odmah ponovno pokrenete (spremite svoje radne dokumente i najprije zatvorite otvorene dokumente i poruke e-pošte) ili zakažete automatsko pokretanje dijagnostike prilikom sljedećeg ponovnog pokretanja PC-ja:

![Dijagnostika memorije u sustavu Windows](media/windows-memory-diagnostic.png)

Kada se PC ponovno pokrene, automatski će se pokrenuti alat za **dijagnostiku memorije** u sustavu Windows. Status i napredak prikazat će se kao pokretanje dijagnostike, a možete otkazati dijagnostiku tako da na tipkovnici ujete **tipku ESC.**

Kada se dijagnostika dovrši, Windows će se normalno pokrenuti.
Odmah nakon ponovnog pokretanja, kada se pojavi radna površina, pojavit će se obavijest (pokraj ikone **Akcijskog** centra na programskoj traci) da bi se naznačilo jesu li pronađene pogreške u memoriji. Na primjer:

Evo ikone Akcijskog centra: ![Ikona akcijskog centra](media/action-center-icon.png) 

I ogledna obavijest: ![Nema pogrešaka u memoriji](media/no-memory-errors.png)

Ako ste propustili obavijest, možete odabrati ikonu **Akcijskog** centra na programskoj traci da biste prikazali **akcijski** centar i vidjeli popis obavijesti koji se može pomicati.

Da biste pregledali detaljne informacije, **upišite** događaj u okvir za pretraživanje na programskoj traci, a zatim **odaberite Preglednik događaja**. U lijevom **oknu preglednika** događaja otvorite zapisnike sustava **Windows > System**. U desnom oknu pregledajte popis dok pregledavate stupac **Izvor** dok ne vidite događaje s izvorišnom vrijednošću **MemoryDiagnostics-Results**. Isticanje svakog takvog događaja i prikaz informacija o rezultatima u okviru ispod **kartice** Općenito ispod popisa.
