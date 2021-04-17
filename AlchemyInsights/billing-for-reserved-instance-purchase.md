---
title: Naplata za kupnju rezervirane instance
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
ms.openlocfilehash: 9d71554d2089a6d9e5d4850149d113959f3d43c0
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820314"
---
# <a name="billing-for-reserved-instance-purchase"></a>Naplata za kupnju rezervirane instance

Rezervirana kupnja instance naplaćuje se za način plaćanja vezan uz pretplatu koju odaberete u trenutku kupnje. Vrsta pretplate mora biti poslovni ugovor (broj ponude: MS-AZR-0017P), Pay-As-You-Go (broj ponude: MS-AZR-0003P), Microsoftov korisnički ugovor ili CSP.

- Za pretplatu na velike tvrtke te se naknade oduzimaju od iznosa novčane obveze upisa ili se naplaćuju kao prekomjeran iznos
- Za pretplatu na Pay-As-You-Go te se naknade naplate na kreditnoj kartici ili načinu plaćanja fakture na pretplati

**Otkazivanje rezervacije**

- **Samoposlužno:** Rezerviranu instancu možete otkazati ili sami zamijeniti pomoću [portala Azure](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Odaberite rezervaciju i kliknite na povrat novca ili zamjenu. Imajte na umu da morate imati vlasnički pristup na nalogu za rezervaciju da biste razmjenili ili povrat novca. Pristup samo rezervaciji neće vam dopustiti nastavak povrata novca ili zamjene. Zatražite od vlasnika narudžbe rezervacije da vam vlasniku da pristup nalogu za rezervaciju
- **Pravilnik sustava Exchange:** Možete zamijeniti rezervaciju za drugu rezervaciju iste vrste – nema novčanih **kazni za razmjenu** rezervacija. Ukupna obveza s novom rezervacijom trebala bi biti veća od zbroja iznosa povrata valutne rezervacije i budućih mjesečnih uplata (ako je primjenjivo)
- **Pravilnik o povratu novca:** Iznos povrata novca i otkazana buduća plaćanja ne smiju premašiti 50 000 USD u 12-mjesečnom prozoru za valjanje. Trenutačno ne **naplaćujemo novčanu naknadu za** povrat novca, ali bismo je mogli naplatiti za buduće povrate novca

**Iznimke:** Mogućnost samoposlužne razmjene i otkazivanja nije dostupna korisnicima ugovora o korporacijama u SAD-u

- **Podrška za API/PS/CLI** nije dostupna za otkazivanje i povrat samoposlužnih [razmjena i povrata novca za rezervacije na servisu Azure](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)
- Mogućnost samoposlužne razmjene i otkazivanja nije dostupna korisnicima ugovora o korporacijama američke vlade. Podržane su druge vrste pretplata za us Government, uključujući Pay-As-You-Go i CSP

Saznajte više: [Kako se obrađuju transakcije](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed) vraćanja i razmjene Saznajte više : Pravila sustava Exchange i [povrata](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies) novca Ostala pitanja: [Posjetite dokumente rezerviranih instanci](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Exchange postojeća rezervirana instanca (samoposlužna)**

Možete zamijeniti rezervaciju za drugu rezervaciju iste vrste. Ako vam više nije potrebna, možete vratiti i rezervaciju do 50 000 USD godišnje. Mogućnost samoposlužne razmjene i otkazivanja nije dostupna korisnicima ugovora o korporacijama američke vlade. Podržane su druge vrste pretplate američke vlade, uključujući Pay-As-You-Go i CSP. Da biste mogli zamijeniti ili vratiti postojeću rezervaciju, morate imati vlasnički pristup na nalogu za rezervaciju.

Sljedeći koraci vodit će o postupku za dovršetak transakcije

1.Prijavite se na [portal Azure](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Odaberite rezervacije koje želite vratiti, a zatim **kliknite Exchange** 2.Odaberite proizvod za virtualno računalo koji želite kupiti i upišite količinu. Provjerite je li novi ukupni iznos kupnje veći od ukupnog iznosa povrata Odredite [pravu veličinu prije kupnje](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy).
3.Pregledajte i dovršite transakciju

**Povrat novca za rezerviranu instancu**

Da biste povrat novca povrat novca za rezervaciju, idite **na Detalji o rezervaciji** i kliknite **Povrat novca**

**Povrat novca za pro-ocijenjenu vrijednost:**

**Pro-ration and minimum requirement examples for refund and exchange** Upfront reservation example:

- Jednogodišnji RI za 120 KN 1. siječnja
- 7. travnja želite vratiti ili zamijeniti ovu rezervaciju
- Budući da je rezervacija uživo 97 dana, dobiti ćete (1-97/365) * $120 natrag. (npr. 88,1 KN). Trenutno nema novčane kazne za povrat novca
- Ako razmjenu mijenjate, vaša nova kupnja trebala bi biti veća od 88,1 KN
- Trenutno nema novčane kazne za povrat novca

**Primjer rezervacije plana naplate:**

- Za 10 USD mjesečno kupujete jednogodišnji RI
- 7. travnja želite vratiti ili zamijeniti ovu rezervaciju
- Budući da se zadnja uplata dogodila 7 dana, dobiti ćete (1-7/31) * $10 natrag. (npr. 7,74 KN)
- Budući otkazani uplata iznose 80 KN. Trenutno nema novčane kazne za povrat novca
- Ovo otkazivanje oduzima 87,74 KN od vas je ograničenje povrata od 50 000 KN
- Ako se razmjena promijeni, ukupna vrijednost nove kupnje trebala bi biti veća od 87,74 KN

**Nije moguće vidjeti fakturu za posljednje razdoblje naplate**

Neki od mogućih razloga zbog kojih možda ne vidite fakturu:

- Uz pretplatu imate mjesečni iznos kredita koji niste prekoračili ili imate besplatnu probnu verziju. Faktura se generira samo kada dugujete novac
- To je manje od 30 dana od dana kada ste se pretplatili na Azure
- Faktura još nije generirana. Pričekajte do kraja razdoblja naplate
- Ako niste administrator računa, starije fakture možda vam neće biti dostupne

**Preuzimanje fakture s portala Azure (.pdf)**

- Odaberite pretplatu na [stranici Pretplate](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) na portalu Azure [kao korisnika s pristupom fakturama](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- Odaberite **Fakture**
- Kliknite **Preuzmi fakturu** da biste pogledali kopiju PDF fakture. Ako piše **Nije dostupno**, pogledajte odjeljak Zašto ne vidim [fakturu za zadnje razdoblje naplate?](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice)

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

Ostala pitanja: [Posjetite dokumente rezerviranih instanci](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Preporučeni dokumenti**

- [Osnove naplate](https://docs.microsoft.com/partner-center/billing-basics/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Razumijevanje primjene popusta rezervirane instance](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Preuzimanje ili prikaz fakture za naplatu na servisu Azure i podataka o dnevnom korištenju](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Razumijevanje primjene popusta rezervirane instance](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Korištenje rezerviranih instanci za pretplatu na Pay-As-You-Go](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Razumijevanje korištenja rezerviranih instanci za prijavu na Enterprise](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage-ea/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Troškovi softvera za Windows koji nisu obuhvaćeni rezerviranim instancama](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Rezervirane instance u partnerskom središnjem davatelju rješenja u oblaku (CSP)](https://docs.microsoft.com/partner-center/azure-reservations/?WT.mc_id=Portal-Microsoft_Azure_Support)