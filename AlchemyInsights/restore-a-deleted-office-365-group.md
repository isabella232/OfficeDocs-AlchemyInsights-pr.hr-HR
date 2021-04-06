---
title: Vraćanje izbrisane grupe sustava Microsoft 365
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
ms.openlocfilehash: caa2c8987eecb89bac3469bf9471847858cab0ba
ms.sourcegitcommit: ec99a3a2e1e6a13d9a829d65ad1692a607dc3a17
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/06/2021
ms.locfileid: "51597435"
---
# <a name="restore-a-deleted-microsoft-365-group"></a>Vraćanje izbrisane grupe sustava Microsoft 365

Izbrisanu grupu sustava Microsoft 365 ili Microsoft Teams možete vratiti u roku od 30 dana od brisanja.

1. Idite u [centar za administratore sustava Microsoft 365](https://aka.ms/RestoreDeletedGroup) da biste se prijavite i na popisu popisa izbrisanih grupa i timova.

    **Napomena:** Prijavite se pomoću računa dodijeljenog administratoru klijenta ili administratoru grupe.

1. Odaberite izbrisanu grupu microsoft 365/Teams koju želite vratiti i kliknite **vrati grupu**.

    Ako grupu nije moguće vratiti zbog smtp adrese koja je u sukobu, pomoću sljedeće naredbe pronađite objekt koji uzrokuje sukob i uklonite SMTP adresu:

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    **Napomena:** U nekim slučajevima može potrajati i do 24 sata da se grupa i svi njezini podaci vrate.

    Dodatne informacije ili upute za vraćanje grupa pomoću komponente PowerShell potražite u članku [Vraćanje izbrisane grupe sustava Microsoft 365](https://go.microsoft.com/fwlink/?linkid=867802).