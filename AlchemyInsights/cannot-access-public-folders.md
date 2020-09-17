---
title: Nije moguće pristupiti javnim mapama
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: 272918b38f6019cb2bdcaa4013baebaa5f04fe85
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47812539"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook se ne može povezati s javnim mapama

Ako pristup javnoj mapi ne funkcionira za neke korisnike, pokušajte sljedeće:

Povežite se s programom EXO PowerShell i konfigurirajte parametar Defaultpublifoldermailbox na korisničkom računu problema da bi odgovarao parametru na radnom korisničkom računu.

Primjer

Nabavite-Mailbox WorkingUser | ft Defaultpublifoldermailbox, Effectivepublifoldermailbox

Problem s postavkom poštanskog sandučića – Defaultpublifoldermailbox \<value from previous command>

Pričekajte najmanje jedan sat da bi promjena stupila na kraj.

Ako problem ostaje, slijedite [ovaj postupak](https://aka.ms/pfcte) da biste otklonili poteškoće s pristupom javnim mapama pomoću programa Outlook.
 
**Da biste kontrolirali koji korisnici mogu pristupati javnim mapama pomoću programa Outlook**:

1.  Korištenje servisa set-CASMailbox <mailboxname> -publifolderclientaccess $TRUE ili $FALSE  
      
    $true: korisnicima dopusti pristup javnim mapama u programu Outlook  
      
    $false: Onemogućivanje korisničkog pristupa javnim mapama u programu Outlook. To je zadana vrijednost.  
        
2.  Set-OrganizationConfig-PublicFolderShowClientControl $true   
      
**Notes** Ovaj postupak može upravljati vezama samo s klijentskim računalima programa Outlook za Windows. Korisnik može nastaviti pristupati javnim mapama pomoću značajke OWA ili programa Outlook za Mac.
 
Dodatne informacije potražite u članku [Objavljivanje podrške za kontrolirane veze s javnim mapama u programu Outlook](https://aka.ms/controlpf).