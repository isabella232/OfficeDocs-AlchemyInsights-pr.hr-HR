---
title: Problem s atributom atribut i skoping
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8470"
- "9004687"
ms.openlocfilehash: 78df24c0d8a670d678e26879cf81476f1ae9b92d
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50480969"
---
# <a name="problem-with-attribute-and-scoping-filter"></a>Problem s atributom atribut i skoping

**Problem s suprotnih vrijednosti UPN-a**

WORKDAY za oglase za dodjelu korisničkih radnih dana u servisu AD za korisnike prikazuje poruku o pogrešci **Hybridsinkronizationactivedirectoryuserprincipalnamenotunique**. Operacija nije uspjela jer vrijednost UPN koja je navedena za dodavanje/izmjena nije jedinstvena u širokom nivou šuma. Pojedinosti o pogrešci: **CONSTRAINT_ATT_TYPE-userPrincipalName**.

Vrijednost **UserPrincipalName** koja WORKDAY konektor pokušava postaviti prilikom stvaranja korisničkog računa za oglas već postoji u ciljnoj domeni oglasa. To implicira da bilo (1) korisnik već postoji, a provjera podudaranja ID-a nije uspjela za korisnika ili (2) pravilo stvaranja različite vrijednosti.

Evo predloženih koraka sanacije:

Ako korisnik već postoji, a provjera podudaranja ID-a nije uspjela povezati račun WORKDAY s računom servisa Active Directory, provjerite je li atribut podudaranja ID-a (obično **IDZaposlenika**) u radnom danu i oglasu točno podudaran. Ako nemaju podudaranje, to je problem s podacima koji je potreban za popravak. Ako je, primjerice, IDZaposlenika u radnim danom 001052, a u aplikaciji AD to je 1052, motor za dodjelu resursa neće uspjeti spojiti dva računa i pokušat će stvoriti korisnika koji već postoji. Rješenje u ovom slučaju jest promjena vrijednosti **zaposlenika** u aplikaciji ad da biste uključili početne nule da bi bilo 001052.
Ako izraz UPN-generiranje ne generira jedinstvenu vrijednost, razmotrite korištenje funkcije de-dupliciranje **Selectuniquevalue** da bi se svaki put generirao jedinstvena vrijednost.

**Radni dan za dodjelu resursa korisniku oglasa ne postavlja vrijednost atributa upravitelja za korisnički račun za oglas**

Radni dan za dodjelu resursa korisniku oglasa ne postavlja vrijednost atributa **upravitelja** za KORISNIČKE račune oglasa. Postoje dva moguća scenarija kada se to ponašanje vidi:

1. Upravitelj u radnim danom ne može se razriješiti na odgovarajući korisnički račun za oglas jer upravitelj nije u opsegu.
2. U scenariju **višestrukih domena oglasa** upravitelj u radnom danu nije prisutan u istoj domeni kao i korisnik.

Da biste riješili problem, isprobajte sljedeće korake:

1. Ako ste definirali filtre za filtriranje, najprije provjerite je li upravitelj u opsegu i zadovoljava li uvjet skoping. Ako upravitelj ne zadovolji filtar, promijenite filtar tako da je i upravitelj u opsegu postupka dodjele resursa.
2. Ako imate više domena oglasa, poveznik sadrži poznato ograničenje nemogućnosti rješavanja referenci upravitelja unakrsnih domena.

Dodatne informacije o konfiguriranju radnog dana za automatiziranu dodjelu resursa potražite u članku [Udžbenik: Konfiguriranje radnog dana za automatsku dodjelu korisnika](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).













