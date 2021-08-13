---
title: Na portalu nema uređaja iz programa Configuration Manager
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
- "9001495"
- "4384"
ms.openlocfilehash: 358bb6aa0420a845e51e0b75049c2ae790daf3690e5cfb115b234d82a29e93a7
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53966101"
---
# <a name="configuration-manager-devices-missing-in-the-portal"></a>Na portalu nema uređaja iz programa Configuration Manager

Da bi sinkronizacija uređaja funkcionirala, [potrebne internetske krajnje točke](https://docs.microsoft.com/configmgr/tenant-attach/device-sync-actions#internet-endpoints) moraju biti dostupne s lokalnog poslužitelja na kojem se hostira uloga točke povezivanja servisa. Da biste otklonili poteškoće sa sinkronizacijom uređaja, pregledajte **CMGatewaySyncUploadWorker.log** u točki povezivanja servisa.

Saznajte više o [pridruživanju klijenata u programu Microsoft Endpoint Manager](https://docs.microsoft.com/configmgr/tenant-attach/).
