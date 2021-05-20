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
ms.openlocfilehash: 2b373423cf3e63b76a62465dd62076c023580e94
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52544570"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a>Upozorenje o porukama e-pošte iz pravilnika "Phish Delivered due to tenant or user override" (Phish Isporučeno zbog nadjačavanja klijenta ili nadjačavanja korisnika)

Zadani pravilnik upozorenja pod nazivom "Phish Delivered due to tenant or user override" (Phish Isporučeno zbog nadjačavanja klijenta ili nadjačavanja korisnika) najmoprimateljima s programom Microsoft Defender za Office 365 P1 i P2 licencama. Ako ste primili ovo upozorenje, evo koraka za istraživanje:

1. U poruci upozorenja kliknite Prikaz upozorenja da **biste** na stranici **Upozorenja u** centru za & usklađenost.

2. Odaberite upozorenje da biste vidjeli mogućnost Prikaz **popisa poruka ili** Prikaz poruka u **pregledniku Explorer**. Obje će vas mogućnosti odvesti do detalja poruke, što obuhvaća ID poruke. Imajte na umu da će veza Eksplorer za prijetnje automatski filtrirati poruke koje odgovaraju kriterijima upozorenja. Možda ćete morati prilagoditi filtar datuma u eksploreru za prijetnje.

Poruka o krađi identiteta isporučena je zbog ručno konfiguriranog nadjačavanja:

- Dopušteni pošiljatelj ili domena koje je postavio korisnik.

- Dopušteni pošiljatelj ili domena koje je administrator postavio u pravilniku o zaštiti od neželjene pošte.

- Dopuštena IP adresa u pravilniku filtra veze.

- Pravilo tijeka pošte (poznato i kao pravilo prijenosa) koje je konfigurirano tako da dopušta poruke u programu.

Ako vjerujete da je poruka netočno označena kao fazana, pomoću dodatka Outlook [report message (Poruka](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) izvješća) pošaljite microsoftu uzorke poruka.
