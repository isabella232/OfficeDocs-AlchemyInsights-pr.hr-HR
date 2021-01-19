---
title: Problemi s prijavom u aplikacije
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7788"
- "9004355"
ms.openlocfilehash: 2d073367dc1c3e8e117c0b68e205297a65024872
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 01/18/2021
ms.locfileid: "49900803"
---
# <a name="issues-signing-in-to-applications"></a>Problemi s prijavom u aplikacije

Da biste otkrili uzrok ili dijagnosticirali poteškoće povezane s korisničkim prijavom, učinite sljedeće:

1. Pokrenite [dijagnostiku za prijavu](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).
2. Pronađite događaj za analizu unosom pojedinosti koje imate o korisniku, aplikaciji, vremenu prijave, ID-u zahtjeva ili ID-u korelacije.
3. Pregledajte rezultate dijagnostičkih prikaza s pojedinostima o tome što se dogodilo i koje akcije možete poduzeti da biste unijeli promjene, ako su potrebne promjene.

Slijede neki Česti problemi koje možete doživjeti prilikom prijave u aplikacije:

1. Vi ili korisnik **dovršili ste prijavu za Azure AD, ali će vam se prikazati neočekivani upit** u članku [neočekivani sporazum o pristanku prilikom prijave u aplikaciju](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-prompt) i [neočekivana pogreška prilikom izvođenja pristanka na aplikaciju](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).
2. Vi ili korisnik ste se **prijavili izravno u aplikaciju, ali se ne možete prijaviti na nju iz funkcije deeplink na prilagođenom portalu ili na ploči programa Access**: Pročitajte članak [Otklanjanje poteškoća s prijavom u aplikaciju iz servisa Azure ad moje aplikacije](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-other-problem-access-panel).
3. Vi ili korisnik **dovršili ste prijavu za Azure AD, no aplikacija prikazuje poruku o pogrešci i ne dopušta korisniku dovršetak tijeka prijave**: problem je u tome što aplikacija nije prihvaćala odgovor koji je Azure ad izdao. Da biste otklonili poteškoće, slijedite [ove korake](https://docs.microsoft.com/azure/active-directory/application-sign-in-problem-application-error) .
4. Vi ili korisnik **ne možete se prijaviti u aplikaciju koja nije galerija konfigurirana za jedinstvenu prijavu lozinke**: slijedite upute u [sljedećim koracima](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso) da biste otklonili poteškoće.
5. Vi ili korisnik **ne možete se prijaviti u aplikaciju za galeriju Azure ad koja je konfigurirana za jedinstvenu prijavu lozinke**: slijedite [ove korake](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso) da biste otklonili poteškoće.
6. Vi ili korisnik **ne možete se prijaviti u Microsoftovu aplikaciju**: slijedite [ove korake](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-first-party-microsoft) da biste otklonili poteškoće.
7. Vi ili korisnik **ne možete se prijaviti u aplikaciju koja nije galerija konfigurirana za udruženu jedinstvenu prijavu**: slijedite [ove korake](https://docs.microsoft.com/azure/active-directory/application-sign-in-problem-federated-sso-non-gallery) da biste otklonili poteškoće.
8. Vi ili korisnik **ne možete se prijaviti u aplikacijsku galeriju za Azure ad konfiguriranu za sjedinjenu jedinstvenu prijavu**: slijedite [ove korake](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery) da biste otklonili poteškoće.
9. Vi ili korisnik **ne možete se prijaviti u aplikaciju prilagođenu razvijenu** stavku: slijedite [ove korake](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery) da biste otklonili poteškoće.
10. Vi ili korisnik **ne možete se prijaviti u lokalnu aplikaciju pomoću proxy poslužitelja za Azure ad**: slijedite [ove korake](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-on-premises-application-proxy) da biste otklonili poteškoće.

