---
title: Poruka dobrodošlice u grupama microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "5685"
ms.openlocfilehash: d82931ae6978a09e674b00640d1dd413bcce7cfd
ms.sourcegitcommit: b196100759b29aecd62b693a2bfedbbd25a697c6
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 05/19/2020
ms.locfileid: "44357321"
---
# <a name="welcome-message-in-microsoft-365-groups"></a>Poruka dobrodošlice u grupama microsoft 365

Novi korisnici koji se pridružuju grupi Microsoft 365 primit će e-poštu dobrodošlice ako je svojstvo "UnifiedGroupWelcomeMessageEnabled" istinito.

U slučaju da želite onemogućiti poruku dobrodošlice, koristite sljedeću naredbu [EXO PowerShell:](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps)

`
Set-UnifiedGroup <groupname> -UnifiedGroupWelcomeMessageEnabled:$False
`
