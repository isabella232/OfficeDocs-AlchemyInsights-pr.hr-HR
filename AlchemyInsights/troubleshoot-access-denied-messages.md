---
title: Rješavanje problema s porukama pristup odbijen
ms.author: kaarins
author: kaarins
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 3973f5bf584343d3353e7389f22bc727827b5c35
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29461283"
---
# <a name="troubleshoot-access-denied-messages"></a>Rješavanje problema s porukama pristup odbijen

Ako netko dobio poruku "Pristup je odbijen" zajedničke mape, administrator zbirke web-mjesta možda imaju omogućen "ograničeni pristup korisnika dozvolu lockdown način." Da biste to isključili: 
  
1. Otiđite na web-mjesto, kliknite ikonu postavke i kliknite **Postavke web-mjesta**.
    
2. U sekciji **Administracija zbirke web-mjesta**pritisnite **značajke zbirke web-mjesta**.
    
3. Uz **način rada lockdown dozvole Ograničeni pristup korisnika**, kliknite **Deaktiviraj**.
    
Pristup odbijen poruke mogu se pojaviti za zajedničke mape ako web-mjesto je web-mjesto za objavljivanje. Info, potražite [Pristup odbijen prilikom pristupanja zajedničkoj mapi](https://go.microsoft.com/fwlink/?linkid=2004317).
  
Ako je netko dobio poruku "Pristup je odbijen" prilikom pokušaja prikaz zahtjeve za pristup, korisnik treba dodati kao administrator zbirke web-mjesta ili član grupe vlasnika web-mjesta. Za dodatne informacije pogledajte [Odbijen pristup zahtjeve za pristup popisu](https://go.microsoft.com/fwlink/?linkid=2004220).
  
Ako korisnik dobio poruku "Pristup je odbijen" nakon što su uklonjene iz servisa Active Directory lokalno i dodali natrag, pogledajte [Pristup odbijen kada korisnički račun je sinkronizirana Office 365](https://go.microsoft.com/fwlink/?linkid=2004318).
  

