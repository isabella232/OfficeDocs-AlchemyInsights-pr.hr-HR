---
title: Pravila zadržavanja u centru za administraciju sustava Exchange ne radi
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 0ceb1737040f0304bfe8b611241ce1deef487652
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29462065"
---
 **Problem:** Novostvoreni ili pravila zadržavanja ažurirani u centru za administraciju sustava Exchange ne primjenjivanje na poštanske sandučiće ili stavke su premještene u poštanski sandučić arhive ili izbrisane. 
  
 **Korijenski uzrok:**
  
- Možda na **Upravljana pomoćnika za mape** nije obrađen korisnikov poštanski sandučić. Upravljani Pomoćnik za mape pokušava obraditi svakih poštanskog sandučića u organizaciji oblak temelji svakih sedam dana. Ako promijenite oznaku zadržavanja ili primijenite neko drugo pravilo zadržavanja poštanski sandučić, možete pričekati dok na upravljana mapa pomoći obrađuje poštanski sandučić ili pokrenite cmdlet Start ManagedFolderAssistant za pokretanje upravljanih Pomoćnik za mape za određenu obradu poštanski sandučić. Ovaj cmdlet pokrenut je korisna za testiranje ili postavke zadržavanja oznaka ili pravila zadržavanja za otklanjanje poteškoća. Za dodatne informacije posjetite [pokrenuti upravljanih Pomoćnik za mape](https://msdn.microsoft.com/en-us/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).
    
  - **Rješenja:** Pokrenite sljedeću naredbu za pokretanje upravljanih Pomoćnik za mape za određene poštanski sandučić: 
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- To može se pojaviti i ako je **omogućeno** u poštanskom sandučiću **RetentionHold** . Ako poštanski sandučić stavljen na RetentionHold, pravila zadržavanja na poštanski sandučić nije obrađena tijekom vremena. Za više informaton na RetentionHold postavku pogledajte: [Poštanski sandučić držite zadržavanja](https://docs.microsoft.com/en-us/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).
    
    Rješenje
    
  - Provjera stanja RetentionHold postavku na određenom poštanskom sandučiću u [PowerShellu EXO](https://docs.microsoft.com/en-us/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - Pokrenite sljedeću naredbu da biste **onemogućili** RetentionHold na određene poštanski sandučić: 
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - Sada, ponovno pokrenite mapi upravljani pomoćnika:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 **Napomena:** Ako poštanski sandučić je manja od 10 MB, upravljana Pomoćnik za mape neće automatski obraditi poštanski sandučić. 
  

