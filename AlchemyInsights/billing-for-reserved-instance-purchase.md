---
title: Naplata instance rezervirane za kupnju
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6814"
- "9003552"
ms.openlocfilehash: 00565470de388165e64c45879c22fd5064b4adc695151edaf58878f38a481ff2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54104012"
---
# <a name="billing-for-reserved-instance-purchase"></a>Naplata instance rezervirane za kupnju

Kupnja rezervirane instance naplaćuje se načinom plaćanja vezanim uz pretplatu koju odaberete u trenutku kupnje. Vrsta pretplate mora biti Enterprise Agreement (broj ponude: MS-AZR-0017P), plaćanje prema potrošnji (broj ponude: MS-AZR-0003P), Microsoftov ugovor s klijentom ili CSP.

- Za pretplatu na razini korporacije, troškovi se odbijaju od salda novčanih obveza upisa ili se naplaćuju kao višak
- Za pretplatu plaćanja prema potrošnji, troškovi se naplaćuju s kreditne kartice ili putem načina plaćanja računa na pretplatu

**Otkazivanje rezervacije**

- **Samoposlužno:** rezerviranu instancu možete sami otkazati ili zamijeniti putem portala platforme [Microsoft Azure](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Odaberite rezervaciju i kliknite povrat novca ili zamjenu. Imajte na umu da za zamjenu ili povrat novca morate imati vlasnički pristup narudžbi s rezervacijom. Ako imate običan pristup rezervaciji, nećete moći nastaviti s povratom novca ili zamjenom. Zatražite vlasnički pristup narudžbi s rezervacijom od njezinog vlasnika.
- **Pravilnik sustava Exchange:** rezervaciju možete zamijeniti za drugu rezervaciju iste vrste – **nema penalizacije** za zamjenu rezervacije. Ukupna obaveza plaćanja s novom rezervacijom treba biti veća od zbroja iznosa povrata za zamijenjenu rezervaciju i budućih mjesečnih plaćanja (ako je moguće)
- **Pravilnik o povratu novca:** zbroj povrata novca i otkazanih budućih plaćanja ne smije prijeći 50 000 USD tijekom neprekinutog razdoblja od 12 mjeseci. Trenutačno **ne penaliziramo** povrat novca, no to se pri budućim povratima može promijeniti

**Iznimke:** mogućnost samoposlužne zamjene i otkazivanja nije dostupna korisnicima Enterprise ugovora s državnom upravom SAD-a

- **Podrška za API/PS/CLI** nije dostupna za otkazivanje i povrat novca [Samoposlužne zamjene i povrati novca za rezervacije servisa na platformi Azure](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)
- Mogućnost samoposlužne zamjene i otkazivanja nije dostupna korisnicima Enterprise ugovora s državnom upravom SAD-a. Podržane su druge vrste pretplata za državnu upravu SAD-a, uključujući Pay-As-You-Go i CSP

Saznajte više : [Kako se obrađuju](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed) transakcije vraćanja i razmjene Saznajte više : [Exchange](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies) i Pravila povrata novca Ostala pitanja: [Posjetite dokumente rezerviranih instanci](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Zamjena postojeće rezervirane instance (samoposlužna)**

Rezervaciju možete zamijeniti za drugu rezervaciju iste vrste. Možete dobiti i povrat novca za rezervaciju u iznosu do 50 000 USD godišnje ako vam ona više nije potrebna. Mogućnost samoposlužne zamjene i otkazivanja nije dostupna korisnicima Enterprise ugovora s državnom upravom SAD-a. Podržane su druge vrste pretplata za državnu upravu SAD-a, uključujući Pay-As-You-Go i CSP. Za zamjenu postojeće rezervacije ili povrat novca za nju morate imati vlasnički pristup narudžbi s rezervacijom.

Sljedeći će vas koraci voditi kroz postupak dovršenja transakcije

1.Prijavite se na [portal Azure](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Odaberite rezervacije koje želite vratiti, a zatim **kliknite Exchange** 2.Odaberite proizvod za virtualno računalo koji želite kupiti i upišite količinu. Provjerite je li novi ukupni iznos kupnje veći od ukupnog iznosa povrata Odredite [pravu veličinu prije kupnje](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy).
3.Pregledajte i dovršite transakciju

**Povrat novca za rezerviranu instancu**

Da biste ostvarili povrat novca za rezervaciju, otvorite **Pojedinosti o rezervaciji** i kliknite **Povrat novca**

**Proporcionalni povrat novca:**

**Pro i minimalni primjeri zahtjeva za povrat novca i zamjenu** Upfront reservation example:

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

**Nije moguće vidjeti fakturu za posljednje razdoblje naplate**

Neki od mogućih razloga zbog kojih možda ne vidite fakturu:

- Uz pretplatu imate mjesečni iznos kredita koji niste prekoračili ili imate besplatnu probnu verziju. Faktura se generira samo kada dugujete novac
- To je manje od 30 dana od dana kada ste se pretplatili na Azure
- Faktura još nije generirana. Pričekajte do kraja razdoblja naplate
- Ako niste administrator računa, starije fakture možda vam neće biti dostupne

**Preuzimanje fakture s portala Azure (.pdf)**

- Odaberite pretplatu na [stranici Pretplate](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) na portalu Azure [kao korisnika s pristupom fakturama](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- Odaberite **Fakture**
- Kliknite **Preuzmi fakturu** da biste prikazali kopiju PDF računa. Ako piše **Nije dostupno**, pročitajte odjeljak [Zašto ne vidim fakturu za zadnje razdoblje naplate?](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice)

**Primanje fakture e-poštom (.pdf)**

- Odaberite pretplatu na [stranici](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) Pretplate. Kliknite **Fakture, a zatim** Pošalji e-poštu na moju fakturu
- Kliknite **uključite se** i prihvatite uvjete. Morat ćete se uključiti za svaku pretplatu koju posjedujete

Napomena: ako nakon sljedećih koraka ne slijedite korake, provjerite je li vaša adresa e-pošte točna u [preferencama komunikacije na profilu](https://account.windowsazure.com/profile)

**Preuzimanje podataka o korištenju s portala Azure**

- Prijavite se u [Centar za račun za Azure](https://account.windowsazure.com/Subscriptions) kao administrator [računa](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#whoisaa)
- Odaberite pretplatu za koju želite podatke o fakturi i korištenju
- Odaberite **Povijest naplate**
- Odaberite **Prikaz trenutne** izjave da biste vidjeli procjenu troškova u trenutku generiranja procjene
- Odaberite **Preuzmi** korištenje da biste podatke o dnevnom korištenju preuzeli kao CSV datoteku. Ako vam se dostupne dvije verzije, preuzmite verziju 2

Ostala pitanja: [posjetite dokumente o rezerviranoj instanci](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Preporučeni dokumenti**

- [Osnove naplate](https://docs.microsoft.com/partner-center/billing-basics/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Razumijevanje primjene popusta rezervirane instance](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Preuzimanje ili prikaz fakture za naplatu na servisu Azure i podataka o dnevnom korištenju](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Razumijevanje primjene popusta rezervirane instance](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Korištenje rezerviranih instanci za pretplatu na Pay-As-You-Go](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Razumijevanje korištenja rezerviranih instanci za prijavu na Enterprise](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage-ea/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Windows troškovi softvera koji nisu obuhvaćeni rezerviranim instancama](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Rezervirane instance u programu Partner Central Davatelj usluga u oblaku (CSP)](https://docs.microsoft.com/partner-center/azure-reservations/?WT.mc_id=Portal-Microsoft_Azure_Support)