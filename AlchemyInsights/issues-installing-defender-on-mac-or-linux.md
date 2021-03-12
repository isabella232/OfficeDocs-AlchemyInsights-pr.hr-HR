---
title: Problemi s instalacijom programa Microsoft Defender na računalu Mac ili Linux
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6028"
- "9001222"
ms.openlocfilehash: a8d5ad2246b9b83e1e0a4d5be4dd8bb41c16e734
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "50713316"
---
# <a name="issues-installing-microsoft-defender-on-mac-or-linux"></a>Problemi s instalacijom programa Microsoft Defender na računalu Mac ili Linux

**Mac**

- Provjerite jesu li sistemski preduvjeti ispunjeni prije instaliranja programa Microsoft Defender ATP za Mac. Dodatne informacije potražite u članku [Instalacija programa Microsoft Defender ATP za Mac](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-mac#how-to-install-microsoft-defender-atp-for-mac).  
- Pregledajte podatke u datoteci: "/Library/Logs/Microsoft/mdatp/install.log".

**Linux**

- Provjerite jesu li sistemski preduvjeti ispunjeni prije instaliranja programa Microsoft Defender ATP za Linux. Dodatne informacije potražite u članku [Instalacija programa Microsoft Defender ATP za Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements). 
- Da biste provjerili je li servis MDATP pokrenut, pročitajte članak [Instalacija nije uspjela](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#installation-failed).  
    Da biste otklonili poteškoće i riješili probleme ako servis nije pokrenut, pročitajte članak [koraci za otklanjanje poteškoća ako servis mdatp nije pokrenut](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#steps-to-troubleshoot-if-mdatp-service-isnt-running).
- Da biste provjerili konfiguraciju klijenta, koji provjerava zdravlje proizvoda i pokrenuli test otkrivanja u tekstnoj datoteci programa EICAR, pročitajte članak [Konfiguracija klijenta](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-install-manually#client-configuration).  

    **Notes** Popis podržanih datotečnih sustava za aktivnost u programu Access potražite u [članku Microsoft Defender ATP za Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements).