---
title: Slanje poruke e-pošte pružanjem ID-a mrežne poruke
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
ms.openlocfilehash: e4a0a3d9b4fede9198c8a235d05945b30a6e0807
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50743601"
---
# <a name="submit-an-email-message-by-providing-the-network-message-id"></a>Slanje poruke e-pošte pružanjem ID-a mrežne poruke

1. U nastavku **nove prijave za podnošenje** odaberite ID **e-pošte** i **mrežne poruke**.
2. Slijedite ove korake da biste pronašli ID poruke za poruku e-pošte u programu Outlook:
    1. Dvokliknite poruku e-pošte da biste je otvorili.
    1. Odaberite   >  **Svojstva** datoteke.
    1. Otvorite Notepad ili prazan dokument programa Word, a zatim kopirajte i zalijepite sadržaj koji se nalazi u okviru **Internetska zaglavlja** u otvoreni dokument radi bolje vidljivosti.
    1. Pronađite polje **X-MS-Exchange-Organization-Network-ID** . Vrijednost iza **:** je ID koji vam je potreban za podnošenje.
3. U odjeljku **Primatelji**, ako je poruka e-pošte sletjela u mapu Bezvrijedna pošta za sve primatelje ove e-pošte, odaberite **Odaberi sve**. Ako nije, odaberite samo korisnika koji je prijavio problem.
4. Ako ste odabrali **razlog za podnošenje**, navedite je li poruka trebala **biti blokirana kao** **neželjena pošta**, **phishing** ili **zlonamjerni softver**, a zatim odaberite **Pošalji**.

Da biste doznali više, pročitajte članak [upute za skeniranje u programu Microsoft radi skeniranja](https://go.microsoft.com/fwlink/?linkid=2101479).
