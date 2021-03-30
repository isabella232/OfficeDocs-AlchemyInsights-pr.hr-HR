---
title: Aplikacija za provjeru autentičnosti
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003252"
- "9909"
ms.openlocfilehash: 67331a9661ee67c4a861feb1a4292255a4d37133
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/29/2021
ms.locfileid: "51404365"
---
# <a name="authentication-app"></a>Aplikacija za provjeru autentičnosti

Ako ste globalni administrator, možete brzo saznati što se dogodilo ili dijagnosticirati probleme vezane uz prijavu korisnika pomoću dijagnostike [za prijavu.](https://ms.portal.azure.com/microsoft.onmicrosoft.com?loginHint=shhada@microsoft.com#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)

1. Pokrenite dijagnostiku klikom na gumb["Pokreni](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)dijagnostiku". 
1. Pronađite događaj koji želite analizirati tako da unesete pojedinosti o korisniku, aplikaciji, vremenu prijave, ID-u zahtjeva ili ID-u korelacije.
1. Pregledajte dijagnostičke rezultate koji prikazuju pojedinosti o tome što se dogodilo i koje akcije možete poduzeti da biste unijeli promjene, ako su potrebne neke promjene.

**Provjerite scenarij koji je primjenjiv:**

1. Ako korisnik ne prima push obavijest u aplikaciji Microsoft Authenticator, provjerite nisu li prikazani pod blokiranim korisnicima MFA-om, kao što je opisano u [članku Blokiraj i deblokiraj korisnike](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).
1. Ako korisnik nije blokiran za MFA, ali ne prima push obavijest, može otvoriti aplikaciju Microsoft Authenticator, koja će povući zahtjeve za odobrenje na čekanju.
1. Kao alternativni način prijave korisnik može i kliknuti Prijava na drugi način i odabrati korištenje koda za provjeru valjanosti iz mobilne aplikacije.
1. Aplikacija Microsoft Authenticator jedina je dostupna metoda za mnoge korisnike. [Dodatne informacije o sigurnosnim zadanim postavkama](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)potražite u najčešćim pitanjima o aplikaciji [Authenticator](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-faq) da biste saznali najčešća pitanja i kako ih riješiti.
 
**Preporučeni videozapisi**

[Postavljanje aplikacije Authenticator na novom telefonu (2min).](https://go.microsoft.com/fwlink/?linkid=2158163&clcid=0x409)
