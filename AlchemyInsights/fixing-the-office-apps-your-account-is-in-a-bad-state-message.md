---
title: Popravljanje aplikacija sustava Office Vaš račun nalazi se u poruci o lošem stanju
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2558"
- "9000571"
ms.openlocfilehash: e591c56dd207a5bcb3979be3f66052121100b162
ms.sourcegitcommit: 2572c4e5a981d5f3f556835061c568cfd08b78da
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 12/27/2019
ms.locfileid: "41969297"
---
# <a name="fixing-the-office-apps-your-account-is-in-a-bad-state-error"></a>Ispravljanje pogreške u vezi s aplikacijama sustava Office "Vaš račun je u lošem stanju"

Da biste riješili tu pogrešku, isprobajte sljedeće mogućnosti na zahvaćenom računalu:

- Otvorite aplikaciju sustava Office, odaberite Odjava**na račun** >  **datoteke** > **sa svih računa**. Ponovno se prijavite pomoću korisničkog računa s valjanom licencom. Detaljne informacije potražite [u odjeljku Računi u sustavu Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- [Izbrišite vjerodajnice sustava Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) pomoću upravitelja vjerodajnica sustava Windows.<br>
  **Napomena:** Putovi registra za Office 2016 promijenili su se u 16.0. Na primjer, \Software\Microsoft\Office\16.0\Common\Identity\
- Na zahvaćenom računalu postavite EnableADAL = 0 pomoću sljedećih koraka:  
     1. Desnom tipkom miša kliknite gumb Windows i odaberite **Pokreni**. U okvir **Otvori** upišite **regedit**, a zatim odaberite **U redu**.
     2. Odaberite **Da** kada se od vas zatraži da biste uređivaču registra dopustili izmjene uređaja.
    3. U uređivaču registra dodajte DWORD vrijednost EnableADAL s postavkom 0 pod HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.
- Ako dođe do pogreške tijekom povezivanja sa sustavom Office 365 pomoću sustava Office 2013, [omogućite modernu provjeru autentičnosti](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication) klijenta sustava Office.

Dodatne informacije potražite u [odjeljku Otklanjanje poteškoća s aplikacijama koje se ne mogu prijaviti u Office 365, Azure ili Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).

