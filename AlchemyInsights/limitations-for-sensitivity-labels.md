---
title: Ograničenja oznaka osjetljivosti za Office datoteka u SharePoint i OneDrive
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12451"
- "9000181"
ms.openlocfilehash: e197c43712c0ead9508a1cfdf48b51d01d2ae957649f73703f9c33733e332bf5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57813150"
---
# <a name="limitations-for-sensitivity-labels-for-office-files-in-sharepoint-and-onedrive"></a>Ograničenja oznaka osjetljivosti za Office datoteka u SharePoint i OneDrive

Prilikom omogućivanja oznaka osjetljivosti za Office datoteka u SharePoint i OneDrive, imajte na umu preduvjete i ograničenja, što obuhvaća sljedeće:

- SharePoint i OneDrive ne mogu obraditi neke datoteke označene i šifrirane iz aplikacija Office za stolna računala kada datoteke sadrže podatke programa PowerQuery, podatke pohranjene u prilagođenim dodacima ili prilagođene XML dijelove.
- SharePoint i OneDrive oznake osjetljivosti ne primjenjuju automatski na postojeće datoteke koje ste već šifrirali pomoću AIP oznaka servisa Azure Information Protection (Azure Information Protection). Da biste na šifrirane datoteke primijenili oznake osjetljivosti: 
    - Provjerite jesu li AIP oznake migrirani i objavljeni u centru za Microsoft 365 usklađenost.
    - Preuzmite označene datoteke, a zatim ih prenesite na izvorno SharePoint ili OneDrive mjesto.
- Za šifrirane dokumente ispis nije podržan.

Dodatne pojedinosti o ograničenjima potražite u članku [Omogućivanje naljepnica osjetljivosti za Office datoteka u SharePoint i OneDrive](/microsoft-365/compliance/sensitivity-labels-sharepoint-onedrive-files#limitations).
