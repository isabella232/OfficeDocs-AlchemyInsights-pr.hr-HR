---
title: Promjena kanala za ažuriranje aplikacija sustava Office
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1740"
- "9000140"
ms.openlocfilehash: 4939682a6ca95c4f5475ee6aedea48c9ce83df7f
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 07/28/2020
ms.locfileid: "45438854"
---
# <a name="change-update-channels-for-office-apps"></a>Promjena kanala za ažuriranje aplikacija sustava Office

Za nove instalacije sustava Office pomoću postavki preuzimanja softvera sustava Office odaberite željeni kanal za ažuriranje, a zatim instalirajte (ili ponovno instalirajte) aplikacije sustava Office. Dodatne informacije [potražite u odjeljku Upravljanje postavkama preuzimanja softvera u sustavu Office 365](https://docs.microsoft.com/deployoffice/manage-software-download-settings-office-365). 

**Napomena:** Kanal za ažuriranje odabran pomoću postavki preuzimanja softvera sustava Office primjenjuje se na sve korisnike koji izvode nove instalacije pomoću portala sustava O365. Dodatne informacije potražite [u odjeljku Preuzimanje i instalacija ili ponovna instalacija sustava Microsoft 365 ili Office 2019 na PC ili Mac](https://support.microsoft.com/office/download-and-install-or-reinstall-microsoft-365-or-office-2019-on-a-pc-or-mac-4414eaaf-0478-48be-9c42-23adc4716658).   

Za postojeće instalacije sustava Office pomoću alata za implementaciju sustava Office (ODT) prijeđite na drugi kanal ažuriranja:  

1. Preuzmite najnoviju verziju alata za implementaciju sustava Office (setup.exe) iz [Microsoftova centra za preuzimanje](https://go.microsoft.com/fwlink/p/?LinkID=626065).
2. Odredite naziv kanala na koji želite prijeći. Dodatne informacije [potražite u odjeljku Mogućnosti konfiguracije alata za implementaciju sustava Office](https://docs.microsoft.com/DeployOffice/configuration-options-for-the-office-2016-deployment-tool#channel-attribute-part-of-add-element).
3. Stvorite konfiguracijsku XML datoteku koja određuje odgovarajući naziv kanala, na primjer, update.xml.  
    A. <Configuration>  
    B. <Updates **Channel="Mjesečno"** />  
    C. </Configuration>
4. From visok naredba brz, šiba to savijač položaj gdje svi setup.exe stanovati i trčanje slijedeće naredba:  
    A. setup.exe /konfiguriraj update.xml
5. Pokrenite aplikaciju sustava Office (kao što je Excel), a zatim odaberite **Račun**  >  **datoteke**. U odjeljku Informacije o proizvodu odaberite **Ažuriraj mogućnosti**  >  **Ažuriraj odmah**.

Dodatne informacije [potražite u odjeljku Promjena kanala ažuriranja za postojeće aplikacije sustava Office](https://support.microsoft.com/help/3185078/how-to-switch-from-semi-annual-channel-to-monthly-channel). 

Za prebacivanje kanala ažuriranja za odabranu grupu korisnika ili pomoću Upravitelj konfiguracije (SCCM), konfigurirajte postavku Ažuriraj kanal pomoću GPO-a. Dodatne informacije [potražite u odjeljku Pregled kanala ažuriranja za Aplikacije microsoft 365](https://docs.microsoft.com/deployoffice/overview-update-channels#group-policy). Pojedinosti potražite [u članku Upravljanje kanalima sustava Office 365 ProPlus za IT profesionalce](https://techcommunity.microsoft.com/t5/office-365-blog/how-to-manage-office-365-proplus-channels-for-it-pros/ba-p/795813) i upravljanje [ažuriranjima aplikacija microsoft 365 pomoću programa Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-microsoft-365-apps-updates-configuration-manager).