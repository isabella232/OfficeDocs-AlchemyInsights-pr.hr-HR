---
title: Sakrivanje javnih mapa
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/18/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "8417"
ms.openlocfilehash: 70179296e9c1bb7391535f55796bc5af80b825f8
ms.sourcegitcommit: a019bd8b0244914edb59e124bc6538cdc5c158f9
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 02/18/2021
ms.locfileid: "50315321"
---
# <a name="hide-public-folders"></a>Sakrivanje javnih mapa

**Da biste skrivali cijelo stablo javne mape**:

Slijedite korake u [ovom](https://aka.ms/ControlPF) članku da biste skrivali cijeli prikaz stabla javnih mapa od selektivnog ili svih korisnika.

**Da biste skrivali određenu javnu mapu**, učinite sljedeće:

1. Dodavanje dozvola za korisnike kojima je potreban pristup javnoj mapi

    `Add-PublicFolderClientPermission \test1 -User cloud1 -AccessRights owner`

2. Uklanjanje **zadanog** korisnika s popisa **dozvola** :

    `Remove-PublicFolderClientPermission \test1 -User Default`
