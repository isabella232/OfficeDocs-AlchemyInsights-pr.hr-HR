---
title: Nadzor u Microsoft 365
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: a5acd322186f8f4b7734f8541877a642a553288e10b3c122e4f276b9bb611308
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53988947"
---
# <a name="auditing-in-microsoft-365"></a>Nadzor u Microsoft 365

Evo nekoliko stvari koje biste trebali znati o nadzoru u Microsoft 365:

1. Exchange administratorske aktivnosti po zadanom su nadzirane.
1. Po zadanom uključujemo nadzor poštanskih sandučića za sve korisnike. Da biste pročitali više o tome, [kliknite ovdje](https://techcommunity.microsoft.com/t5/Security-Privacy-and-Compliance/Exchange-Mailbox-Auditing-will-be-enabled-by-default/ba-p/215171). Do tada, ako želite ručno omogućiti upute za jednu osobu ili cijelu organizaciju, u nastavku odaberite gumb Uključi nadzor poštanskog sandučića.
1. Microsoft 365 Poštanski sandučići grupe i poštanski sandučići javne mape ne podržavaju zapisivanje nadzora.
1. Za SharePoint/OneDrive nije potrebna dodatna konfiguracija za omogućeno nadziranje. Da biste saznali koje se aktivnosti nad kojima se obavlja nadzor, pogledajte sljedeće:
    1. [Aktivnosti datoteka](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#file-and-page-activities)
    1. [Aktivnosti mape](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
    1. [Zajedničko korištenje i aktivnosti programa Access](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities).
1. Popis svih nadziranih aktivnosti po servisu pogledajte u članku [Nadzirane aktivnosti](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#audited-activities).
