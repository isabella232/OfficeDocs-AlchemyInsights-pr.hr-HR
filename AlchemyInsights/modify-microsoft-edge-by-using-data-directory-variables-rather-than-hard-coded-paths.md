---
title: Izmjena Microsoftova ruba pomoću varijabli podatkovnog direktorija, a ne tvrdih puteva
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8222"
- "9004596"
ms.openlocfilehash: 23ce69157c465c56d0fc5ada7c2c159e3192fd75
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035013"
---
# <a name="modify-microsoft-edge-by-using-data-directory-variables-rather-than-hard-coded-paths"></a>Izmjena Microsoftova ruba pomoću varijabli podatkovnog direktorija, a ne tvrdih puteva

Da biste, primjerice, u sustavu Windows pohranili podatke o profilu u odjeljku korisnika lokalnih aplikacija, a ne na zadanom mjestu, postavite pravilnik *Userdatadir* na **$ {local_app_data} \Edge\Profile**.

Dodatne informacije potražite u članku [Stvaranje varijabli Microsoftovih podatkovnih direktorija](https://docs.microsoft.com/deployedge/microsoft-edge-policies)u pregledniku.