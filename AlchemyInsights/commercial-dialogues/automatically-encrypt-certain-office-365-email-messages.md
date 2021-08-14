---
title: Automatsko šifriranje određenih Office 365 e-pošte
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
ms.openlocfilehash: 8ae1c6853f41790efc3b24a9dc696bccf8385967d8c9219a1200e287e6ce32a1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53949559"
---
# <a name="automatically-encrypt-certain-office-365-email-messages"></a>Automatsko šifriranje određenih Office 365 e-pošte

Poruke koje korisnici šalju određenim vanjskim osobama ili tvrtkama ili ustanovama možete automatski šifrirati. Da biste to učiniti, učinite sljedeće:

1. U centru [Exchange administratora odaberite](https://outlook.office365.com/ecp/) **tijek pošte > pravila**. 
2. Kliknite **ikonu Novo (+),** a zatim Primijeni **šifriranje poruka sustava Office 365 zaštitu prava na poruke**.
3. U **okvir** Naziv unesite naziv pravila, npr. Šifriraj *poruke poslane DrToniRamos@gmail.com*.
4. U **programu Primijeni ovo pravilo ako** odaberite Primatelj > je ta **osoba**. 
5. U **prozoru Odabir** članova odaberite ime osobe na koju želite primijeniti pravilo šifriranja, a zatim kliknite **dodaj**. 
6. Kada završite s dodavanjem korisnika, kliknite U **redu**.
7. Pokraj polja **Učinite sljedeće kliknite** Odaberi **jedno**. 
8. Na **padajućem izborniku RMS** predloška odaberite **Šifriraj**, a zatim kliknite U **redu**. (Ako vam se ta mogućnost ne vidi, to znači da vaš plan ne sadrži automatsko šifriranje. No možete ga dodati!)
9. Odaberite bilo koji neobavezni odabir (s popisa neobaveznih odabira koje možete odabrati u ovom trenutku, od kojih se mnoge mogu ostaviti uz zadanu postavku jednostavnosti).
10. Kliknite **Spremi**.

> [!IMPORTANT]
> Uvijek se možete vratiti i urediti to pravilo kasnije.

Dodatne informacije o stvaranju pravila za šifriranje potražite u članku Definiranje pravila tijeka pošte radi [šifriranja poruka e-pošte Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).

