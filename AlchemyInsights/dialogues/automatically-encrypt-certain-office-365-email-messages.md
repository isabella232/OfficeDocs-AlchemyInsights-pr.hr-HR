---
title: Automatski Šifriraj određene poruke e-pošte u sustavu Office 365
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: e4b2f4ffcacf03e145b4c6d5ff6e73a75cb7c184
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50523558"
---
# <a name="automatically-encrypt-certain-office-365-email-messages"></a>Automatski Šifriraj određene poruke e-pošte u sustavu Office 365

Možete automatski šifrirati poruke koje korisnici šalju određenim vanjskim osobama ili organizacijama. Da biste to učinili, slijedite sljedeće korake:

1. U [centru za administratore sustava Exchange](https://outlook.office365.com/ecp/)odaberite **tijek pošte > pravila**. 
2. Kliknite ikonu **Novo (+)** , a zatim kliknite **Primijeni šifriranje poruka i zaštita prava u sustavu Office 365 na poruke**.
3. U **naziv** unesite naziv pravila, primjerice *Šifriraj poruke poslane u DrToniRamos@gmail.com*.
4. **Ako primijenite ovo pravilo**, odaberite **primatelja > je ta osoba**. 
5. U prozoru **Odabir članova** odaberite ime osobe na koju želite primijeniti pravilo šifriranja, a zatim kliknite **Dodaj**. 
6. Kada završite s dodavanjem korisnika, kliknite **u redu**.
7. Pokraj polja **učinite sljedeće** kliknite **Odaberi jednu**. 
8. Na padajućem izborniku **predloška RMS** -a odaberite **Šifriraj**, a zatim kliknite **u redu**. (Ako ne vidite tu mogućnost, to znači da vaš plan ne obuhvaća automatsko šifriranje. No, možete ga dodati!)
9. Odaberite bilo koji neobavezni odabir (s popisa neobaveznih odabira koje možete učiniti u ovom trenutku, od kojih se mnogi mogu vratiti uz zadanu postavku za jednostavnost).
10. Kliknite **Spremi**.

> [!IMPORTANT]
> Uvijek se možete vratiti i urediti to pravilo kasnije.

Dodatne informacije o stvaranju pravila šifriranja potražite [u članku definiranje pravila tijeka pošte za šifriranje poruka e-pošte u sustavu Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).

