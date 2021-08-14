---
title: Vraćanje izbrisane Microsoft 365 grupe
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "98"
- "1200024"
ms.assetid: bc0396ea-c426-4d1d-bb89-ced602d06fb6
ms.openlocfilehash: 6262ca04335c355fb4de41a9e1d854b666f47e10321a843717d6eb951c46cafd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53959018"
---
# <a name="restore-a-deleted-microsoft-365-group"></a>Vraćanje izbrisane Microsoft 365 grupe

Izbrisanu grupu možete vratiti Microsoft 365 ili Microsoft Teams roku od 30 dana od brisanja.

1. Idite [na Centar za administratore okruženja Microsoft 365](https://aka.ms/RestoreDeletedGroup) se prijavite na popis izbrisanih grupa i timova.

    **Napomena:** Prijavite se pomoću računa dodijeljenog administratoru klijenta ili administratoru grupe.

1. Odaberite izbrisanu Microsoft 365 grupu/Teams koju želite vratiti, a zatim **kliknite vrati grupu**.

    Ako grupu nije moguće vratiti zbog smtp adrese koja je u sukobu, pomoću sljedeće naredbe pronađite objekt koji uzrokuje sukob i uklonite SMTP adresu:

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    **Napomena:** U nekim slučajevima može potrajati i do 24 sata da se grupa i svi njezini podaci vrate.

    Dodatne informacije ili upute za vraćanje grupa pomoću komponente PowerShell potražite u članku Vraćanje [izbrisane Microsoft 365 grupe](https://go.microsoft.com/fwlink/?linkid=867802).