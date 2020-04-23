---
title: Rješavanje problema sa sinkronizacijom lozinki
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: edd4f68466296f72c2dc0bafda45e6749d62d942
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43732502"
---
# <a name="troubleshoot-password-synchronization"></a>Rješavanje problema sa sinkronizacijom lozinki

Da biste otklonili poteškoće kada se lozinke ne sinkroniziraju sa servisom Azure AD Connect verzije 1.1.614.0 ili novije:
  
1. Otvorite novu sesiju komponente Windows PowerShell na poslužitelju Azure AD Connect pomoću mogućnosti **Pokreni kao administrator.**

2. Pokrenite **Set-ExecutionPolicy RemoteSigned** ili **Set-ExecutionPolicy neograničen**.

3. Pokrenite čarobnjak za Azure AD Connect.

4. Idite na stranicu **Dodatni zadaci,** odaberite **Otklanjanje poteškoća**i kliknite **Dalje**.

5. Na stranici Otklanjanje poteškoća kliknite **Pokreni da biste pokrenuli** izbornik za otklanjanje poteškoća u programu PowerShell.

6. U glavnom izborniku odaberite **Otklanjanje poteškoća sa sinkronizacijom lozinki**.

7. U podizborniku odaberite **Sinkronizacija lozinki uopće ne funkcionira**.

**Objašnjenje rezultata zadatka otklanjanja poteškoća**
  
Zadatak otklanjanja poteškoća izvodi sljedeće provjere:
  
- Provjerava je li značajka sinkronizacije lozinke omogućena za klijenta Azure AD-a.

- Provjerava je li poslužitelj Azure AD Connect u pripremnom načinu rada.

- Za svaki postojeći lokalni konektor servisa Active Directory (koji odgovara postojećoj šumi servisa Active Directory):

- 
  - Provjerava je li omogućena značajka sinkronizacije lozinke.

  - Traži događaje zapisnika zapisnika zapisnika sinkronizacije lozinkom u zapisnicima događaja aplikacije sustava Windows.

  - Za svaku domenu servisa Active Directory pod lokalnim povezom servisa Active Directory:

  - Provjerava je li domena dostupna s poslužitelja Azure AD Connect.

  - Provjerava ima li računi servisa Active Directory Domain Services (AD DS) koje koristi lokalni poveznik servisa Active Directory ispravno korisničko ime, lozinku i dozvole potrebne za sinkronizaciju lozinki.

Dodatne informacije o otklanjanju poteškoća pri sinkronizaciji lozinki [potražite u članku Otklanjanje poteškoća sa sinkronizacijom lozinke pomoću sinkronizacije usluge Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).
  