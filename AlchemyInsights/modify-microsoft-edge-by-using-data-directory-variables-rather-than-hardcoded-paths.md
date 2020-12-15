---
title: Izmjena Microsoftova ruba pomoću varijabli podatkovnog direktorija, a ne tvrdokornih puteva
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: ''
ms.custom:
- "9003873"
- "6926"
ms.openlocfilehash: 5c40aa1d7f61fbd2842839a5839899af8ab439f2
ms.sourcegitcommit: 523098560e54a50184a99c974809dfbfffadacb5
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 12/09/2020
ms.locfileid: "49677025"
---
# <a name="modify-microsoft-edge-by-using-data-directory-variables-rather-than-hardcoded-paths"></a>Izmjena Microsoftova ruba pomoću varijabli podatkovnog direktorija, a ne tvrdokornih puteva

Da biste, primjerice, u sustavu Windows pohranili podatke o profilu u odjeljku korisnika lokalnih aplikacija, a ne na zadanom mjestu, postavite pravilnik **Userdatadir** na **$ {local_app_data} \Edge\Profile**. 

Dodatne informacije potražite u članku [Stvaranje varijabli za Microsoft Edge korisnički podatkovni direktorij](https://docs.microsoft.com/deployedge/edge-learnmore-create-user-directory-vars).