---
title: 0x8004de40 prilikom pokretanja OneDrive
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
ms.openlocfilehash: 23c57356c8bd94c1cbafb538c9318208429754115a7c4e88abc93d293b5ea6e1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53946571"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a>0x8004de40 prilikom pokretanja OneDrive

Ako se prilikom prijave u **0x8004de40** pojavljuje pogreška, OneDrive ponovno pokrenite računalo dok ste povezani s domenom na poslu ili u školi. Ako se ta pogreška pojavi nakon ponovnog pokretanja, pokušajte to dok ste povezani s domenom na poslu ili u školi:

1. Kliknite Start, a zatim  u okvir za pretraživanje upišite **cmd** ili naredbeni redak, desnom tipkom miša kliknite aplikaciju naredbenog retka, a zatim **odaberite Pokreni kao administrator**. Ako se od vas zatraži da upišete administratorsku lozinku ili potvrdu, upišite lozinku ili kliknite **Dopusti**.  

2. U prozor naredbenog retka upišite **dsregcmd /leave**  i pričekajte da se naredba dovrši. Zatim **upišite dsregcmd /join** i pričekajte da se naredba dovrši.
3. Ponovno pokrenite računalo.
