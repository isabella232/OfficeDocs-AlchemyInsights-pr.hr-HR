---
title: Nije moguće pristupiti javnim mapama
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: d63a193585cb73c2ce8e160d413db4e837100d33
ms.sourcegitcommit: d3ace2376195d54229ee1e232daf8133ba4e58a9
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/03/2020
ms.locfileid: "47341395"
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