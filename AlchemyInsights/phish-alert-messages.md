---
title: 2491 upozorite poruke e-pošte iz ' Phish isporučen zbog klijenta ili korisnici nadjačati ' pravilnik
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
ms.openlocfilehash: 5b5faa08542cb5878107f10afb34427f636562ac
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47728603"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a>Upozorite poruke e-pošte s servisa ' Phish isporučen zbog korisnika ili pravila nadjačavanja klijenta

Zadana pravila upozorenja koja se naziva "Phish isporučen zbog korisnika ili nadjačavanja klijenta" odkotrljali su se stanarima sa sustavom Office 365 ATP P1 i P2 licenci. Ako ste primili ovo upozorenje, slijedite upute za istragu:

1. U poruci upozorenja kliknite **Prikaži upozorenje** da biste prešli na stranicu s **upozorenjima** u centru za sigurnost & usklađenosti.

2. Odaberite upozorenje da biste vidjeli mogućnost **prikaza popisa poruka** ili **Prikaz poruka u programu Explorer**. Obje te mogućnosti odvesti će vas do pojedinosti poruke, koja sadrži ID poruke. Imajte na čemu da će veza eksplorera za prijetnje automatski filtrirati poruke koje odgovaraju kriterijima upozorenja. Možda ćete morati prilagoditi filtar datuma u eksploreru za prijetnje.

Poruka o krađi identiteta isporučena je zbog ručnog konfiguriranog premošćivanja:

- Dopušteni pošiljatelj ili domena koje je postavio korisnik.

- Dopušteni pošiljatelj ili domena koje je administrator postavio u pravilnik o suzbijanju neželjene pošte.

- Dopuštena IP adresa u pravilima filtra veze.

- Pravilo protoka pošte (poznato i kao pravilo prijenosa) koje je konfigurirano tako da dopušta poruke u programu.

Ako smatrate da je poruka neispravno označena kao Phish, upotrijebite [dodatak za poruke](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) programa Outlook da biste Microsoftu poslali uzorke poruka.
