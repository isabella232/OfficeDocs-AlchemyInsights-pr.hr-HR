---
title: Otklanjanje poteškoća s grupnim pitanjima
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7814"
- "9004358"
ms.openlocfilehash: 7e2957a27305e8fb0bfd10e21189cef9870c5aaa
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 01/18/2021
ms.locfileid: "50713437"
---
# <a name="troubleshoot-group-issues"></a>Otklanjanje poteškoća s grupnim pitanjima

**Moram dodijeliti grupu na ulogu Azure AD**

Da biste grupu Azure Active Directory (AD) dodijelili u ulogu Azure AD, slijedite sljedeće korake:

1. Stvaranje nove grupe – stvaranje nove grupe:

    je. Prijavite se u centar za administratore servisa Azure s povlaštenim administratorima i dozvolama za globalne administratore. 
    b. Odaberite Azure Active Directory > grupe > sve grupe > nova grupa. 
    c. Stvaranje grupe.

2. Dodijelite ulogu grupi bilo tijekom stvaranja grupe ili nakon stvaranja grupe.

    je. Da biste grupi dodijelili ulogu u vrijeme stvaranja grupe, odaberite grupu za uključivanje i isključivanje servisa Azure, a zatim stvorite grupu.
    b. Da biste grupi dodijelili ulogu nakon stvaranja, dođite do kartice dodijeljene uloge za novostvorenu grupu i dodijelite ulogu grupi.

**Moram upravljati članstvom grupe koja je dodijeljena ulozi za Azure AD**

1. Da biste spriječili povećanje privilegija, prema zadanim postavkama samo povlašteni administrator uloga i globalni administrator mogu izmijeniti članstvo u grupi koja je dodijeljena ulozi. Oni mogu, međutim, odabrati dodjelu vlasnika za takvu grupu i delegirati taj zadatak. Dodatne informacije potražite u članku [korištenje grupa u oblaku za upravljanje dodjelama uloga u servisu Azure Active Directory](https://docs.microsoft.com/azure/active-directory/roles/groups-concept).
2. Najčešća pitanja i Savjeti za otklanjanje poteškoća za dodjelu uloga grupama u servisu Azure AD potražite [u članku Otklanjanje poteškoća s ulogama koje su dodijeljene grupama oblaka](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting).

**Dinamičke grupe**

1. Ako ne možete pronaći ugrađene korisničke atribute, provjerite je li atribut na popisu podržanih svojstava.
2. Ako tražite ugrađene atribute uređaja, provjerite je li atribut na popisu atributa uređaja. 
3. Osim ugrađenih atributa korisnika i uređaja, možete koristiti i [atribute proširenja](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-dynamic-membership#extension-properties-and-custom-extension-properties). Nakon sinkronizacije atributa proširenja iz lokalnog sustava Windows Server AD ili iz povezane aplikacije SaaS, atributi bi trebali biti vidljivi na padajućem popisu sastavljača pravila. Naziv prilagođenog atributa može se pronaći u direktoriju tako da upita korisničkog atributa pomoću komponente PowerShell i traži naziv atributa. To se može koristiti i prilikom izrade pravila u sintaksi pravila.
4. Pobrinite se da vaš stanar ima odgovarajuću licencu. Dinamičke grupe zahtevaju da stanar ima licencu za Azure AD P1 Premium. Popis licenci za Azure AD možete pristupiti [ovdje](https://azure.microsoft.com/pricing/details/active-directory/). Enterprise Mobility + tarife za sigurnosno licenciranje možete pristupiti [ovdje](https://www.microsoft.com/microsoft-365/enterprise-mobility-security/compare-plans-and-pricing).
5. Provjerite je li uloga korisnika koja stvara dinamičku grupu globalni administrator, Intune administrator, administrator grupe ili administrator korisnika.
6. Ostavite vrijeme da se grupa popunjava. Ovisno o veličini vašeg stanara, grupa može potrajati i do 24 sata radi otvaranja po prvi put ili nakon promjene pravila.
7. Dodatne informacije potražite u članku [Stvaranje pravila utemeljenih na atributima za dinamično članstvo u grupi](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-dynamic-membership).

**Moram izbrisati grupu**

1. Grupe se mogu izbrisati iz direktorija pomoću Remove-AzureADGroup cmdleta u modulu Azure AD PowerShell.
2. Prije nego što pokušate izbrisati sinkroniziranu grupu u servisu Azure AD, provjerite jeste li izbrisali sve dodijeljene licence da biste izbjegli pogreške.
3. Dodatne informacije o brisanju grupa potražite u članku [Brisanje grupe pomoću dodijeljene licence](https://docs.microsoft.com/azure/active-directory/enterprise-users/licensing-group-advanced#deleting-a-group-with-an-assigned-license).

**Moram vratiti izbrisanu grupu**

1. Ako je grupa sustava Office 365 izbrisana, može se vratiti samo do 30 dana prije nego što se pojavi trajno brisanje. Kada se jednom trajno izbriše, grupa se više ne može vratiti. Saznajte više o vraćanju grupa [ovdje](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted).
2. Ta funkcija nije podržana za sigurnosne grupe i grupe za raspodjelu.
3. Provjerite jeste li ovlašteni za vraćanje grupe sustava Office 365. Globalni administratori, administratori grupe, administratori korisničkog računa, Intune administratore servisa, partner Tier1 ili tier2 Support, a vlasnik grupe može vratiti grupu.
4. Kada je dinamička grupa izbrisana i vraćena, ona se smatra novom grupom i ponovno je nastanjena u skladu s pravilom. Ovaj postupak može potrajati i do 24 sata.
5. Dodatne informacije o vraćanju izbrisane grupe potražite u članku [Vraćanje izbrisane grupe sustava Office 365 u servisu Azure Active Directory](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted).

**Konfiguracija pravilnika o isteku grupe**

1. Te su funkcije podržane samo za grupe sustava Office 365, ali ne i za sigurnosne grupe i grupe za raspodjelu nisu podržane.
2. Konfiguriranje i korištenje pravilnika o isteku za grupe sustava Office 365 potrebna je licenca za Azure AD Premium.
3. Trenutno se samo jedno pravilo isteka može konfigurirati za grupe sustava Office 365 na zakupcu.
4. U grupi možete obnoviti samo globalne administratore, administratore grupe, korisničke administratore i vlasnika grupe.
5. Ako je grupa sustava Office 365 istekla, ona se briše i može se vratiti samo do 30 dana prije isteka trajnog brisanja. Kada se jednom trajno izbriše, grupa se više ne može vratiti. Saznajte više o vraćanju grupa [ovdje](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted).

**Automatsko obnavljanje utemeljeno na aktivnostima**

Korisničke aktivnosti iz sustava SharePoint, Outlook i timovi mogu pokrenuti grupu automatskog obnavljanja. Aktivnosti se provjeravaju na 35 dana prije isteka grupe. Ako tijekom postojećeg životnog ciklusa grupe postoji aktivnost, grupa će se automatski obnoviti, a obavijesti e-poštom neće biti poslane vlasnicima grupa.

**Vrijeme obavijesti za istekle grupe**

1. Obavijesti e-poštom šalju se vlasnicima grupa sustava Office 365 30 dana, 15 dana i 1 dan prije isteka grupe.
2. Kada prvi put postavite isteku, sve grupe starije od intervala isteka postavljeni su na 35 dana do isteka.
3. Datum isteka grupe izračunava se na temelju datuma obnove grupe, a ne na temelju datuma ažuriranog pravilnika. Ako je pravilnik o isteku ažuriran, Datum isteka neće se promijeniti.
4. Dodatne informacije potražite u članku [Grupiranje pravilnika o isteku i obnove e-pošte](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-lifecycle) te [Vraćanje izbrisane grupe sustava Office 365 u servisu Azure Active Directory](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted).

**Dozvola za stvaranje grupe**

Provjerite jeste li ovlašteni za stvaranje nove grupe. Globalni administratori mogu onemogućiti stvaranje grupe na portalu Azure ili na ploči programa Access. Da biste stvorili novu grupu za vas, možda će vam trebati administrator ili vam dati odgovarajuće dozvole.

1. [Stvaranje nove grupe i dodavanje članova na portal Azure](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-groups-create-azure-portal)
2. [Stvaranje grupa u komponenti PowerShell MSOnline](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-settings-v2-cmdlets#create-groups)
3. [Onemogućivanje stvaranja grupa u komponenti PowerShell](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-settings-v2-cmdlets#disable-group-creation-by-your-users) 
4. [Upravljanje osobama koje mogu stvarati grupe u sustavu Office 365](https://docs.microsoft.com/microsoft-365/solutions/manage-creation-of-groups) 
5. [Onemogućivanje obavijesti o dobrodošlici u Office 365 pomoću komponente PowerShell](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup)
6. [Administrativne uloge za Azure AD](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)

**Upravljanje dozvolama za stvaranje grupa**

1. Globalni administratori mogu upravljati dozvolama za stvaranje grupa za sigurnost ili grupe sustava Office 365 stvorene na portalu Azure ili na ploči programa Access, postavljanjem **korisnika može stvarati sigurnosne grupe na servisu Azure portali** ili **korisnici mogu stvarati grupe sustava Office 365 u postavkama Azure portala** u **svim grupama > općenito (postavke)**.
2. Možete i ograničiti Stvaranje grupe da biste odabrali grupu korisnika ako imate licenčnu licencu za Azure AD P1 Premium.

**Onemogućivanje obavijesti dobrodošlice za nove članove grupe sustava Office 365**

Obavijest dobrodošlice koja se šalje korisnicima koji se dodaju u grupe sustava Office 365 može se onemogućiti postavljanjem `UnifiedGroupWelcomeMessageEnabled` na **False** u komponenti PowerShell. Saznajte više o ovoj [postavci](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup).













