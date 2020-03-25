---
title: Ograničavanje migracije sustava SharePoint s 503 pogreške
ms.author: pebaum
author: pebaum
ms.date: 8/8/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000136"
- "2541"
ms.openlocfilehash: 7e12c74d33e3cee7c626ad899a4e7f2f0a409bca
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931650"
---
# <a name="sharepoint-migration-throttling-with-503-errors"></a>Ograničavanje migracije sustava SharePoint s 503 pogreške

**Važno**: Mnogi korisnici sustava SharePoint Online i OneDrive pokrenuti poslovne kritične aplikacije protiv servisa koji se izvodi u pozadini. To uključuje migraciju sadržaja, sprječavanje gubitka podataka (DLP) i sigurnosna rješenja. Tijekom ovih dosad nezabilježenih vremena poduzimamo korake kako bismo osigurali da usluge sustava SharePoint Online i OneDrive ostanu vrlo dostupne i pouzdane za korisnike koji više nego ikad ovise o usluzi.

U prilog tom cilju, implementirali smo stroža ograničenja regulacije pozadinskih aplikacija (migracije, DLP i backup rješenja) tijekom radnih dana. Trebali biste očekivati da ove aplikacije će postići vrlo ograničen propusnost tijekom tih vremena. Međutim, tijekom večernjih i vikend sati za regiju, usluga će biti spremna za obradu znatno veći volumen zahtjeva iz pozadinskih aplikacija.

**503 pogreške prilikom migracije u SharePoint Online**

Čini se da migrirate u SharePoint Online i primate 503 pogreške. Slijedite korake u nastavku kako bismo vam mogli pomoći što je prije moguće. 

1. Kliknite **Obratite se službi za podršku**, a zatim Novi zahtjev za **servisom**.
2. Za naslov i opis upišite **Ograničavanje migracije sustava SharePoint s 503**.
3. Nakon podnošenja karte ažurirajte je sljedećim informacijama:
    - Koliko je ostalo migracije (na primjer, koliko tbs?).
    - Datum početka i završetka migracije.
    - Opišite odakle migrirate sadržaj, kao što su SharePoint Server, Box, GDrive, Zajedničko korištenje datoteka itd..
    - Procijeniti broj pogrešaka regulacije (na primjer, x gasa na sat?) i kada se regulacija dogodila.
    - Koji alat za migraciju koristite (na primjer, SPMT ili ShareGate).


