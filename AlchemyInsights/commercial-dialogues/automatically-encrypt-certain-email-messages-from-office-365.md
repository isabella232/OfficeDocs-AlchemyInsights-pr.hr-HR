---
title: Automatsko šifriranje određenih poruka e-pošte iz sustava Office 365
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
ms.openlocfilehash: 74f9733196004fd7a78eeb290c948a9f35ac2a31b3c5b00bf82e44081aac8637
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53988827"
---
# <a name="automatically-encrypt-certain-email-messages-from-office-365"></a>Automatsko šifriranje određenih poruka e-pošte iz sustava Office 365

1. U centru [Exchange administratora odaberite](https://outlook.office365.com/ecp/) **tijek pošte > pravila**. 
2. Kliknite **ikonu Novo (+),** a zatim Primijeni **šifriranje poruka sustava Office 365 zaštitu prava na poruke**.
3. U **okvir** Naziv unesite naziv pravila, npr. *Šifriraj sve poruke*.
4. U **aplikaciji Primijeni ovo pravilo ako** odaberite **[Primijeni na sve poruke]**. 
5. Pokraj polja **Učinite sljedeće kliknite** Odaberi **jedno**. 
6. Na **padajućem izborniku RMS** predloška odaberite **Šifriraj**, a zatim kliknite U **redu**. (Ako vam se ta mogućnost ne vidi, to znači da vaš plan ne sadrži automatsko šifriranje. No možete ga dodati!)
7. Potvrdite okvir **Nadzor ovog pravila s razinom ozbiljnosti,** a zatim odaberite željenu razinu. Ako vaša tvrtka ima ugovorne obaveze slanja šifriranih poruka e-pošte, preporučujem da postavite razinu na **Visoko**.
8. U **odjeljku Odabir modela za ovo pravilo** kliknite **Nametanje**. 
9. Odaberite bilo koji neobavezni odabir (s popisa neobaveznih odabira koje možete odabrati u ovom trenutku, od kojih se mnoge mogu ostaviti uz zadanu postavku jednostavnosti).
10. Kliknite **Spremi**.

> [!IMPORTANT]
> Uvijek se možete vratiti i urediti to pravilo kasnije.

Dodatne informacije o stvaranju pravila za šifriranje potražite u članku Definiranje pravila tijeka [pošte radi šifriranja poruka e-pošte Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)

