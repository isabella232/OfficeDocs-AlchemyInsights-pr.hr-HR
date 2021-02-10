---
title: Sinkronizacija zaporke za servis domena
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8248"
- "9004400"
- "8249"
- "9003245"
ms.openlocfilehash: 7f138837b720926c5b687285a105eb0417ca5b39
ms.sourcegitcommit: 22eaf0a151ab95414476f596db8d318b6540ff31
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50177384"
---
# <a name="password-hash-synchronization-for-domain-service"></a>Sinkronizacija zaporke za servis domena

**Ako vam je instanca servisa Azure AD DS potakla da omogućite sinkronizaciju lozinki za lozinke**

Naiđete na scenarij u kojem se prikazuju hibridno okruženje s sinkronizacijom korisnika iz lokalnog okruženja Azure Active Directory domena Services (AD DS). Ovaj se scenarij susreće unatoč tome što ste sinkroniziranje lozinke iz lokalnog servisa AD DS uključili u zakupac Azure oglasa.

**Jer**

To se događa budući da se Azure AD Connect po zadanom ne sinkronizira s novim tehnologijama za upravljanje lancima (NTLM) i Kerberos lozinkama koje su potrebne za Azure AD DS.

**Workaround** 

Morate konfigurirati Azure AD Connect da biste sinkronizirali lozinke koje su potrebne za provjeru autentičnosti NTLM i Kerberos.

Kada je konfigurirana Azure AD Connect, lokalno stvaranje računa ili događaj promjene lozinke također sinkronizira nasljeđene lozinke za Azure AD. Dodatne informacije o tome potražite [u članku upute](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-password-hash-sync) za omogućivanje sinkronizacije lozinki u hibridnu okruženju Azure AD DS.