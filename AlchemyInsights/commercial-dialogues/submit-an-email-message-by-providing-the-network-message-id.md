---
title: Slanje poruke e-pošte tako da unesite ID mrežne poruke
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 1a6f9815a36cc267a815ff9757d713afed5d95aec4f7c537135c88cadf26cc51
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53929909"
---
# <a name="submit-an-email-message-by-providing-the-network-message-id"></a>Slanje poruke e-pošte tako da unesite ID mrežne poruke

1. U **brošuri Novi podnesak** odaberite **E-pošta** i **ID mrežne poruke**.
2. Slijedite ove korake da biste pronašli ID poruke za poruku e-pošte u Outlook:
    1. Dvokliknite poruku e-pošte da biste je otvorili.
    1. Odaberite **Svojstva**  >  **datoteke**.
    1. Otvorite Blok za pisanje ili prazan dokument programa Word, a zatim kopirajte i zalijepite sadržaj pronađen u okviru **Internetska** zaglavlja u otvoreni dokument radi bolje vidljivosti.
    1. Pronađite polje **X-MS-Exchange-Organization-Network-Message-ID.** Vrijednost nakon : **jest** ID koji vam je potreban za slanje.
3. U **odjeljku Primatelji** ako je poruka e-pošte sletela u mapu bezvrijedne pošte za sve primatelje te poruke e-pošte, **odaberite Odaberi sve**. Ako nije, odaberite samo korisnika koji je prijavio problem.
4. U **odjeljku Razlog za slanje**, ako odaberete Treba biti blokirano , navedite je li poruka trebala biti blokirana kao **Neželjena** pošta ,  **Krađa identiteta** ili **Zlonamjerni** softver , a zatim odaberite **Pošalji**.

Dodatne informacije potražite u članku Kako microsoftu poslati sumnjivu [neželjenu poštu, phish, URL-ove](https://go.microsoft.com/fwlink/?linkid=2101479)i datoteke radi skeniranja.
