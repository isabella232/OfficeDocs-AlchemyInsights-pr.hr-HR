---
title: Problemi s uvjetnim pristupom
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004349"
- "7768"
ms.openlocfilehash: 85cbd89e461f36a51eed816619fd132ea60dfdb0014eb850c7ec3f38d41e1ca2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54069956"
---
# <a name="conditional-access-issues"></a>Problemi s uvjetnim pristupom

**Rješavanje problema s dijagnostikom za prijavu**

Pomoću dijagnostike za prijavu možete brzo saznati što se dogodilo ili dijagnosticirati probleme vezane [uz prijavu korisnika:](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)

1. Pokrenite dijagnostiku za prijavu.
1. Pronađite događaj koji želite analizirati tako da unesete pojedinosti o korisniku, aplikaciji, vremenu prijave, ID-u zahtjeva ili ID-u korelacije.
1. Pregledajte dijagnostičke rezultate koji prikazuju pojedinosti o tome što se dogodilo i koje radnje možete poduzeti da biste unijeli promjene (ako su potrebne neke promjene).

**Koraci za otklanjanje poteškoća s prijavom** 

1. Otvorite stranicu za prijavu na Azure AD.
1. Filtrirajte prijave po korisniku, vremenskom rasponu, aplikaciji, statusu, klijentskom aplikacijom i tako dalje.
1. Odaberite događaj prijave i prikažite karticu Uvjetni pristup da biste vidjeli koji su pravilniki procijenjeni.
1. Kliknite redak pravilnika da biste pogledali pojedinosti pravilnika i razumjeli zašto je primijenjen.

**Alati za otklanjanje poteškoća s pravilnikom uvjetnog pristupa**

- Način rada samo za izvješća omogućuje vam procjenu pravilnika bez utjecaja na korisnike.
- Alat "što ako" omogućuje simuliranje događaja prijave i pregled primjenjivih pravilnika.
- Uvidi i izvješćivanje radne knjige prikazuje učinak svakog pravilnika u stvarnom vremenu.

**Pravila zaštite od osnovne vrijednosti**

Pravila zaštite od osnovne vrijednosti zastarjela su. Više se ne primjenjuju i uskoro će se ukloniti s portala Azure. Preporučujemo omogućivanje [zadanih sigurnosnih postavki](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).

Dodatne informacije o uvjetnom pristupu potražite u članku:

[Najbolje prakse za uvjetni pristup u Azure Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Uvjeti u uvjetnom pristupu](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Kontrole u uvjetnom pristupu](https://docs.microsoft.com/azure/active-directory/conditional-access/controls)  
 [Mjesta u uvjetnom pristupu](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)
