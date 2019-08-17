---
title: Pravila zadržavanja u centru za administraciju sustava Exchange ne radi
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: d0af4c933f262fe1ec4c2a6ff16d5f6195398b0d
ms.sourcegitcommit: e98443a049108e0dc83d63895af66944bdb1f108
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/16/2019
ms.locfileid: "36444800"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Pravila zadržavanja u centru za administraciju sustava Exchange

 **Problem:** Novostvoreni ili pravila zadržavanja ažurirani u centru za administraciju sustava Exchange ne primjenjivanje na poštanske sandučiće ili stavke su premještene u poštanski sandučić arhive ili izbrisane. 
  
 **Korijenski uzrok:**
  
- Možda na **Upravljana pomoćnika za mape** nije obrađen korisnikov poštanski sandučić. Upravljani Pomoćnik za mape pokušava obraditi svakih poštanskog sandučića u organizaciji oblak temelji svakih sedam dana. Ako promijenite oznaku zadržavanja ili primijenite neko drugo pravilo zadržavanja poštanski sandučić, možete pričekati dok na upravljana mapa pomoći obrađuje poštanski sandučić ili pokrenite cmdlet Start ManagedFolderAssistant za pokretanje upravljanih Pomoćnik za mape za određenu obradu poštanski sandučić. Ovaj cmdlet pokrenut je korisna za testiranje ili postavke zadržavanja oznaka ili pravila zadržavanja za otklanjanje poteškoća. Za dodatne informacije posjetite [pokrenuti upravljanih Pomoćnik za mape](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).
    
  - **Rješenja:** Pokrenite sljedeću naredbu za pokretanje upravljanih Pomoćnik za mape za određene poštanski sandučić:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- To može se pojaviti i ako je **omogućeno** u poštanskom sandučiću **RetentionHold** . Ako poštanski sandučić stavljen na RetentionHold, pravila zadržavanja na poštanski sandučić nije obrađena tijekom vremena. Za više informaton na RetentionHold postavku pogledajte: [Poštanski sandučić držite zadržavanja](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).
    
    **Rješenje:**
    
  - Provjera stanja RetentionHold postavku na određenom poštanskom sandučiću u [PowerShellu EXO](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):
    
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
 
Dodatne informacije o pravilima zadržavanja u centru za administraciju Exchange potražite:
- [Oznake zadržavanja i pravila zadržavanja](https://docs.microsoft.com/en-us/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [Primijeni pravila zadržavanja poštanski sandučići](https://docs.microsoft.com/en-us/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [Dodavanje ili uklanjanje oznake zadržavanja](https://docs.microsoft.com/en-us/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [Kako prepoznati vrstu čekanje smjestiti na poštanski sandučić](https://docs.microsoft.com/en-us/office365/securitycompliance/identify-a-hold-on-an-exchange-online-mailbox)
