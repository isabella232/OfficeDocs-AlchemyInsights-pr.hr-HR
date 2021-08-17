---
title: 726 Blokiranje prosljeđivanja e-pošte
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
ms.openlocfilehash: 0bff7ede02809e133dc6616452ec840f552bd4fa6c45b7987d6455b2a9ba49bf
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54059624"
---
# <a name="blocking-or-unblocking-email-forwarding"></a>Blokiranje i deblokiranje prosljeđivanja e-pošte

Da biste omogućili ili onemogućili prosljeđivanje e-pošte za određeni poštanski sandučić, pogledajte [konfiguriranje prosljeđivanja e-pošte](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).

Na razini klijenta kontrola vanjskog prosljeđivanja obavlja se pomoću pravilnika o odlaznoj neželjenoj pošti. Ovdje možete provjeriti pravilnik filtra odlazne neželjene pošte iz centra za sigurnost i usklađenost ili pomoću naredbe [Get-HostedOutboundSpamFilterPolicy](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy). [](https://protection.office.com/antispam)

Ako vam se prikazuje sljedeća pogreška: **"550 5.7.520 Access denied, Vaša** tvrtka ili ustanova ne dopušta vanjsko prosljeđivanje", provjerite je li pravilnik konfiguriran tako da omogući vanjsko automatsko prosljeđivanje.

**Napomena:** Preporučuje se da vanjski automatski pristup onemogućite u zadanom pravilniku o filtriranju neželjene pošte i omogućite ga samo korisnicima kojima je potrebno vanjsko prosljeđivanje stvaranjem prilagođenog pravilnika za te korisnike. Dodatne informacije potražite u [web-aplikaciji Konfiguriranje vanjskog prosljeđivanja e-pošte u Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).