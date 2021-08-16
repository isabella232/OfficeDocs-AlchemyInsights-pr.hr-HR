---
title: Pronalaženje IP adrese u zapisniku nadzora
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: 5b58803719df700290f495cb2d2d6742f072420a2a1d393534ca165bb5a14fbb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54017124"
---
# <a name="find-the-ip-address-in-audit-log"></a>Pronalaženje IP adrese u zapisniku nadzora

1. IP adresa koja odgovara aktivnosti koju je izveo korisnik ili administrator prikazuje se u zapisnicima nadzora. Zapisuje se i podaci o klijentu. Evo kako prepoznati IP adresu:

1. Idite na [centar Office 365 sigurnosti & usklađenosti](https://go.microsoft.com/fwlink/p/?linkid=2077143).
1. Odaberite **Pretraživanje**  >  **[pretraživanja zapisnika nadzora](https://go.microsoft.com/fwlink/?linkid=2103759)**.
    > [!NOTE]
    > Ako vidite obavijest da morate uključiti nadzor, odmah je uključite. Ako ta značajka nije omogućena, rezultati pretraživanja neće moći povući podatke iz prethodnih datuma.
1. Ako vas zanima određena aktivnost, odaberite je na popisu **Aktivnosti;** u suprotnom će se prema zadanim postavkama sve aktivnosti vratiti za odabranog korisnika. Imajte na umu da određene aktivnosti možda neće biti dostupne za odabir s **izbornika** Aktivnosti; No te će se stavke nadzora vratiti ako je **odabrana postavka** Prikaži rezultate za sve aktivnosti (zadana postavka).
1. Navedite datumski raspon, a zatim u **polju** Korisnici odaberite korisničko ime za korisnika koji želite istražiti.
1. Odaberite **Pretraživanje**. Aktivnosti se prikazuju u odjeljku **Rezultati**. Za svaku aktivnost možete vidjeti IP adresu.
1. Da biste pogledali pojedinosti, odaberite aktivnost, a zatim **dodatne informacije**.

Dodatne informacije potražite u članku Pretraživanje zapisnika [Office 365 da biste otklonili uobičajene scenarije](https://go.microsoft.com/fwlink/?linkid=2103944).