---
title: Kupnja rezervirane instance za naplatu
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6814"
- "9003552"
ms.openlocfilehash: 6cdcb5af27a475cc838eb434ff025eb18356360c
ms.sourcegitcommit: 1ac3474897abb7c4969e222f934294e05f468536
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 10/30/2020
ms.locfileid: "48823003"
---
# <a name="billing-for-reserved-instance-purchase"></a>Kupnja rezervirane instance za naplatu

Kupnja rezervirane instance naplaćuje se načinu plaćanja vezan uz pretplatu koju odaberete u vrijeme kupnje. Vrsta pretplate mora biti korporacijski ugovor (broj ponude: MS-AZR-0017P), Pay-It-You-Go (broj ponude: MS-AZR-0003P), Microsoftov ugovor o klijentu ili CSP.

- Za pretplatu na Enterprise, naknade se odbijaju od iznosa novčane obveze za upis ili se naplaćuju kao prestar
- Za pretplatu na plaćanje-kao-te-go naknade se naplaćuju na kreditnu karticu ili način plaćanja na fakturi na pretplati.

**Otkazivanje rezervacije**

- **Samoposluživanje:** Sami možete otkazati ili promijeniti rezerviranu instancu uz pomoć [portala Azure](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Odaberite rezervaciju, a zatim kliknite povrat novca ili Exchange. Obratite pozornost na to da morate imati pristup vlasniku na nalogu za rezervaciju za razmjenu ili povrat novca. Pristup samo rezerviranju neće vam omogućiti nastavak povrata ili Exchange. Zatražite od vlasnika narudžbe da vam daje pristup nalogu za rezervaciju
- **Pravilnik o sustavu Exchange:** Možete izmijeniti rezervaciju za neku drugu rezervaciju iste vrste – nema **kazni** na Exchange za rezervaciju. Ukupna obveza s novom rezervacijom trebala bi biti veća od iznosa povrata naknade za razmjenu i budućih mjesečna plaćanja (ako je primjenjivo)
- **Pravilnik o povratu novca:** Zbroj povrata i otkazanih budućih uplata ne može premašiti $50.000 USD u 12-mjesečnom prozoru za valjanje. **Trenutno ne naplaćujemo nikakvu kaznu** za povrat novca, no možemo je naplatiti za buduće povrat novca.

**Iznimke:** Mogućnosti samoservisiranja i otkazivanja nisu dostupne za korisnike američke vlade za Enterprise sporazum

- **API/PS/CLI** podrška nije dostupna za otkazivanje i povrat [samoposlužnih razmjena i povrat sredstava za rezervaciju za Azure](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)
- Mogućnosti samoservisiranja i otkazivanja nisu dostupne za korisnike američke vlade za Enterprise ugovor. Ostale vrste pretplata na američke vlade, uključujući plaćanje-as-te-Go i CSP su podržane

Dodatne informacije: [upute za vraćanje i razmjenu transakcija](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed) potražite u članku dodatne informacije: [razmjena i pravila povrata](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies) drugih pitanja: [posjetite dokumente rezervirane instance](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Exchange postojeću rezerviranu instancu (samoposluživanje)**

Možete izmijeniti rezervaciju za drugu rezervaciju iste vrste. Možete i vratiti rezervaciju, do $50.000 USD godišnje, ako vam više nije potrebna. Mogućnosti samoservisiranja i otkazivanja nisu dostupne za korisnike američke vlade za Enterprise ugovor. Ostale vrste pretplata na američke vlade, uključujući plaćanje-as-te-Go i CSP, podržane su. Da biste mogli promijeniti ili vratiti postojeću rezervaciju, morate imati pristup vlasniku na nalogu za rezervaciju.

Sljedećim će se koracima voditi postupak dovršetka transakcije

1. prijavite se na [portal Azure](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Odaberite rezervaciju koje želite vratiti, a zatim kliknite **Exchange** 2. Odaberite VM proizvod koji želite kupiti, a zatim upišite količinu. Provjerite je li novi ukupni iznos kupnje više od iznosa povrata ukupno [određuje odgovarajuću veličinu prije kupnje](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy).
3. Pregledajte i dovršite transakciju

**Povrat za rezerviranu instancu**

Da biste povratili rezervaciju, idite na **Pojedinosti o rezervaciji** i kliknite **povrat novca** .

**Pro-rated povrat:**

**Primjeri zahtjeva za nadoknadu i minimalnim preduvjetima za povrat i razmjenu** Ogledni upit:

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

**Nije moguće vidjeti fakturu za posljednje razdoblje naplate**

Neki od mogućih razloga zbog kojih možda nećete vidjeti fakturu:

- Imate mjesečni kreditni iznos s pretplatom koju niste premašili ili imate besplatnu probnu verziju. Faktura se generira samo kada dugujete novac
- To je manje od 30 dana od dana kada ste se pretplatili na Azure
- Faktura još nije generirana. Čekanje na kraj razdoblja naplate
- Ako niste administrator računa, starije fakture možda vam neće biti dostupne.

**Preuzimanje fakture iz portala Azure (. PDF)**

- Odaberite pretplatu na stranici [pretplate](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) na portalu Azure kao [korisnika s pristupom računima](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- Odabir **faktura**
- Kliknite **Preuzmi fakturu** da biste pogledali kopiju PDF fakture. Ako kaže da **nije dostupno** , pročitajte članak [Zašto ne vidim fakturu za posljednje razdoblje naplate?](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice)

**Primanje fakture u poruci e-pošte (. PDF)**

- Odaberite pretplatu na stranici [pretplate](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) . Kliknite **fakture** Pa pošaljite e-poštom moj račun
- Kliknite **Uključivanje** i prihvaćanje uvjeta. Morat ćete se uključiti u svaku pretplatu koju posjedujete

Pažnja: ako ne dobijete poruku e-pošte nakon praćenja koraka, provjerite je li vaša adresa e-pošte ispravna u [postavkama komunikacije na profilu](https://account.windowsazure.com/profile)

**Preuzimanje podataka o korištenju s portala Azure**

- Prijavite se u [centar za Azure račun](https://account.windowsazure.com/Subscriptions) kao [administrator računa](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#whoisaa)
- Odaberite pretplatu za koju želite podatke o fakturi i korištenju
- Odabir **povijesti naplate**
- Odaberite **Prikaz sadašnje naredbe** da biste vidjeli procjenu troškova u trenutku stvaranja procjene.
- Odaberite **Preuzmi upotrebu** da biste svakodnevno preuzeli podatke o korištenju u obliku CSV datoteke. Ako vam se prikazuje dvije verzije dostupne, preuzmite verziju 2

Ostala pitanja: [posjetite dokumente rezervirane instance](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Preporučeni dokumenti**

- [Osnove naplate](https://docs.microsoft.com/partner-center/billing-basics/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Objašnjenje kako se primjenjuje rezervirani popust instance](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Preuzimanje ili prikaz fakture za naplatu Azure i dnevnih podataka o korištenju](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Objašnjenje kako se primjenjuje rezervirani popust instance](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Korištenje rezervirane instance za pretplatu](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Korištenje korištenja rezerviranih instanci za upis u Enterprise](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage-ea/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Troškovi softvera u sustavu Windows nisu obuhvaćeni rezerviranim slučajevima](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Rezervirane instance u programu partner Central Cloud solution provider (CSP)](https://docs.microsoft.com/partner-center/azure-reservations/?WT.mc_id=Portal-Microsoft_Azure_Support)