---
title: 646 kako konfigurirati AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "646"
- "1300023"
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 6327e42b74283d732247c9a847c68db72082c56a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47704481"
---
# <a name="configure-sync-features"></a>Konfiguriranje značajki sinkronizacije

Azure AD Connect sadrži nekoliko značajki koje su omogućene po zadanom ili koje možete omogućiti kasnije. Za neke je značajke potrebna dodatna konfiguracija u određenim okruženjima.

- [Filtriranje](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) ograničava objekte sinkroniziraju s Azure AD. Po zadanom se sinkroniziraju svi korisnici, kontakti, grupe i računi računala sa sustavom Windows 10. Objekte možete uvrstiti ili isključiti na temelju domena, tih ili drugih atributa.

- [Sinkronizacija zaporke za lozinke](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) sinkronizira dodatak za lozinke iz lokalnog servisa Active Directory na Azure AD. Time se omogućuje upravljanje lozinkama na jednom mjestu, no korištenje iste lozinke u lokalnim i okruženjima oblaka. Budući da je Active Directory Autoritativni izvor, možete koristiti vlastite pravilnike za lozinku.

- [Samoposlužno ponovno postavljanje lozinke (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) korisnicima omogućuje ponovno postavljanje vlastitih lozinki u oblaku dok se i dalje primjenjuje pravilnik o lozinci za lokalnu lozinku.

- [Nepotvrđenim uređaja](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) omogućuje pisanje registriranih uređaja u servisu Azure ad u lokalni aktivni direktorij da bi se mogli koristiti za uvjetni pristup.

- [Onemogućivanje slučajnog](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) brisanja po zadanom je omogućeno da bi se spriječilo previše brisanje istovremenih objekata (više od 500 objekata po sinkronizaciji). Tu postavku možete promijeniti tako da udovoljite potrebama tvrtke ili ustanove.

- [Automatska nadogradnja](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) omogućena je prema zadanim postavkama za ekspresne instalacije te omogućuje da vaša verzija servisa Azure ad Connect uvijek bude aktivna.
