---
title: Zašto je gumb Dodaj proračun onemogućen?
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
- "9003547"
- "6464"
ms.openlocfilehash: 426a54ea22490dcc47f40fd990654b2cf051a058
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51822627"
---
# <a name="why-is-the-add-budget-button-disabled-for-me"></a>Zašto je gumb Dodaj proračun onemogućen?

Da biste stvorili proračun, potrebna vam je jedna od sljedećih dozvola:

- Management Group, Subscription, Resource Group Scopes
- Suradnik za upravljanje troškovima
- Vlasnik
- Suradnik
- Samo poslovni korisnici: registracija, odjel, opseg računa
- Administrator za prijavu (postavljanje proračuna u opsegu registracije)
- Administrator odjela (postavljanje proračuna u opsegu odjela)
- Vlasnik računa (postavljanje proračuna u opsegu računa)
- Samo moderni klijentski ugovor: račun za naplatu, profil za naplatu, opsege sekcije Faktura
- Kreator pretplate na Azure

**Stvorio sam proračun kada mi je cijena trenutnog mjeseca već bila prekoraenom proračunu. Zašto nisam primio upozorenje?**  
Ako ste već prekoračili određeni prag troškova prilikom stvaranja proračuna koji upozorenje neće ispaivati. Kada započne novi ciklus, ako prekršite prag, upozorenje će se zapaliti.

**Kada očekivati primanje upozorenja nakon što prekoračim jedan od definiranih pragova upozorenja o proračunu?**  
Proračuni se vrednuju svaka 4 sata. Da bi podaci o korištenju došli do sustava proračuna, potrebno je najmanje 8 sati. S obzirom na to, upozorenja mogu potrajati i do 12 sati nakon što prekoračite prag.

**Zašto je gumb Početni datum onemogućen prilikom odabira razdoblja za ponovno postavljanje mjeseca ili naplate?**  
Proračuni su usklađeni s trenutnim kalendarskim mjesecom ili trenutnim razdobljem naplate (u slučaju kada je odabran mjesec naplate). Stoga tu vrijednost unaprijed popunjavamo za vas.

**Zašto ne vidim grafikon troškova u iskustvu stvaranja proračuna?**  
Da bismo mogli iscrtavanje grafikona, potrebno nam je najmanje 2 mjeseca podataka o cijeni da bismo vam pomogli pri stvaranju proračuna.

**Zašto ne mogu postaviti proračun za pretplatu koju sam upravo stvorio?**  
Nakon stvaranja pretplate podaci se obrađuju od 24 do 48 sati prije postavljanja proračuna.

**Resursi API-ja za proračun**

- [API za proračune v1:](https://docs.microsoft.com/rest/api/consumption/budgets?WT.mc_id=Portal-Microsoft_Azure_Support)pruža operacije za stvaranje i ažuriranje proračuna. Pomoću API-ja proračuni možete postaviti prag proračuna i konfigurirati više upozorenja da se ispale dok se približavate tom pragu. Upozorenja mogu pokrenuti e-poštu ili akcijsku grupu servisa Azure radi automatizacije. Napomena: filtriranje za ovaj API ne poravnava se s filtriranje API-ja upita / dimenzijama.
- [API za proračune v2:](https://github.com/Azure/azure-rest-api-specs/blob/master/specification/cost-management/resource-manager/Microsoft.CostManagement/preview/2019-04-01-preview/examples/CreateOrUpdateBudget.json)stvaranje proračuna s većim mogućnostima filtriranja troškova od v1. Filtriranje se poravnava s ugovorom koji se koristi u API-jem za upite i dimenzije. To je preporučeni API za proračune koji se koristi za kretanje unaprijed.
- [Dimenzije:](https://docs.microsoft.com/rest/api/cost-management/dimensions?WT.mc_id=Portal-Microsoft_Azure_Support)omogućuje operacije da biste dobili podržane dimenzije za korištenje u različitim opsegima. Pomoću API-ja dimenzije možete dohvatiti popis dimenzija koje se mogu koristiti kao unosi za generiranje upita pomoću API-ja za upite.
- [Upit:](https://docs.microsoft.com/rest/api/cost-management/query?WT.mc_id=Portal-Microsoft_Azure_Support)omogućuje operacije za prikupljanje podataka o troškovima i korištenju na temelju upita koji nadodijelite. Pomoću API-ja za upite možete odrediti željeno filtriranje, sortiranje i grupiranje na svim dostupnim dimenzijama (kojima se pristupa putem API-ja za dimenzije).

**Predviđanje troškova**

**Zašto u analizi troškova ne vidim predviđanja troškova?**  
U analizi troškova postoji više razloga zbog kojih predviđanje možda nedostaje u analizi troškova, a neki su od njih sljedeći:

1. Ako su podaci o cijeni manji od 10 dana, grafikon predviđanja neće se učitati. Model zahtijeva najmanje 10 dana nedavnih podataka o troškovima za točne projekcije
2. Ako ste odabrali povijesne datume, grafikon predviđanja neće biti vidljiv. Odaberite raspon datuma s budućim datumima za prikaz grafikona predviđanja
3. Ako vaš račun ima više valuta, na grafikonu predviđanja troškovi će biti samo za "Svi troškovi u USD"

**Zašto se predviđanje ne mijenja prilikom promjene resursa?**  
Za model predviđanja potrebno je nekoliko dana da bi se u obzir uzimali promjene na računu i ne bi se odmah projekcije temeljili na promjenama resursa  
Za veće korake povećanja ili smanjenja resursa model će se malo dulje prilagođavati tim promjenama radi računa o anomalijama

**Zašto se predviđanje povećava nakon kupnje rezervacije ili trgovine?**  
U modelu predviđanja razmatra se vaš "stvarni trošak" i ne računa se zasebno za korištenje i kupnju. Za jednu kupnju model će smanjiti projekcije nakon 10 dana da bi se u obzir uzmu nagli porast troškova

**Želim vidjeti predviđanja za jednu dimenziju (npr. Metar)**  
Predviđanje trenutno podržava projekcije ukupnih troškova, a ne za pojedinačne brojila. Stoga, kada je dimenzija "Grupirano po", projekcije će biti za ukupne stavke u dimenziji

**Preporučeni dokumenti**

- [Što je Azure Cost Management?](https://docs.microsoft.com/azure/cost-management/overview-cost-mgt?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Najbolje prakse za upravljanje troškovima na servisu Azure](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Analiza troškova i potrošnje](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Istraživanje i analiza troškova pomoću analize troškova](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Upravljanje troškovima servisa Azure: cijene](https://azure.microsoft.com/services/cost-management/#pricing)
- [Pregled troškova u analizi troškova](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support#review-costs-in-cost-analysis)
- [Vodič za videozapise: Stvaranje proračuna na portalu Azure](https://www.youtube.com/watch?v=ExIVG_Gr45A&t=4s)
- [Preduvjeti za prikaz i prilagodbu proračuna](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#prerequisites)
- [Stvaranje proračuna i upravljanje njima](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#create-a-budget-in-the-azure-portal)
- [Konfiguriranje automatizacije pomoću akcijskih grupa i API-ja za proračune servisa Azure](https://docs.microsoft.com/azure/cost-management/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#trigger-an-action-group)
- [Praćenje korištenja i potrošnje pomoću upozorenja o troškovima](https://docs.microsoft.com/azure/cost-management/cost-mgt-alerts-monitor-usage-spending?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Najbolje prakse za upravljanje troškovima](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)  

**Videozapisi s vodičima**

- [Stvaranje proračuna na portalu Azure](https://go.microsoft.com/fwlink/?linkid=2146761)
- [Upravljanje troškovima pomoću API-ja za proračune i akcijskih grupa](https://go.microsoft.com/fwlink/?linkid=2147038)