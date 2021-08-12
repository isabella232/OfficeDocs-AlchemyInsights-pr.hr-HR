---
title: 646 Konfiguriranje servisa AADConnect
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
ms.openlocfilehash: c5fa5fd7586f999698fe43554fb9a2b205be3e25740c20763254a38d41297e0c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53963635"
---
# <a name="configure-sync-features"></a>Konfiguriranje značajki sinkronizacije

Azure AD Povezivanje sadrži nekoliko značajki koje su po zadanom omogućene ili koje kasnije možete omogućiti. Neke značajke zahtijevaju dodatnu konfiguraciju u određenim okruženjima.

- [Filtriranje ograničava](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) sinkronizaciju objekata sa servisom Azure AD. Po zadanom se sinkroniziraju svi korisnici, kontakti, grupe i Windows 10 računa računala. Objekte možete uvrstiti ili izuzeti na temelju domena, OU-ova ili drugih atributa.

- [Sinkronizacija hasha](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) lozinkom sinkronizira hash lozinke s lokalnog servisa Active Directory sa servisom Azure AD. To omogućuje upravljanje lozinkom na jednom mjestu, ali korištenje iste lozinke u lokalnim okruženjima i u oblaku. Budući da je Active Directory mjerodavni izvor, možete koristiti vlastite pravilnike za lozinke.

- [Samoposlužno ponovno postavljanje lozinke (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) korisnicima omogućuje ponovno postavljanje vlastitih lozinki u oblaku uz primjenu lokalnog pravilnika o lozinkama.

- [Vraćanje pisanja na](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) uređaj registriranim uređajima na servisu Azure AD omogućuje da se pišu natrag u lokalni Active Directory da bi se mogli koristiti za uvjetni pristup.

- [Sprječavanje slučajnih brisanja](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) po zadanom je omogućeno da bi se spriječilo previše istodobnih brisanja objekata (više od 500 objekata po sinkronizaciji). Tu postavku možete promijeniti tako da zadovoljava potrebe tvrtke ili ustanove.

- [Automatska nadogradnja](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) po zadanom je omogućena za ekspresne instalacije i pridonosi osiguravanju da je verzija servisa Azure AD Povezivanje uvijek aktualna.
