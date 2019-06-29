---
title: Rješavanje problema s lozinku sinkronizacije
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 165e0ff4b2136b727450946d2c47756ebee7d393
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/28/2019
ms.locfileid: "35353097"
---
# <a name="troubleshoot-password-synchronization"></a>Rješavanje problema s lozinku sinkronizacije

Otklanjanje poteškoća gdje nema lozinke su sinkronizirane s verzijom Azure AD povezivanje 1.1.614.0 ili noviji:
  
1. Otvorite novu sesiju Windows PowerShell na poslužitelju Azure AD povezivanje s mogućnost **Pokreni kao Administrator** .

2. Pokrenite **RemoteSigned skup pravilnik izvođenja** ili **Postavi pravilnik izvođenja neograničen**.

3. Pokretanje čarobnjaka za povezivanje Azure AD.

4. Idite na stranicu **Dodatne zadatke** , odaberite **Otklanjanje**i kliknite **Dalje**.

5. Na stranici otklanjanje poteškoća kliknite izbornik **pokretanje pokrenuti otklanjanje pogrešaka** u PowerShellu.

6. U glavnom izborniku odaberite **Otklanjanje sinkronizacije lozinku**.

7. U izborniku sub odaberite **lozinku sinkronizacije neće raditi uopće**.

**Razumjeli rezultate otklanjanje zadatka**
  
Otklanjanje poteškoća zadatak izvodi sljedeće čekove:
  
- Ovjerava za klijentske Azure AD omogućena značajka sinkronizacije lozinku.

- Ovjerava da poslužitelj Azure AD povezivanje nije u pripremne načinu.

- Za svaki postojeći lokalno Active Directory poveznik (koji odgovara postojećem šume servisa Active Directory):

- 
  - Provjerava je li omogućena značajka sinkronizacije lozinku.

  - Traži lozinku sinkronizacije pulsnom događaje u zapisnicima događaja aplikacija sustava Windows.

  - Za svaku domenu Active Directory pod Active Directory poveznik lokalno:

  - Ovjerava domena je dostupno s poslužitelja Azure AD povezivanje.

  - Ovjerava računi Active Directory Domain Services (AD DS) koje koriste Active Directory poveznik lokalno ima ispravan korisničko ime, lozinku i dozvole potrebne za sinkronizaciju lozinku.

Više pomoć sinkronizaciju lozinku za otklanjanje poteškoća potražite [Otklanjanje lozinku sinkronizacije s Azure AD povezivanje sinkronizaciju](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).
  