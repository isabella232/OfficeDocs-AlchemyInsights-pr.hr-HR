---
title: 726 blokiranje prosljeđivanja e-pošte
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "726"
- "1200004"
ms.assetid: 8865c68e-7e8a-4135-a254-d7f69f1ded30
ms.openlocfilehash: c0d9ed14f83d3c7d47e1728d5ed9ca3a19412ad2
ms.sourcegitcommit: f74c9698a31634154ce58dda8b3145bb10685ace
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/23/2020
ms.locfileid: "48219847"
---
# <a name="blocking-or-unblocking-email-forwarding"></a>Blokiranje ili deblokiranje prosljeđivanja e-pošte

Da biste omogućili ili onemogućili prosljeđivanje e-pošte za određeni poštanski sandučić, pročitajte članak [Konfiguriranje prosljeđivanja e-pošte](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).

Na razini korisnika kontrola vanjskog prosljeđivanja obavlja se pomoću izlaznog pravilnika o suzbijanju neželjene pošte. Ako je postavljena na Isključeno ili automatsko, možda blokira prosljeđivanje e-pošte pomoću pogreške "550 5.7.520 Access denied, vaša tvrtka ili ustanova ne dopušta pogrešku za vanjsko prosljeđivanje". Nakon toga, ako je prosljeđivanje postavljeno na blokiranje, to je pogreška koju će korisnici vidjeti.

Ako je prosljeđivanje blokirano, provjerite je li pravilo konfigurirano tako da omogući vanjsko automatsko prosljeđivanje. Pravilnik o izlaznom filtriranju neželjene pošte možete provjeriti iz centra za sigurnost i usklađenost ili pokretanjem naredbe Get-Hostedespamfilterpolicy | FL naziv, Autoforwardingmodu. Ako želite postaviti blokiranje automatskog prosljeđivanja, ta će vam naredba odmah reći stanje pravilnika.

Imajte na glavi: preporučuje se da vanjsko automatsko prosljeđivanje bude onemogućeno na zadanom pravilniku o izlaznom filtriranju neželjene pošte i omogućite ga samo korisnicima kojima je potreban vanjski prijenos stvaranjem prilagođenog pravilnika za te korisnike. Dodatne informacije možete pročitati u [konfiguriranju vanjskog prosljeđivanja e-pošte u sustavu Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).