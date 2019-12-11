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
ms.openlocfilehash: a9305b175e1ca0b992c014a73705447d67e037bc
ms.sourcegitcommit: cbbd46fa9a32873c5446d9fd5a532cea0300b795
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39959487"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook se ne može povezati s javnim mapama

Ako pristup javnim mapama ne funkcionira za nekoliko korisnika, pokušajte sljedeće:

Povežite se s EXO PowerShell i konfigurirati Defaultpublicfolderpoštanski sandučić na problem korisničkog računa da odgovara jedan na radnom korisničkom računu.

Primjer:

Get-poštanski sandučić WorkingUser | ft Defaultpublicfolderpoštanski sandučić, Učinkovitjepublicfolderpoštanski sandučić

Set-poštanski sandučić ProblemUser-Defaultpublicfolderpoštanski sandučić \<vrijednosti iz prethodne naredbe>

Pričekajte najmanje jedan sat kako bi promjena stupile na snagu.