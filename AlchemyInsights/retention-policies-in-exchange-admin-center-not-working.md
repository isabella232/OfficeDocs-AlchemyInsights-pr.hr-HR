---
title: Pravila zadržavanja u centru za administratore sustava Exchange ne funkcioniraju
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: e2fb22f872be0eefc3b4b78b18cd09baffa66cda
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43742425"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Pravila zadržavanja u centru za administratore sustava Exchange

 **Broj izdanja:** Novostvorena ili ažurirana pravila zadržavanja u centru za administratore sustava Exchange ne primjenjuju se na poštanske sandučiće ili stavke ne premještaju se u poštanski sandučić arhive ili se ne brišu. 
  
 **Glavni uzroci:**
  
- To je možda zato što **pomoćnik za upravljane mape** nije obradio korisnički poštanski sandučić. Pomoćnik za upravljane mape pokušava obraditi svaki poštanski sandučić u vašoj organizaciji utemeljenoj na oblaku svakih sedam dana. Ako promijenite oznaku zadržavanja ili primijenite drugo pravilo zadržavanja na poštanski sandučić, možete pričekati dok pomoć upravljane mape ne obradi poštanski sandučić ili možete pokrenuti cmdlet Start-ManagedFolderAssistant da biste pokrenuli pomoćnika za upravljane mape da biste obradili određeni poštanski sandučić. Pokretanje ovog cmdleta korisno je za testiranje ili otklanjanje poteškoća s pravilima zadržavanja ili postavkama oznake zadržavanja. Dodatne informacije [potražite u odjeljku Pokrenite pomoćnika za upravljane mape](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).
    
  - **Rješenje:** Pokrenite sljedeću naredbu da biste pokrenuli pomoćnika za upravljane mape za određeni poštanski sandučić:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- To se može dogoditi i ako je na poštanskom sandučiću **omogućena** **čuvanje vremena zadržavanja.** Ako je poštanski sandučić smješten na čuvanje zadržavanja, pravila zadržavanja poštanskog sandučića neće se obraditi tijekom tog vremena. Za više informaton na postavku ZadržavanjeHold pogledajte: [Zadržavanje poštanskog sandučića Čekanje](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).
    
    **Rješenje:**
    
  - Provjerite status postavke ZadržavanjaDržite na određenom poštanskom sandučiću u [EXO powershell:](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - Pokrenite sljedeću naredbu da biste **onemogućili** zadržavanjeDržite na određenom poštanskom sandučiću:
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - Sada ponovno pokrenite Pomoćnik za upravljane mape:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 **Napomena:** Ako je poštanski sandučić manji od 10 MB, pomoćnik za upravljane mape neće automatski obraditi poštanski sandučić.
 
Dodatne informacije o pravilima zadržavanja u centru za administratore sustava Exchange potražite u članku Sljedeće:
- [Oznake zadržavanja i pravila zadržavanja](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [Primjena pravila zadržavanja na poštanske sandučiće](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [Dodavanje ili uklanjanje oznaka zadržavanja](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [Kako prepoznati vrstu čekanja postavljenog na poštanski sandučić](https://docs.microsoft.com/office365/securitycompliance/identify-a-hold-on-an-exchange-online-mailbox)
