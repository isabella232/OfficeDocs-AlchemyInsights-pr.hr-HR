---
title: Instalacija sustava Office i servisa OneDrive na virtualnoj radnoj površini sustava Windows
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9004219"
- "10871"
ms.openlocfilehash: fb38f46cced928e33e16e8e83ad740dd83aea622
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/05/2021
ms.locfileid: "51595510"
---
# <a name="install-office-and-onedrive-on-windows-virtual-desktop"></a>Instalacija sustava Office i servisa OneDrive na virtualnoj radnoj površini sustava Windows

1. [Priprema i prilagodba glavne VHD slike](https://docs.microsoft.com/azure/virtual-desktop/set-up-customize-master-image). Stvorite virtualno računalo (VIRTUALNO računalo) ako još nije stvoreno.

1. [Instalacija sustava Office u načinu aktivacije zajedničkog računala](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-office-in-shared-computer-activation-mode). Aktivacija zajedničkog računala omogućuje više korisnika pristup sustavu Office.

1. [Instalirajte OneDrive u načinu rada po stroju](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-onedrive-in-per-machine-mode). OneDrive se obično instalira po korisniku, ali ovdje je potrebno instalirati po računalu.