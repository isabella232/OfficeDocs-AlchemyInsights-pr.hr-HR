---
title: Stvaranje oznaka ili grupa uređaja i upravljanje njima
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11446"
- "9003537"
ms.openlocfilehash: 3a7d53beaaf830055904f0634f09a3e9e447006e
ms.sourcegitcommit: 1226e9a9601dc8fc8ec427235f3c2dd88ff84ced
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/02/2021
ms.locfileid: "52731340"
---
# <a name="create-and-manage-device-tags-or-groups"></a>Stvaranje oznaka ili grupa uređaja i upravljanje njima

Dodajte oznake na uređajima da biste stvorili pripadnost logičkoj grupi. Oznake uređaja podržavaju pravilno mapiranje mreže, što omogućuje prilaganje različitih oznaka radi snimanja konteksta i omogućivanja stvaranja dinamičkog popisa u sklopu incidenta. Oznake se mogu koristiti kao filtar u prikazu popisa Uređaji ili za grupiranje uređaja. Dodatne informacije o grupiranje uređaja potražite u članku Stvaranje [oznaka uređaja i upravljanje njima.](/microsoft-365/security/defender-endpoint/machine-tags)

Oznake na uređajima možete dodati na sljedeće:

- Korištenje portala

- Postavljanje vrijednosti ključa registra
 
**Napomena:** Može biti kašnjenja između vremena dodavanja oznake na uređaj i dostupnosti na popisu uređaja i na stranici uređaja.

Da biste dodali oznake uređaja pomoću API-ja, [pogledajte dodavanje ili uklanjanje API oznaka uređaja](/microsoft-365/security/defender-endpoint/add-or-remove-machine-tags).

## <a name="add-and-manage-device-tags-using-the-portal"></a>Dodavanje oznaka uređaja i upravljanje njima pomoću portala

1. Odaberite uređaj na koji želite upravljati oznakama. Uređaj možete odabrati ili potražiti iz bilo kojeg od sljedećih prikaza:

    - **Nadzorna ploča sigurnosnih operacija** U odjeljku Top uređaji s aktivnim upozorenjima odaberite naziv uređaja.
    - **Red čekanja upozorenja** – odaberite naziv uređaja pokraj ikone uređaja iz reda čekanja upozorenja.
    - **Popis uređaji** – na popisu uređaja odaberite naziv uređaja.
    - **Okvir za** pretraživanje – na padajućem izborniku odaberite Uređaj pa unesite naziv uređaja.

    Stranicu upozorenja možete doći i putem prikaza datoteke i IP-a.

1. U **retku Akcija** odgovora odaberite Upravljanje oznakama.

1. Upišite da biste pronašli ili stvorili oznake.

Oznake se dodaju u prikaz uređaja i odražavaju se na prikazu popisa Uređaji. Zatim pomoću filtra Oznake možete vidjeti odgovarajući popis uređaja.

Dodatne informacije potražite u članku [Stvaranje oznaka uređaja i upravljanje njima.](/microsoft-365/security/defender-endpoint/machine-tags)