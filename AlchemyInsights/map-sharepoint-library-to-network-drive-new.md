---
title: Mapiranje biblioteke SharePoint na mrežni pogon
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 4b8245c3-a179-4524-ae83-0c22d539c202
ms.openlocfilehash: 4eae45992d3fe6b31ae4d1aed02484cf20cb2260
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58315540"
---
# <a name="map-a-sharepoint-library-to-a-network-drive"></a>Mapiranje biblioteke SharePoint na mrežni pogon

Umjesto mapiranja mrežnog pogona sinkronizirajte SharePoint datoteka s novim Sinkronizacija sa servisom OneDrive, koji nudi datoteke na zahtjev. Pristupajte svim svojim datotekama u sustavu OneDrive bez upotrebe lokalnog prostora za pohranu. Dodatne informacije potražite u članku [Sinkronizacija SharePoint i Teams datoteka](https://support.microsoft.com/office/sync-sharepoint-and-teams-files-with-your-computer-6de9ede8-5b6e-4503-80b2-6190f3354a88) s računalom i Spremanje prostora na disku OneDrive datoteka na zahtjev za [Windows 10](https://support.microsoft.com/office/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e).

Ako odaberete mapiranje pogona umjesto korištenja novog [klijenta Sinkronizacija sa servisom OneDrive,](https://support.microsoft.com/office/sync-sharepoint-and-teams-files-with-your-computer-6de9ede8-5b6e-4503-80b2-6190f3354a88)slijedite ove korake:

- [Otklanjanje poteškoća s mapiranim mrežnim pogonima koji se povezuju na sustav SharePoint Online](https://docs.microsoft.com/sharepoint/support/administration/troubleshoot-mapped-network-drives)

- [Pogreške provjere autentičnosti pojavljuju se kada klijent nema podršku za TLS 1.2](https://docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support#network-drive-mapped-to-a-sharepoint-library)  

**NAPOMENA:** Ako koristite Internet Explorer 10 s Windows 8 ili Windows 7, a access **denied** ili **Path** nije dostupan prilikom mapiranja pogona, riješite taj problem instalacijom tog hitnog [popravka](https://support.microsoft.com/topic/error-when-you-open-a-sharepoint-document-library-in-windows-explorer-or-map-a-network-drive-to-the-library-after-you-install-internet-explorer-10-96e640ba-059f-9b09-bb91-2a0319ee8b1d).