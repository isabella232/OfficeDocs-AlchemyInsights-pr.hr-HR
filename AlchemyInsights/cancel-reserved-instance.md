---
title: Otkazivanje rezervacije
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
- "9003552"
- "6817"
ms.openlocfilehash: 6b27344b43aa5c20d64d148ff164be805f3b5ef8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819684"
---
# <a name="cancelling-reservation"></a>Otkazivanje rezervacije

- **Samoposlužno:** rezerviranu instancu možete sami otkazati ili zamijeniti putem portala platforme [Microsoft Azure](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Odaberite rezervaciju i kliknite povrat novca ili zamjenu. Imajte na umu da za zamjenu ili povrat novca morate imati vlasnički pristup narudžbi s rezervacijom. Ako imate običan pristup rezervaciji, nećete moći nastaviti s povratom novca ili zamjenom. Zatražite vlasnički pristup narudžbi s rezervacijom od njezinog vlasnika.
- **Pravilnik sustava Exchange:** rezervaciju možete zamijeniti za drugu rezervaciju iste vrste – **nema penalizacije** za zamjenu rezervacije. Ukupna obaveza plaćanja s novom rezervacijom treba biti veća od zbroja iznosa povrata za zamijenjenu rezervaciju i budućih mjesečnih plaćanja (ako je moguće)
- **Pravilnik o povratu novca:** zbroj povrata novca i otkazanih budućih plaćanja ne smije prijeći 50 000 USD tijekom neprekinutog razdoblja od 12 mjeseci. Trenutačno **ne penaliziramo** povrat novca, no to se pri budućim povratima može promijeniti  
    **Iznimke:** mogućnost samoposlužne zamjene i otkazivanja nije dostupna korisnicima Enterprise ugovora s državnom upravom SAD-a
- **Podrška za API/PS/CLI** nije dostupna za otkazivanje i povrat novca [Samoposlužne zamjene i povrati novca za rezervacije servisa na platformi Azure](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)
- Mogućnost samoposlužne zamjene i otkazivanja nije dostupna korisnicima Enterprise ugovora s državnom upravom SAD-a. Podržane su druge vrste pretplata za državnu upravu SAD-a, uključujući Pay-As-You-Go i CSP

Saznajte više: [kako se obrađuju transakcije vraćanja i zamjene](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed)  
Dodatne informacije: [pravilnici o povratu novca i zamjeni](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)  
Ostala pitanja: [posjetite dokumente o rezerviranoj instanci](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Zamjena postojeće rezervirane instance (samoposlužna)**

Rezervaciju možete zamijeniti za drugu rezervaciju iste vrste. Možete dobiti i povrat novca za rezervaciju u iznosu do 50 000 USD godišnje ako vam ona više nije potrebna. Mogućnost samoposlužne zamjene i otkazivanja nije dostupna korisnicima Enterprise ugovora s državnom upravom SAD-a. Podržane su druge vrste pretplata za državnu upravu SAD-a, uključujući Pay-As-You-Go i CSP. Za zamjenu postojeće rezervacije ili povrat novca za nju morate imati vlasnički pristup narudžbi s rezervacijom.

Sljedeći će vas koraci voditi kroz postupak dovršenja transakcije

1. Prijavite se na portal platforme[Microsoft Azure](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Odaberite rezervacije za koje želite povrat novca i kliknite **Zamijeni**
2. Odaberite VM proizvod koji želite kupiti i upišite količinu. Provjerite je li ukupan iznos nove kupnje veći od ukupnog iznosa povrata [Odredite pravu veličinu prije kupnje](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy)
3. Pregled i dovršenje transakcije

**Povrat novca za rezerviranu instancu**

Da biste ostvarili povrat novca za rezervaciju, otvorite **Pojedinosti o rezervaciji** i kliknite **Povrat novca**

**Proporcionalni povrat novca:**

**Primjeri proporcionalnog izračuna i minimalnih zahtjeva za povrat novca i zamjenu**  
Primjer rezervacije unaprijed:

- Kupili ste jednogodišnji RI za 120 USD na dan 1. siječnja
- 7. travnja želite ostvariti povrat novca ili zamijeniti tu rezervaciju
- Budući da se rezervacija koristila 97 dana, dobit ćete povrat u iznosu od (1 – 97/365) * 120 USD. (tj. 88,1 USD). Trenutno nema penalizacije prilikom povrata novca
- U slučaju zamjene nova kupnja treba biti veća od 88,1 USD.
- Trenutno nema penalizacije prilikom povrata novca

**Primjer rezervacije tarife za naplatu:**

- Kupili ste jednogodišnji RI za 10 USD mjesečno
- 7. travnja želite ostvariti povrat novca ili zamijeniti tu rezervaciju
- Budući da je zadnja uplata bila prije 7 dana, dobit ćete povrat od (1 – 7/31) * 10 USD. (tj. 7,74 USD).
- Vrijednost otkazanih budućih uplata iznosi 80 USD. Trenutno nema penalizacije prilikom povrata novca
- To će otkazivanje vaš limit za povrat novca od 50 000 USD umanjiti za 87,74 USD
- U slučaju zamjene ukupna vrijednost nove kupnje treba biti veća od 87,74 USD.

**Preporučeni dokumenti**

- [Kako se obrađuju transakcije vraćanja i zamjene](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed)
- [Pravilnici o povratu novca i zamjeni](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)