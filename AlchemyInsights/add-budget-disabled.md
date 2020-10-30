---
title: Zašto je gumb Dodaj proračun onemogućen za mene?
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
- "9003547"
- "6464"
ms.openlocfilehash: 18edad73f617ba180cb08576ee6e5fa8faf07128
ms.sourcegitcommit: 9a7b85eae0bb775bc2498a83d8f5fedb72a6451e
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 10/27/2020
ms.locfileid: "48807215"
---
# <a name="why-is-the-add-budget-button-disabled-for-me"></a>Zašto je gumb Dodaj proračun onemogućen za mene?

Da biste stvorili proračun, potrebna vam je jedna od sljedećih dozvola:

- Grupa upravljanje, pretplata, dosezi grupe resursa
- Suradnik za upravljanje troškovima
- Vlasnik
- Suradnika
- Samo klijent za Enterprise: upis, odjel, dosezi računa
- Administrator upisa (postavljanje proračuna u opsegu upisa)
- Administrator odjela (postavljanje proračuna u opsegu odjela)
- Vlasnik računa (postavljanje proračuna pri opsegu računa)
- Samo suvremeni korisnički ugovor: račun za naplatu, profil za naplatu, dosezi sekcije fakture
- Stvaranje pretplate na Azure

**Stvorio sam proračun kada je moja cijena za sadašnji mjesec već bila iznad proračuna. Zašto nisam primio upozorenje?**  
Ako ste već premašili zadani prag troška kada ste stvorili proračun koji upozorenje neće pucati. Kada novi ciklus počne, ako prekršiš Prag, uzbuna će se zapaliti.

**Kada očekivati da ću primiti upozorenje nakon što prekoračim jedan od mojih definiranih pragova za upozorenje o proračunu?**  
Proračuni se procjenjuju svakih 4 sata. Podaci o korištenju moraju biti najmanje 8 sati da bi se postigli sustav proračuna. S obzirom na to, upozorenja mogu potrajati i 12 sati nakon što prekoračite prag.

**Zašto je gumb početni datum onemogućen kada odaberem razdoblje ponovnog postavljanja mjeseca ili naplate?**  
Proračuni su poravnani s trenutnim kalendarskim mjesecom ili trenutnim razdobljem naplate (u slučaju kada je odabrana mogućnost naplati mjesečno). Dakle, prije ćemo popuniti tu vrijednost za vas.

**Zašto ne vidim grafikon svojih troškova u iskustvu stvaranja proračuna?**  
Potrebno nam je minimalno 2 mjeseca troška podataka prije nego što možemo prikazati grafikon da biste vam pomogli pri stvaranju proračuna.

**Zašto ne mogu postaviti proračun na pretplatu koju sam upravo stvorio?**  
Nakon stvaranja pretplate podaci su potrebni za 24-48 sati prije postavljanja proračuna.

**Resursi za proračun API-ja**

- [API v1 za proračune](https://docs.microsoft.com/rest/api/consumption/budgets?WT.mc_id=Portal-Microsoft_Azure_Support): nudi operacije za stvaranje i ažuriranje proračuna. Pomoću API-ja za proračune možete postaviti prag proračuna i konfigurirati više upozorenja na vatru dok prilazite tom pragu. Upozorenja mogu pokrenuti automatizaciju e-pošte ili grupe Azure. Pažnja: filtriranje ovog API-ja ne poravnava se pomoću API filtriranja/dimenzija upita.
- [API proračuni v2](https://github.com/Azure/azure-rest-api-specs/blob/master/specification/cost-management/resource-manager/Microsoft.CostManagement/preview/2019-04-01-preview/examples/CreateOrUpdateBudget.json): stvaranje proračuna s većim mogućnostima filtriranja troška od v1. Filtriranje se poravnava s ugovorom koji se koristi u API-Jima upita i dimenzija. Ovo je Preporučeni API za proračune da biste koristili pomicanje naprijed.
- [Dimenzije](https://docs.microsoft.com/rest/api/cost-management/dimensions?WT.mc_id=Portal-Microsoft_Azure_Support): operacije osiguravaju podržane dimenzije za korištenje u različitim dosezi. Pomoću API-ja za dimenzione možete dohvatiti popis dimenzija koje se mogu koristiti kao ulazne podatke za generiranje upita s API-jem upita.
- [Query](https://docs.microsoft.com/rest/api/cost-management/query?WT.mc_id=Portal-Microsoft_Azure_Support): nudi operacije za dohvaćanje skupnih troškova i podataka o korištenju na temelju upita koji isporučujete. Pomoću API-ja UPITA možete navesti željenu filtriranje, sortiranje i grupiranje na svim dostupnim dimenzijama (kojima se pristupa iz API-ja za dimenzije).

**Predviđene troškove**

**Zašto ne vidim prognoze za troškove u analizi troškova?**  
Postoji više razloga zbog kojih bi projekcija predviđanja mogla nedostajati u analizi troškova, a neke od njih su sljedeće:

1. Ako su podaci o troškovima stari manje od 10 dana, grafikon prognoze neće se učitati. Model zahtijeva najmanje 10 dana nedavnih podataka o troškovima za točne projekcije
2. Ako ste odabrali povijesne datume, Grafikon predviđanja neće biti vidljiv. Odaberite datumski raspon s budućim datumom za prikaz grafikona prognoze.
3. Ako vaš račun ima više valuta, grafikon prognoze Projektirat će samo troškove za sve troškove u USD-u.

**Zašto se prognoza ne mijenja kada mijenjam resurse?**  
Model Forecast zahtjeva nekoliko dana da se računa za promjene na računu i ne stvara neposredne projekcije na temelju promjena u resursima  
Za veće korake povećanja ili smanjenja resursa model će potrajati malo dulje da bi se prilagodili ovim promjenama u obzir za anomalije

**Zašto se moja prognoza povećava kada rezerviram rezervaciju ili kupnju tržnice?**  
Model Forecast smatra vaš "stvarni trošak", a ne računa se za korištenje i kupnju odvojeno. Za jednokratnu kupnju model će smanjiti projekcije nakon 10 dana da bi se u obzir došlo do iznenadnog povećanja troškova.

**Želim vidjeti prognoze za jednu dimenziju (npr. Mjerač**  
Vremenska prognoza trenutno podržava projekcije ukupnog troška, a ne za pojedinačne metre. Dakle, kada je "grupirana prema" dimenziji, projekcije će biti za ukupno svih stavki u dimenziji

**Preporučeni dokumenti**

- [Što je upravljanje troškovima za Azure?](https://docs.microsoft.com/azure/cost-management/overview-cost-mgt?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Najbolja praksa upravljanja troškovima za Azure](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Analizirajte troškove i potrošnju](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Istražite i Analizirajte troškove pomoću analize troškova](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Upravljanje troškovima Azure: Cijena](https://azure.microsoft.com/services/cost-management/#pricing)
- [Pregled troškova u analizi troškova](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support#review-costs-in-cost-analysis)
- [Vodič za videozapise: stvaranje proračuna na portalu Azure](https://www.youtube.com/watch?v=ExIVG_Gr45A&t=4s)
- [Preduvjeti za pregledavanje i prilagođavanje proračuna](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#prerequisites)
- [Stvaranje proračuna i upravljanje njima](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#create-a-budget-in-the-azure-portal)
- [Konfiguriranje automatizacije pomoću API-ja za Azure i programa za proračune](https://docs.microsoft.com/azure/cost-management/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#trigger-an-action-group)
- [Korištenje upozorenja o troškovima za praćenje upotrebe i potrošnje](https://docs.microsoft.com/azure/cost-management/cost-mgt-alerts-monitor-usage-spending?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Najbolje prakse za upravljanje troškovima](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)  

**Vodič za videozapise**

- [Stvaranje proračuna na portalu Azure](https://go.microsoft.com/fwlink/?linkid=2146761)
- [Upravljanje troškovima pomoću API-ja za proračune i grupe akcija](https://go.microsoft.com/fwlink/?linkid=2147038)