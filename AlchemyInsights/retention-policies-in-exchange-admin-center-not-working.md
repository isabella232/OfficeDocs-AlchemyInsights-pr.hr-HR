---
title: Pravila zadržavanja u centru za administratore sustava Exchange ne funkcioniraju
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
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 1fee2361b2dd6e0989d430a17aebb13bd5948578
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47740502"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Pravila zadržavanja u centru za administratore sustava Exchange

Ako želite da pokrenete automatske provjere za navedene postavke, odaberite gumb natrag < – pri vrhu ove stranice, a zatim unesite adresu e-pošte korisnika koji ima problema s pravilima zadržavanja.

 **Problem:** Novo stvorene ili ažurirane pravilnika o zadržavanju u centru za administratore sustava Exchange ne primjenjuju se na poštanske sandučiće ili se stavke ne premještaju u arhivski poštanski sandučić ili izbrisane. 
  
 **Korijenski uzroci:**
  
- To je možda zato što **Pomoćnik za upravljane mape** nije procesira korisnikov poštanski sandučić. Pomoćnik za upravljane mape pokušava obraditi svaki poštanski sandučić u tvrtki ili ustanovi utemeljenoj na oblaku jednom svakih sedam dana. Ako promijenite oznaku zadržavanja ili primijenite drugo pravilo zadržavanja na poštanski sandučić, možete pričekati dok upravna mapa ne obradi poštanski sandučić, a možete i pokrenuti cmdlet Start-ManagedFolderAssistant da biste pokrenuli pomoćnik za upravljane mape da bi obradio određeni poštanski sandučić. Pokretanjem tog cmdleta korisna je provjera i otklanjanje poteškoća s pravilima zadržavanja ili oznakama zadržavanja. Dodatne informacije potražite u odjeljku [pokretanje pomoćnika za upravljanu mapu](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).
    
  - **Rješenje:** Pokrenite sljedeću naredbu da biste pokrenuli pomoćnik za upravljane mape za određeni poštanski sandučić:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- To se može dogoditi i ako je na poštanskom sandučiću **omogućena** mogućnost **Retentionhold** . Ako je poštanski sandučić stavljen na nastavak, pravilnik o zadržavanju na poštanskom sandučiću neće biti obrađen tijekom tog vremena. Dodatne informacije o postavljanju programa RetentionHold potražite u članku [zadržavanje poštanskog sandučića na čekanju](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).
    
    **Rješenje**
    
  - Provjerite status postavke RetentionHold na određenom poštanskom sandučiću u programu [Exo PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - Pokrenite sljedeću naredbu da biste **onemogućili** retentionhold na određenom poštanskom sandučiću:
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - Zatim ponovno pokrenite pomoćnik za upravljane mape:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 **Upozorenje:** Ako je poštanski sandučić manji od 10 MB, pomoćnik za upravljanu mapu neće automatski obraditi poštanski sandučić.
 
Dodatne informacije o pravilima zadržavanja u centru za administratore sustava Exchange potražite u članku:
- [Oznake zadržavanja i pravila zadržavanja](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [Primjena pravilnika o zadržavanju na poštanske sandučiće](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [Dodavanje i uklanjanje oznaka zadržavanja](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [Prepoznavanje vrste držite smještenih na poštanskom sandučiću](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
