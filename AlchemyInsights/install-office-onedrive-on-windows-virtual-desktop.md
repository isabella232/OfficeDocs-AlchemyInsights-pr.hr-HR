---
title: Instalacija Office i OneDrive na Windows virtualnu radnu površinu
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
ms.openlocfilehash: 226bd24a955f6165969102c8cf00cf45da537ee05a5363c74f1dfd055d922e1d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028608"
---
# <a name="install-office-and-onedrive-on-windows-virtual-desktop"></a>Instalacija Office i OneDrive na Windows virtualnu radnu površinu

1. [Priprema i prilagodba glavne VHD slike](https://docs.microsoft.com/azure/virtual-desktop/set-up-customize-master-image). Stvorite virtualno računalo (VIRTUALNO računalo) ako još nije stvoreno.

1. [Instalirajte Office načinu aktivacije zajedničkog računala](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-office-in-shared-computer-activation-mode). Aktivacija zajedničkog računala omogućuje više korisnika pristup Office.

1. [Instalacija OneDrive u načinu rada po stroju](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-onedrive-in-per-machine-mode). Obično se OneDrive instalira po korisniku, ali ovdje je potrebno instalirati po računalu.