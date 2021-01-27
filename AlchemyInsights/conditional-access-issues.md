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
ms.openlocfilehash: 7c20b26e3a038dc4392684ca410eba97cec2df30
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 01/27/2021
ms.locfileid: "50014747"
---
# <a name="conditional-access-issues"></a>Problemi s uvjetnim pristupom

**Rješavanje problema s Dijagnosticiom za prijavu**

Možete brzo saznati što se dogodilo ili dijagnosticirati poteškoće povezane s korisničkim prijavom pomoću [dijagnostike za prijavu](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom):

1. Pokrenite dijagnostiku za prijavu.
1. Pronađite događaj za analizu unosom u detalje koje imate o korisniku, aplikaciji, vremenu prijave, ID-u zahtjeva ili ID-u korelacije.
1. Pregledajte rezultate dijagnostičkih prikaza s pojedinostima o tome što se dogodilo i koje akcije možete poduzeti da biste unijeli promjene (ako su potrebne promjene).

**Koraci za otklanjanje poteškoća s prijavom** 

1. Idite na stranicu za prijavu na Azure AD.
1. Filtriranje prijava prema korisniku, vremenskom rasponu, aplikaciji, statusu, klijentskoj aplikaciji i tako dalje.
1. Odaberite događaj prijave i prikažite karticu uvjetni pristup da biste vidjeli koja su pravila vrednovana.
1. Kliknite redak pravilnika da biste pogledali detalje o politici i razumjeli zašto se primjenjuje.

**Alati za otklanjanje poteškoća s Pravilnikom o uvjetnom pristupu**

- Način rada samo za izvješća omogućuje procjenu pravilnika bez ometanja korisnika.
- Alat što-ako vam omogućuje simulaciju događaja prijave i pogledajte koja se pravila primjenjuju.
- Radna knjiga uvida i izvješćivanja prikazuje utjecaj svakog pravilnika u stvarnom vremenu.

**Osnovna pravila zaštite**

Osnovna pravila zaštite su deprecated. Oni se više ne provode i uskoro će biti uklonjeni iz portala Azure. Preporučujemo omogućavanje [sigurnosnih zadanih postavki](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).

Dodatne informacije o uvjetnom pristupu potražite u članku:

[Najbolje prakse za uvjetni pristup u servisu Azure Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Uvjeti u uvjetnom pristupu](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Kontrole u uvjetnom pristupu](https://docs.microsoft.com/azure/active-directory/conditional-access/controls)  
 [Mjesta u uvjetnom pristupu](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)
