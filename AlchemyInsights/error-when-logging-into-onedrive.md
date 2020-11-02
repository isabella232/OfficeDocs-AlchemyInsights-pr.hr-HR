---
title: 0x8004de40 pogreška prilikom pokretanja servisa OneDrive
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
- "6886"
- "9003837"
ms.openlocfilehash: f689fcf9432e9b356843efe73ed0f79a32735e6f
ms.sourcegitcommit: 1ac3474897abb7c4969e222f934294e05f468536
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 10/30/2020
ms.locfileid: "48822999"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a>0x8004de40 pogreška prilikom pokretanja servisa OneDrive

Ako se prilikom prijave na OneDrive pojavi pogreška **0x8004de40** , ponovno pokrenite računalo dok ste povezani s domenom rada ili škole. Ako se ta pogreška pojavi nakon ponovnog pokretanja, isprobajte ovo dok ste spojeni na domenu rada ili škole:

1. Kliknite Start, a zatim u okvir za pretraživanje upišite **cmd** ili **naredbeni upit**  , desnom tipkom miša kliknite aplikaciju naredbenog upita, a zatim odaberite  **Pokreni kao administrator** . Ako se od vas zatraži administratorska lozinka ili potvrda, upišite lozinku ili kliknite **Dopusti** .  

2. U prozoru naredbenog upita upišite **dsregcmd/ostavite**  i pričekajte da se naredba dovrši. Zatim upišite **dsregcmd/pridružite** se i pričekajte da se naredba dovrši.
3. Ponovno pokrenite računalo.
