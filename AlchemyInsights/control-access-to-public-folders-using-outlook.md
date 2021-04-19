---
title: Upravljanje pristupom javnim mapama pomoću programa Outlook
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
ms.openlocfilehash: f528044ca7f6f2ee2812f9f831093c44eca26fe1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816732"
---
# <a name="control-access-to-public-folders-using-outlook"></a>Upravljanje pristupom javnim mapama pomoću programa Outlook

Da biste upravljali korisnicima koji mogu pristupati javnim mapama pomoću programa Outlook:

1. Korištenje `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`

$true: omogući korisnicima pristup javnim mapama u programu Outlook  
$false: onemogućivanje korisničkog pristupa javnim mapama u programu Outlook. To je zadana vrijednost.  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

Napomena: ovim postupkom možete upravljati samo vezama s klijentima programa Outlook za računala za Windows. Korisnici mogu nastaviti pristupati javnim mapama pomoću aplikacije OWA ili Outlook za Mac.

Dodatne informacije potražite u članku [Kontrolirane veze s javnim mapama u programu Outlook.](https://aka.ms/controlpf)
