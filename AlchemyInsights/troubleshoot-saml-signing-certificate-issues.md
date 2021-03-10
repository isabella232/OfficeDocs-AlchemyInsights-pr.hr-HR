---
title: Otklanjanje poteškoća sa potpisom SAML certifikata
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9406"
- "9004341"
ms.openlocfilehash: 3bc8b2e751395b8a099fb5079ad40c5c93222e0e
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/08/2021
ms.locfileid: "50692652"
---
# <a name="troubleshoot-saml-signing-certificate-issues"></a>Otklanjanje poteškoća sa potpisom SAML certifikata

Da biste riješili problem sa potpisom SAML certifikata, izvedite sljedeće preporučene korake:

1. Kada dodate korporacijsku aplikaciju koja podržava SSO, Azure će generirati certifikat koji se naziva [certifikatom saml za potpisivanje](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#auto-generated-certificate-for-gallery-and-non-gallery-applications). Ovaj certifikat ima Datum isteka od 3 godine. Da biste promijenili datum isteka certifikata, pročitajte članak [Prilagodba datuma isteka za certifikat Federacije i njegovo pretvaranje u novi certifikat](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#customize-the-expiration-date-for-your-federation-certificate-and-roll-it-over-to-a-new-certificate).
2. Azure će ovaj certifikat koristiti za potpisivanje tokena za SAML koje zatraži aplikacija i poslat će ga u aplikaciju za uspješan SSO. Da biste to dovršili, Preuzmite certifikat s portala Azure i poљaljite ga dobavljaču aplikacije da biste dovršili postupak SSO.

Nakon završetka postupka, aplikacija će potvrditi taj certifikat i sve tokene za SAML koje je potpisao taj certifikat.

3. Ako ovaj certifikat istekne, stvorite novi certifikat, ažurirajte ga proizvođaču aplikacija, a zatim ga učinite aktivnim na stranici Azure. Dodatne informacije potražite u članku [obnavljanje certifikata koji će uskoro isteći](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#renew-a-certificate-that-will-soon-expire).

> [!NOTE]
> Ako certifikat istekne, korisnik neće biti blokiran.

4. [Dodajte adresu e-pošte](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#add-email-notification-addresses-for-certificate-expiration) da bi se obavijesti primljene prije isteka tekućeg certifikata.

> [!NOTE]
> Korak-4 je neobavezan jedan.

5. Promjena mogućnosti potpisivanja certifikata za SAML i algoritam potpisivanja certifikata. Dodatne informacije potražite u članku [Promjena mogućnosti potpisivanja certifikata i algoritma potpisivanja](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).

