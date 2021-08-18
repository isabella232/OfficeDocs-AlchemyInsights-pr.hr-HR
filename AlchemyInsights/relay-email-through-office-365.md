---
title: Razmjena e-pošte putem sustava Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "154"
- "3000003"
ms.assetid: 84191e23-496c-495a-a2ec-28c5ae0d4c0b
ms.openlocfilehash: f02daad7d4b4a11f8d8bb1ef1467db5809cbd291
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58324354"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email"></a>Postavljanje višefunkcijskog uređaja ili aplikacije za slanje e-pošte

Informacije o dostupnim mogućnostima i upute potražite u članku [Postavljanje višefunkcijskog uređaja ili aplikacije za slanje e-pošte pomoću sustava Microsoft 365](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).
  
Ako imate uređaj ili aplikaciju koja je nedavno prestala funkcionirati, najčešći su problemi:

- **Pogreške povezane s provjerom autentičnosti prilikom korištenja slanja KLIJENTA SMTP-a** Nedavno smo napravili neke promjene povezane s načinom na koji funkcionira SMTP provjera autentičnosti. Dodatne informacije o rješavanju problema potražite u odjeljku Provjera autentičnosti koja nije uspješna u odjeljku Rješavanje problema s [pisačima, skenerima](https://docs.microsoft.com/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off#error-authentication-unsuccessful)i LOB aplikacijama koje šalju e-poštu pomoću Microsoft 365 ili Office 365 .
- **Prihvaćamo samo verziju TLS 1.2 prilikom sigurne veze s Office 365** Ako koristite sigurnu vezu (TLS), provjerite podržava li uređaj za aplikaciju TLS 1.2. Dodatne informacije potražite u članku [Priprema za TLS 1.2 u Office 365 i Office 365 GCC](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365).
 
Ostale probleme i rješenja pronaći ćete u članku Rješavanje problema [s pisačima,](https://docs.microsoft.com/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off)skenerima i LOB aplikacijama koje šalju e-poštu pomoću Microsoft 365 ili Office 365 .

Da biste vidjeli zahvaćene uređaje, idite na izvješće [Klijenti SMTP provjere autentičnosti](https://protection.office.com/mailflow/dashboard).

**Napomena:** Exchange Online ne odgovara scenarijima masovne pošte. Da biste slali skupnu komercijalnu e-poštu (npr. biltene klijenata), trebali biste koristiti davatelje usluga drugih proizvođača koji su specijalizirani za te servise.
