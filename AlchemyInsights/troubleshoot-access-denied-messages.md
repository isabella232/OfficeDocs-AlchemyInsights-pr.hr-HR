---
title: Otklanjanje poteškoća s zabranom pristupa porukama
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 6c8ad84123fb58b73b9c378592ce970997893ea2
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704886"
---
# <a name="troubleshoot-access-denied-messages"></a>Otklanjanje poteškoća s zabranom pristupa porukama

Ako je netko dobio poruku "pristup je odbijen" u zajedničku mapu u sustavu SharePoint, administrator zbirke web-mjesta mogao je omogućiti "ograničen pristup korisniku dozvola za zaključavanje." Da biste isključili ovu stavku, učinite sljedeće: 
  
1. Dođite do web-mjesta, kliknite ikonu Postavke, a zatim **Postavke web-mjesta**.
    
2. U odjeljku **Administracija zbirke web-mjesta** kliknite **značajke zbirke web-mjesta**.
    
3. Pokraj funkcije **zaključavanje korisničkih dozvola za ograničen pristup** kliknite **Deaktiviraj**.
    
Ako je web-mjesto web-mjesto za objavljivanje, može se pojaviti i poruka o uskraćenog pristupa. Informacije potražite u članku [zabranjen pristup prilikom pristupanja zajedničkoj mapi](https://answers.microsoft.com/windows/forum/windows_7-files/access-denied-to-share-folder/79fae49d-cddf-4845-8ac8-c141884d85fb).
  
Ako je netko dobio poruku "pristup je odbijen" prilikom pokušaja pregledavanja zahtjeva za pristup, korisnik mora biti dodan kao administrator zbirke web-mjesta ili član grupe vlasnici za web-mjesto. Dodatne informacije potražite u članku [zabranjen pristup popisu zahtjeva za pristup](https://go.microsoft.com/fwlink/?linkid=2004220).
  
Ako je korisnik dobio poruku "pristup je odbijen" nakon uklanjanja iz lokalnih servisa Active Directory, a zatim dodan natrag, pročitajte članak [zabranjen je kada se korisnički račun sinkronizira sa sustavom Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).
  

