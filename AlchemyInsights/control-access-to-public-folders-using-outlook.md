---
title: Upravljanje pristupom javnim mapama pomoću Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: 1386b97f804e63455094abf64b9d9e2541d57dafa36535813b0d7689e0ce2966
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54032550"
---
# <a name="control-access-to-public-folders-using-outlook"></a>Upravljanje pristupom javnim mapama pomoću Outlook

Da biste upravljali korisnicima koji mogu pristupati javnim mapama pomoću Outlook:

1. Korištenje `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`

$true: korisnicima omogućite pristup javnim mapama u Outlook  
$false: onemogućivanje korisničkog pristupa javnim mapama u Outlook. To je zadana vrijednost.  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

Napomena: ovim postupkom možete upravljati samo vezama s Outlook za Windows klijentima. Korisnici mogu nastaviti pristupati javnim mapama pomoću aplikacije OWA ili Outlook za Mac.

Dodatne informacije potražite u članku [Kontrolirane veze s javnim mapama Outlook dodatne](https://aka.ms/controlpf) informacije.
