---
title: Otklanjanje poteškoća s porukama koje su odbijene u programu Access
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: c62186fd346efd539b13cef9c80f5e797ebf80811a21db73f0f07fd86c080d55
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53939875"
---
# <a name="troubleshoot-access-denied-messages"></a>Otklanjanje poteškoća s porukama koje su odbijene u programu Access

Ako je netko dobio poruku "Pristup je odbijen" u zajedničku mapu u programu SharePoint, administrator zbirke web-mjesta možda je omogućio "Način zaključavanja korisničkih dozvola s ograničenim pristupom". Da biste to isključili: 
  
1. Pronađite web-mjesto, kliknite ikonu Postavke, a zatim Kliknite **Web-Postavke**.
    
2. U **odjeljku Administracija zbirke web-mjesta** kliknite **Značajke zbirke web-mjesta**.
    
3. Pokraj mogućnosti **Način zaključavanja korisničkih dozvola s ograničenim pristupom** kliknite **Deaktiviraj**.
    
Poruka o odbijenom pristupu može se pojaviti i za zajedničke mape ako je web-mjesto za objavljivanje. Informacije potražite u članku [Pristup je odbijen prilikom pristupa zajedničkoj mapi](https://answers.microsoft.com/windows/forum/windows_7-files/access-denied-to-share-folder/79fae49d-cddf-4845-8ac8-c141884d85fb).
  
Ako je netko dobio poruku "Pristup je odbijen" prilikom pokušaja prikaza zahtjeva za pristup, korisnika je potrebno dodati kao administrator zbirke web-mjesta ili kao član grupe Vlasnika za web-mjesto. Dodatne informacije potražite u članku [Popis zahtjeva za pristup odbijen pristupu](https://go.microsoft.com/fwlink/?linkid=2004220).
  
Ako je korisnik dobio poruku "Access Denied" (Pristup je odbijen) nakon što je uklonjen iz lokalnog servisa Active Directory, a zatim je ponovno dodao, pogledajte access denied when [a user account is synced to Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).
  

