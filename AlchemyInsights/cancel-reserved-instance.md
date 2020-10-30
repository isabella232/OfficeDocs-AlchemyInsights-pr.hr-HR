---
title: Otkazivanje rezervacije
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003552"
- "6817"
ms.openlocfilehash: 04875e33f07c6d0a4306b3579ef81f2d28c7f506
ms.sourcegitcommit: f8b41ecda6db0b8f64fe0c51f1e8e6619f504d61
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 10/28/2020
ms.locfileid: "48807250"
---
# <a name="cancelling-reservation"></a>Otkazivanje rezervacije

- **Samoposluživanje:** Sami možete otkazati ili promijeniti rezerviranu instancu uz pomoć [portala Azure](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Odaberite rezervaciju, a zatim kliknite povrat novca ili Exchange. Obratite pozornost na to da morate imati pristup vlasniku na nalogu za rezervaciju za razmjenu ili povrat novca. Pristup samo rezerviranju neće vam omogućiti nastavak povrata ili Exchange. Zatražite od vlasnika narudžbe da vam daje pristup nalogu za rezervaciju
- **Pravilnik o sustavu Exchange:** Možete izmijeniti rezervaciju za neku drugu rezervaciju iste vrste – nema **kazni** na Exchange za rezervaciju. Ukupna obveza s novom rezervacijom trebala bi biti veća od iznosa povrata naknade za razmjenu i budućih mjesečna plaćanja (ako je primjenjivo)
- **Pravilnik o povratu novca:** Zbroj povrata i otkazanih budućih uplata ne može premašiti $50.000 USD u 12-mjesečnom prozoru za valjanje. **Trenutno ne naplaćujemo nikakvu kaznu** za povrat novca, no možemo je naplatiti za buduće povrat novca.  
    **Iznimke:** Mogućnosti samoservisiranja i otkazivanja nisu dostupne za korisnike američke vlade za Enterprise sporazum
- **API/PS/CLI** podrška nije dostupna za otkazivanje i povrat [samoposlužnih razmjena i povrat sredstava za rezervaciju za Azure](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)
- Mogućnosti samoservisiranja i otkazivanja nisu dostupne za korisnike američke vlade za Enterprise ugovor. Ostale vrste pretplata na američke vlade, uključujući plaćanje-as-te-Go i CSP su podržane

Dodatne informacije: [Obrada povrata i transakcije u sustavu Exchange](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed)  
Dodatne informacije: [pravila za razmjenu i povrat novca](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)  
Ostala pitanja: [posjetite dokumente rezervirane instance](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Exchange postojeću rezerviranu instancu (samoposluživanje)**

Možete izmijeniti rezervaciju za drugu rezervaciju iste vrste. Možete i vratiti rezervaciju, do $50.000 USD godišnje, ako vam više nije potrebna. Mogućnosti samoservisiranja i otkazivanja nisu dostupne za korisnike američke vlade za Enterprise ugovor. Ostale vrste pretplata na američke vlade, uključujući plaćanje-as-te-Go i CSP, podržane su. Da biste mogli promijeniti ili vratiti postojeću rezervaciju, morate imati pristup vlasniku na nalogu za rezervaciju.

Sljedećim će se koracima voditi postupak dovršetka transakcije

1. Prijavite se na [portal Azure](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Odaberite rezervaciju koje želite vratiti, a zatim kliknite **Exchange**
2. Odaberite VM proizvod koji želite kupiti, a zatim upišite količinu. Provjerite je li novi ukupni zbroj kupnje veći od iznosa povrata ukupno [Odredite veličinu prave veličine prije kupnje](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy)
3. Pregled i dovršetak transakcije

**Povrat za rezerviranu instancu**

Da biste povratili rezervaciju, idite na **Pojedinosti o rezervaciji** i kliknite **povrat novca** .

**Pro-rated povrat:**

**Primjeri zahtjeva za nadoknadu i minimalnim preduvjetima za povrat i razmjenu**  
Ogledni upit:

- Možete kupiti jednogodišnji termin za $120 u siječnju 1.
- 7. travnja želite vratiti ili izmijeniti ovu rezervaciju
- Budući da je rezervacija bila živa za 97 dana, dobit ćete (1-97/365) * $120 natrag. (tj. $88,1). Trenutno ne postoji kazna za povrat novca
- Ako je razmjena, vaša nova Kupnja trebala bi biti veća od $88,1
- Trenutno ne postoji kazna za povrat sredstava

**Primjer rezervacije tarife za naplatu:**

- Kupnja jednogodišnjeg termina RI za $10 mjesečno
- 7. travnja želite vratiti ili izmijeniti ovu rezervaciju
- Budući da se Posljednja uplata dogodila sedam dana, dobit ćete (1-7/31) * $10 natrag. (i.e. $7,74)
- Otkazivanje budućih isplata jest $80. Trenutno ne postoji kazna za povrat novca
- Ovim će se otkazom odbiti $87,74 od vas je ograničenje povrata iznosa od $50.000.
- Ako je razmjena, ukupna vrijednost nove kupnje trebala bi biti veća od $87,74

**Preporučeni dokumenti**

- [Način obrade povrata i transakcije u sustavu Exchange](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed)
- [Pravila za razmjenu i povrat novca](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)