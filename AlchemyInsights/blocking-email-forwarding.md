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
ms.openlocfilehash: 2f3528375d251542fd82761d00c776706de2e23c
ms.sourcegitcommit: f7b82f75a5400e992ecbd48a666783354e2e2871
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 10/15/2020
ms.locfileid: "48473093"
---
# <a name="blocking-or-unblocking-email-forwarding"></a>Blokiranje ili deblokiranje prosljeđivanja e-pošte

Da biste omogućili ili onemogućili prosljeđivanje e-pošte za određeni poštanski sandučić, pročitajte članak [Konfiguriranje prosljeđivanja e-pošte](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).

Na razini korisnika kontrola vanjskog prosljeđivanja obavlja se pomoću izlaznog pravilnika o neželjenoj pošti. Pravilnik o izlaznom filtriranju neželjene pošte možete provjeriti iz centra za sigurnost i usklađenost [ovdje] ( https://protection.office.com/antispam) ili pomoću [naredbe Dohvati-Hostedespamfilterpolicy](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy).

Ako vam se prikaže sljedeća pogreška: **"550 5.7.520 je odbijen pristup, vaša tvrtka ili ustanova ne dopušta vanjsko prosljeđivanje"**, provjerite je li pravilo konfigurirano tako da omogući vanjsko automatsko prosljeđivanje.

**Upozorenje:** Preporučuje se da vanjsko automatsko prosljeđivanje bude onemogućeno na zadanom pravilniku o izlaznom filtriranju neželjene pošte i omogućite ga samo korisnicima kojima je potreban vanjski prijenos stvaranjem prilagođenog pravilnika za te korisnike. Dodatne informacije možete pročitati u [konfiguriranju vanjskog prosljeđivanja e-pošte u sustavu Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).