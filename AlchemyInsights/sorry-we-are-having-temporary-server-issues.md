---
title: Rješavanje Microsoft 365 aplikacija Nažalost, imamo poruku o privremenim problemima s poslužiteljem
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3420"
- "9001430"
ms.openlocfilehash: 565f70d9a09c61bef84cdd1c23e9b0ed34bebe51
ms.sourcegitcommit: b6dd6ae628a02ea6b997a993c49de083465bc2ac
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/30/2021
ms.locfileid: "58744638"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a>Rješavanje problema Microsoft 365 aplikacije "Nažalost, imamo privremene probleme s poslužiteljem"

Napomena: ako koristite stariju verziju sustava Windows (npr. Windows 7 SP1, Windows Server 2008 R2), [](https://download.microsoft.com/download/0/6/5/0658B1A7-6D2E-474F-BC2C-D69E5B9E9A68/MicrosoftEasyFix51044.msi) kao zadano omogućite TLS 1.2 jednostavan popravak. Dodatne informacije potražite u članku Ažuriranje radi omogućivanja [TLS 1.1 i TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)kao zadanih sigurnih protokola u aplikaciji WinHTTP Windows .

Ako primite ovu poruku, pokušajte sljedeće:

1. Provjerite postavke vatrozida, antivirusnog softvera i proxyja da biste potvrdili da ne blokiraju pristup internetu Microsoft 365 aplikacijama. Pogledajte [URL-ove i raspone IP adresa](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Idite na **Pokreni**  >  **pokreni**, a zatim upišite **services.msc**. Provjerite jesu li svi sljedeći servisi pokrenuti:
    - Automatsko postavljanje mrežnih uređaja
    - Servis za mrežni popis
    - Svijest o mrežnom mjestu
    - Windows Zapisnik događaja

Ako neki od tih servisa nije pokrenut, pokušajte ga pokrenuti. Ako imate problema s pokretanjem servisa, pokrenite sljedeću naredbu tako da otvorite naredbeni redak s dodatnim dozvolama:

**sfc /scannow**

Kada ova naredba završi, ponovno pokrenite računalo.

Detaljne informacije potražite u članku ["Nažalost, ne možemo se povezati s vašim računom. Kada aktivirate, pokušajte ponovno kasnije".](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)