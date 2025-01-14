---
title: 2491 Upozorenje porukama e-pošte iz pravilnika "Phish Isporučeno zbog klijenta ili nadjačavanja korisnika"
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 90b078147bbb1e60cba0a2de6e49a862469f93aa
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58316350"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a>Upozorenje porukama e-pošte iz pravilnika "Phish Isporučeno zbog klijenta ili nadjačavanja korisnika"

Zadani pravilnik upozorenja pod nazivom **Phish Delivered** zbog nadjačavanja klijenta ili korisnika dostupan je u tvrtkama ili ustanovama s programom Microsoft Defender za Office 365 P1 i P2. Ako ste primili ovo upozorenje, evo koraka za istraživanje:

1. U poruci upozorenja kliknite Prikaz upozorenja **da biste** na stranici **Upozorenja na** Microsoft 365 Defender portalu.

2. Odaberite upozorenje da biste vidjeli mogućnost Prikaz **popisa poruka ili** Prikaz poruka u **pregledniku Explorer**. Obje će vas mogućnosti odvesti do detalja poruke, što obuhvaća ID poruke. Imajte na umu da će veza Eksplorer za prijetnje automatski filtrirati poruke koje odgovaraju kriterijima upozorenja. Možda ćete morati prilagoditi filtar datuma u eksploreru za prijetnje.

Poruka o krađi identiteta isporučena je zbog ručno konfiguriranog nadjačavanja:

- Dopušteni pošiljatelj ili domena koje je postavio korisnik.
- Dopušteni pošiljatelj ili domena koje je administrator postavio u pravilniku o zaštiti od neželjene pošte.
- Dopuštena IP adresa u pravilniku filtra veze.
- Pravilo tijeka pošte (poznato i kao pravilo prijenosa) koje je konfigurirano tako da dopušta poruke u programu.

Ako mislite da je poruka pogrešno označena kao krađa identiteta, pomoću slanja [administratora](https://docs.microsoft.com/microsoft-365/security/office-365-security/admin-submission) prijavite poruku Microsoftu.

Korisnici mogu pomoću [dodatka Report Message](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) ili dodatka Report Phishing u programu Outlook poslati uzorke poruka Microsoftu.
