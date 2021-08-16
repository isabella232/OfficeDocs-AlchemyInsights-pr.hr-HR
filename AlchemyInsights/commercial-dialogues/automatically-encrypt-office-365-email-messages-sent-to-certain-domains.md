---
title: Automatsko šifriranje Office 365 poruke e-pošte poslane određenim domenama
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
ms.openlocfilehash: 5a285f36aeb814e3b1d361c8cbffd5a6bef0770d10082d24654c7bbda59ce65b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54082178"
---
# <a name="automatically-encrypt-office-365-email-messages-sent-to-certain-domains"></a>Automatsko šifriranje Office 365 poruke e-pošte poslane određenim domenama

1. U centru [Exchange administratora odaberite](https://outlook.office365.com/ecp/) **tijek pošte > pravila**. 
2. Kliknite **ikonu Novo (+),** a zatim Primijeni **šifriranje poruka sustava Office 365 zaštitu prava na poruke**.
3. U **okvir** Naziv unesite naziv pravila, primjerice Šifriraj *poruke poslane u contoso.com*.
4. U **domenu Primijeni ovo pravilo ako** **odaberite Primatelj > je domena**. 
5. Unesite naziv domene, npr. **contoso.com**.
6. Kliknite **ikonu Dodaj (+),** a zatim U **redu.**
7. Pokraj polja **Učinite sljedeće kliknite** Odaberi **jedno**. 
8. Na **padajućem izborniku RMS** predloška odaberite **Šifriraj**, a zatim kliknite U **redu**. (Ako vam se ta mogućnost ne vidi, to znači da vaš plan ne sadrži automatsko šifriranje. No možete ga dodati!)
9. Odaberite bilo koji neobavezni odabir (s popisa neobaveznih odabira koje možete odabrati u ovom trenutku, od kojih se mnoge mogu ostaviti uz zadanu postavku jednostavnosti).
10. Kliknite **Spremi**.

> [!IMPORTANT]
> Uvijek se možete vratiti i urediti to pravilo kasnije.

Dodatne informacije o stvaranju pravila za šifriranje potražite u članku Definiranje pravila tijeka [pošte radi šifriranja poruka e-pošte Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)