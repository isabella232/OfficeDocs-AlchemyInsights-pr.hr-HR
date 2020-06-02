---
title: Pravila zadržavanja u sustavu Exchange Admin Center ne funkcioniraju
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
ms.openlocfilehash: 3040365b9d686bcbcce60977ee9bdbbaffc70b24
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44502599"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Pravila zadržavanja u centru za administratore sustava Exchange

 **Problem:** Novostvorena ili ažurirana pravila zadržavanja u centru za administratore sustava Exchange ne primjenjuju se na poštanske sandučiće ili se stavke ne premještaju u poštanski sandučić arhive ili brišu. 
  
 **Uzroci korijena:**
  
- To je možda zato što pomoćnik za **upravljane mape** nije obradio korisnikov poštanski sandučić. Pomoćnik za upravljane mape pokušava obraditi svaki poštanski sandučić u vašoj organizaciji utemeljenoj na oblaku svakih sedam dana. Ako promijenite oznaku zadržavanja ili primijenite drugo pravilo zadržavanja na poštanski sandučić, možete pričekati dok pomoć u upravljanim mapama ne obradi poštanski sandučić ili možete pokrenuti cmdlet Start-ManagedFolderAssistant da biste pokrenuli pomoćnika za upravljane mape za obradu određenog poštanskog sandučića. Pokretanje ovog cmdleta korisno je za testiranje ili otklanjanje poteškoća s pravilima zadržavanja ili postavkama oznake zadržavanja. Dodatne informacije [potražite u odjeljku Pokretanje pomoćnika za upravljane mape](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).
    
  - **Rješenje:** Pokrenite sljedeću naredbu da biste pokrenuli pomoćnik za upravljane mape za određeni poštanski sandučić:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- To se može dogoditi i ako je u poštanskom sandučiću **omogućena** **zadržavanja.** Ako je poštanski sandučić postavljen na zadržavanje, pravila zadržavanja na poštanskom sandučiću neće se obraditi tijekom tog vremena. Dodatne informacije o postavkama Zadržavanje potražite u odjeljku: [Zadržavanje poštanskog sandučića](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).
    
    **Rješenje:**
    
  - Provjerite status postavke Zadržavanje na određenom poštanskom sandučiću u [EXO powershellu:](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - Pokrenite sljedeću naredbu da biste **onemogućili** zadržavanje na određenom poštanskom sandučiću:
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - Zatim, re- trčanje Uprava savijač Pomoćnik:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 **Napomena:** Ako je poštanski sandučić manji od 10 MB, pomoćnik za upravljane mape neće automatski obraditi poštanski sandučić.
 
Dodatne informacije o pravilima zadržavanja u centru za administratore sustava Exchange potražite u članku:
- [Oznake zadržavanja i pravila zadržavanja](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [Primjena pravila zadržavanja na poštanske sandučiće](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [Dodavanje ili uklanjanje oznaka zadržavanja](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [Kako prepoznati vrstu čekanja postavljenu na poštanski sandučić](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
