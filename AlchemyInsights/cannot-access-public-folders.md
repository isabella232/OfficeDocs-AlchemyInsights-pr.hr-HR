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
ms.openlocfilehash: a579b89b68bfb8432adfe64b155803eda2c3b086
ms.sourcegitcommit: a3b42ee05224846327d353b48a8c67dab724f6eb
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/21/2020
ms.locfileid: "42891741"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook se ne može povezati s javnim mapama

Ako pristup javnoj mapi ne funkcionira za neke korisnike, pokušajte sljedeće:

Povežite se s EXO PowerShell i konfigurirajte parametar DefaultPublicFolderMailbox na računu problema da odgovara parametru na radnom korisničkom računu.

Primjer:

Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox

Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<vrijednost iz prethodne naredbe>

Pričekajte najmanje jedan sat da promjena stupi na snagu.

Ako problem ostane, slijedite [ovaj postupak](https://aka.ms/pfcte) da biste otklonili poteškoće s pristupom javnim mapama pomoću programa Outlook.