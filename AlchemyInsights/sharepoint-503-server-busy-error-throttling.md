---
title: Ograničavanje sustava SharePoint Online
ms.author: pebaum
author: pebaum
ms.date: 9/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.custom:
- "9000149"
- "1662"
- "3491"
ms.openlocfilehash: 59104ef96c95de4e4bc7744825245bdafba97d7c
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931218"
---
# <a name="sharepoint-online-throttling"></a>Ograničavanje sustava SharePoint Online

**Važno**: Mnogi korisnici sustava SharePoint Online i OneDrive pokrenuti poslovne kritične aplikacije protiv servisa koji se izvodi u pozadini. To uključuje migraciju sadržaja, sprječavanje gubitka podataka (DLP) i sigurnosna rješenja. Tijekom ovih dosad nezabilježenih vremena poduzimamo korake kako bismo osigurali da usluge sustava SharePoint Online i OneDrive ostanu vrlo dostupne i pouzdane za korisnike koji više nego ikad ovise o usluzi.

U prilog tom cilju, implementirali smo stroža ograničenja regulacije pozadinskih aplikacija (migracije, DLP i backup rješenja) tijekom radnih dana. Trebali biste očekivati da ove aplikacije će postići vrlo ograničen propusnost tijekom tih vremena. Međutim, tijekom večernjih i vikend sati za regiju, usluga će biti spremna za obradu znatno veći volumen zahtjeva iz pozadinskih aplikacija.

**503 poslužitelj je zauzet greška**

Korisnici mogu primiti 503 poslužitelj je zauzet greška prilikom pokušaja navigacije do SharePoint ili OneDrive web-mjesta. 

Ta je pogreška moguće uzrokovati ograničavanjem unutar servisa sustava SharePoint. SharePoint Online koristi ograničavanje za održavanje optimalnih performansi i pouzdanosti servisa sustava SharePoint Online. Ograničavanje ograničava broj korisničkih akcija ili istodobnih poziva (po skripti ili kodu) kako bi se spriječilo prekomjerno korištenje resursa. 

Dodatne informacije o regulaciji potražite u odjeljku [Izbjegavanje ograničavanja ili blokiranja u sustavu SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).

Ako smatrate da ta pogreška nije povezana s ograničavanjem, možete provjeriti postoji li aktivno održavanje na vašem klijentu tako da odete do [centra za poruke](https://portal.office.com/adminportal/home#/MessageCenter).

 Naposljetku, provjerite da posjetite stranicu [Zdravlje servisa](https://portal.office.com/adminportal/home#/servicehealth) da biste provjerili ima li savjeta/incidenata koji se mogu pojaviti.

