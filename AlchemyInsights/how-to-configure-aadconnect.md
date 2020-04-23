---
title: 646 Kako konfigurirati AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "646"
- "1300023"
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 713cda26e55f07f0438cb9ebe5aa9da86c4ebb3a
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43722521"
---
# <a name="configure-sync-features"></a>Konfiguriranje značajki sinkronizacije

Azure AD Connect sadrži nekoliko značajki koje su prema zadanim postavkama omogućene ili koje možete omogućiti kasnije. Neke značajke zahtijevaju dodatnu konfiguraciju u određenim okruženjima.

- [Filtriranje](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) ograničava da se objekti sinkroniziraju sa Azure AD-om. Prema zadanim postavkama, svi korisnici, kontakti, grupe i računi računala sa sustavom Windows 10 sinkroniziraju se. Objekte možete uključiti ili izuzeti na temelju domena, OU-ova ili drugih atributa.

- [Sinkronizacija raspisija](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) lozinkom sinkronizira raspadjevi lozinke iz lokalnog servisa Active Directory u Azure AD. To omogućuje upravljanje lozinkom na jednom mjestu, ali korištenje iste lozinke u lokalnim i cloud okruženjima. Budući da je Active Directory autoritativni izvor, možete koristiti vlastita pravila za lozinku.

- [Samoposlužno ponovno postavljanje lozinke (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) korisnicima omogućuje ponovno postavljanje vlastitih lozinki u oblaku, a da još uvijek primjenjujete pravila lokalne lozinke.

- [Povrat podataka uređaja](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) omogućuje vraćanje registriranih uređaja u Azure AD u lokalni Active Directory da bi se mogli koristiti za uvjetni pristup.

- [Sprječavanje slučajnog brisanja](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) omogućeno je prema zadanim postavkama kako bi se spriječilo previše istovremenih brisanja objekata (više od 500 objekata po sinkronizaciji). Tu postavku možete promijeniti tako da odgovara potrebama vaše tvrtke ili ustanove.

- [Automatska nadogradnja](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) omogućena je prema zadanim postavkama za ekspresne instalacije i pomaže vam da vaša verzija usluge Azure AD Connect bude uvijek aktualna.
