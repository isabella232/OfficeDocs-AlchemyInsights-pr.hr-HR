---
title: 0x8004de40 prilikom pokretanja servisa OneDrive
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
- "6886"
- "9003837"
ms.openlocfilehash: e329d7fe881a0fc9514584e06aa2d6e8ebab5b11
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813644"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a>0x8004de40 prilikom pokretanja servisa OneDrive

Ako vam se prilikom 0x8004de40 **na** OneDrive prikazuje pogreška, ponovno pokrenite računalo dok ste povezani s domenom tvrtke ili škole. Ako se ta pogreška pojavi nakon ponovnog pokretanja, pokušajte to dok ste povezani s domenom na poslu ili u školi:

1. Kliknite Start, a zatim  u okvir za pretraživanje upišite **cmd** ili naredbeni redak, desnom tipkom miša kliknite aplikaciju naredbenog retka, a zatim **odaberite Pokreni kao administrator**. Ako se od vas zatraži da upišete administratorsku lozinku ili potvrdu, upišite lozinku ili kliknite **Dopusti**.  

2. U prozor naredbenog retka upišite **dsregcmd /leave**  i pričekajte da se naredba dovrši. Zatim **upišite dsregcmd /join** i pričekajte da se naredba dovrši.
3. Ponovno pokrenite računalo.
