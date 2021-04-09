---
title: Rješavanje 0x8004de40 pogreške na servisu OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 0edb3e19b5dea240c9f2846dc503e65d92113cb7
ms.sourcegitcommit: 477cce131dc4a3c212ab18a8763a50b2f3bb20b1
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/09/2021
ms.locfileid: "51649740"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>Rješavanje 0x8004de40 pogreške na servisu OneDrive

Ako koristite Windows 7 i primite tu pogrešku, ažuriranje da biste [omogućili TLS 1.1 i TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)kao zadane sigurne protokole u sustavu WinHTTP u sustavu Windows .

Ako koristite Windows 10 i prikazuje vam se pogreška 0x8004de40 onedrive:

- Ponovno pokrenite zahvaćeno računalo dok ste povezani s domenom Acitve Directory.
- Ako se problem ne riješi ponovnim pokretanjem, ponovno se pridružite uređaju pomoću servisa Azure AD. 

**Napomena:** tijekom izvođenja ovih koraka trebali biste biti na mreži tvrtke. Nemojte izvoditi ove korake kada niste povezani s korporativnom infrastrukturom (primjerice, tijekom putovanja). 

1. Otvorite povišen naredbeni redak tako da odaberete **Start**, desnom tipkom miša kliknite **Naredbeni redak**, a zatim **odaberite Pokreni kao administrator**.

1. Upišite *dsregcmd /leave pa* pritisnite **Enter**.

1. Kada završite, upišite *dsregcmd /join i* pritisnite **Enter**.

1. Kada završite, zatvorite naredbeni redak.

1. Ponovno pokrenite računalo i prijavite se na OneDrive.