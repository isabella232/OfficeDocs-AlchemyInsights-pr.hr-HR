---
title: Nije moguće pristupiti javnim mapama
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: af5bd57512ee917d6e22d3838d55a2a1d62750d4
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819504"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook se ne može povezati s javnim mapama

Ako pristup javnim mapama ne funkcionira za neke korisnike, pokušajte sljedeće:

Povežite se s ljuskom EXO PowerShell i konfigurirajte parametar DefaultPublicFolderMailbox na korisničkom računu problema tako da odgovara parametru na radnom korisničkom računu.

Primjer:

Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox

Set-Mailbox Korisnik -DefaultPublicFolderMailbox \<value from previous command>

Pričekajte najmanje jedan sat da bi promjena snazi.

Ako problem i dalje postoji, slijedite ovaj [postupak da biste otklonili](https://aka.ms/pfcte) poteškoće s pristupom javnim mapama pomoću programa Outlook.
 
**Da biste upravljali korisnicima koji mogu pristupati javnim mapama pomoću programa Outlook:**

1.  Korištenje Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true ili $false  
      
    $true: omogući korisnicima pristup javnim mapama u programu Outlook  
      
    $false: onemogućivanje korisničkog pristupa javnim mapama u programu Outlook. To je zadana vrijednost.  
        
2.  Set-OrganizationConfig -PublicFolderShowClientControl $true   
      
**Napomena** Taj postupak može upravljati vezama samo s klijentima programa Outlook za računala za Windows. Korisnik može nastaviti pristupati javnim mapama pomoću aplikacije OWA ili Outlook za Mac.
 
Dodatne informacije potražite u članku [Najava podrške za kontrolirane veze s javnim mapama u programu Outlook](https://aka.ms/controlpf).