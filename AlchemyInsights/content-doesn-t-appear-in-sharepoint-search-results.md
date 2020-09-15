---
title: Sadržaj se ne prikazuje u rezultatima pretraživanja sustava SharePoint
ms.author: tlarsen
author: tklarsen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "750"
- "5300017"
ms.assetid: 693db84f-2737-4c21-b027-4ab3d121b4a8
ms.openlocfilehash: a57711434d653f5d5667776916c9251bba2370e6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47713122"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a>Sadržaj se ne prikazuje u rezultatima pretraživanja sustava SharePoint

Slijedite ove korake za otklanjanje poteškoća kada se očekivani sadržaj ne prikazuje u rezultatima pretraživanja:
  
1. Provjerite je li **web-mjesto** koje sadrži očekivani sadržaj postavljeno tako da dopušta prikaz sadržaja u rezultatima pretraživanja. Slijedite korake u članku [Prikaz sadržaja na web-mjestu u rezultatima pretraživanja](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).

2. Provjerite je li **popis** ili **Biblioteka** koja sadrži očekivani sadržaj postavljena tako da omogućuje prikaz sadržaja u rezultatima pretraživanja. Slijedite korake u odjeljku [Prikaz sadržaja s popisa ili biblioteka u rezultatima pretraživanja](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).

3. Provjerite je li stranica, dokument ili prilagođeni prikaz stranice objavljen kao **glavna verzija.** Slijedeći korak 3 u [pretraživanju ne vraća sve rezultate u sustavu SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).

4. Provjerite ima li korisnik **dozvolu** za prikaz sadržaja. Slijedite korake u članku [razumijevanje razina dozvola u sustavu SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
    
5. Ako je shema pretraživanja izmijenjena dodavanjem novog upravljanog svojstva uređivanjem upravljanog svojstva ili uklanjanjem upravljanog svojstva, zatražiće se mogućnost pretraživanja radi indeksiranja i ponovnog indeksa. **Ponovno Indeksirajte** sadržaj slijedeći korake u odjeljku [ručno zahtjev za indeksiranje i ponovnim indeksiranjem web-mjesta, biblioteke ili popisa](https://docs.microsoft.com/sharepoint/crawl-site-content). To bi moglo potrajati, čekati 24 sata prije nego što ponovno provjerite rezultate.

Dodatne informacije potražite u članku [Omogućivanje pretraživanja sadržaja na web-mjestu](https://docs.microsoft.com/sharepoint/make-site-content-searchable). 
  
