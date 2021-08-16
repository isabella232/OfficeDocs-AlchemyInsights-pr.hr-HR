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
ms.openlocfilehash: f129da8731877aa00fd9b1dcf20905d353a4895303390ce7ff5642a8ff3ccbc2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53996622"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook se ne može povezati s javnim mapama

Ako pristup javnim mapama ne funkcionira za neke korisnike, pokušajte sljedeće:

Povezivanje exo PowerShell i konfigurirati parametar DefaultPublicFolderMailbox na korisničkom računu problema tako da odgovara parametru na radnom korisničkom računu.

Primjer:

Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox

Set-Mailbox Korisnik -DefaultPublicFolderMailbox \<value from previous command>

Pričekajte najmanje jedan sat da bi promjena snazi.

Ako problem i dalje postoji, slijedite [ovaj postupak da biste otklonili](https://aka.ms/pfcte) poteškoće s pristupom javnim mapama pomoću Outlook.
 
**Da biste upravljali korisnicima koji mogu pristupati javnim mapama pomoću Outlook:**

1.  Korištenje Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true ili $false  
      
    $true: korisnicima omogućite pristup javnim mapama u Outlook  
      
    $false: onemogućivanje korisničkog pristupa javnim mapama u Outlook. To je zadana vrijednost.  
        
2.  Set-OrganizationConfig -PublicFolderShowClientControl $true   
      
**Napomena** Ovaj postupak može kontrolirati veze samo s Outlook za Windows klijentima. Korisnik može nastaviti pristupati javnim mapama pomoću aplikacije OWA ili Outlook za Mac.
 
Dodatne informacije potražite u članku [Najava podrške za kontrolirane veze s javnim mapama u sustavu Outlook](https://aka.ms/controlpf).