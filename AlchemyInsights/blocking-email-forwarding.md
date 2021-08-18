---
title: Blokiranje i deblokiranje vanjskog automatskog prosljeđivanja e-pošte
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
ms.openlocfilehash: fe9e52023b809b38c43332a10a1184d114798cfe
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58315866"
---
# <a name="block-or-unblock-eternal-automatic-email-forwarding"></a>Blokiranje i deblokiranje vječitog automatskog prosljeđivanja e-pošte

Da biste omogućili ili onemogućili prosljeđivanje e-pošte za određeni poštanski sandučić, pogledajte [konfiguriranje prosljeđivanja e-pošte](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).

Administratori mogu upravljati vanjskim prosljeđivanjem za organizaciju pomoću [pravilnika o odlaznom neželjenom sadržaju](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-outbound-spam-policy). Pravilnikima o odlaznom neželjenom sadržaju na Microsoft 365 Defender portalu upravljate putem <https://security.microsoft.com/antispam> cmdleta [Get-HostedOutboundSpamFilterPolicy](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy) u Exchange Online PowerShell.

Ako vam se prikazuje sljedeća pogreška: **"550 5.7.520 Access denied, Vaša** tvrtka ili ustanova ne dopušta vanjsko prosljeđivanje", provjerite je li pravilnik konfiguriran tako da omogući vanjske automatski prosljeđivanje poruka.

**Napomena:** preporučena je zadana vrijednost  **Automatski –** kontrola sustava za postavku Pravila automatskog prosljeđivanja u zadanom pravilniku o odlaznom filtriranju neželjene pošte (automatsko vanjsko prosljeđivanje je blokirano, interno automatsko prosljeđivanje i dalje funkcionira). Trebali biste stvoriti prilagođene pravilnike za filtriranje neželjene pošte i koristiti vrijednost Na **– prosljeđivanje** omogućeno je samo za korisnike kojima je potrebno vanjsko automatsko prosljeđivanje e-pošte. Dodatne informacije potražite u članku Konfiguriranje [vanjskog prosljeđivanja e-pošte u Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).
