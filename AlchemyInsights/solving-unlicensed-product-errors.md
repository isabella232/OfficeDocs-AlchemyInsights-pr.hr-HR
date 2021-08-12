---
title: Rješavanje pogrešaka nelicencirani proizvod
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
- "3412"
- "9001428"
ms.openlocfilehash: 7922a2c5306f9d16856502b5e57e585cb90f2f7c9abaad0366f72ed46de786d5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53957092"
---
# <a name="suggestions-for-solving-unlicensed-product-errors"></a>Prijedlozi za rješavanje pogrešaka "Nelicencirani proizvod"

Da biste riješili pogreške o "nelicenciranom proizvodu", pokušajte sljedeće:

- Provjerite je li status pretplate istekao.
- Provjerite imate li pretplatu koja omogućuje klijentske licence, kao što su Microsoft 365 Apps za male tvrtke ili Business premium, te provjerite je li [korisniku dodijeljena licenca](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users). 
- Provjerite prijavljuje li se korisnik na Office s istim računom koji ima dodijeljenu licencu.
- Na [stranici Stanje servisa](https://docs.microsoft.com/office365/enterprise/view-service-health) provjerite postoje li neki poznati problemi sa servisom.
- Provjerite postavke vatrozida, antivirusnog softvera i proxyja da biste provjerili ne blokiraju li Microsoft 365 aplikacijama pristup internetu. Pogledajte [URL-ove i raspone IP adresa](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

Možete isprobati i sljedeće akcije otklanjanja poteškoća: 

- Otvorite aplikacija Office i [odjavite se](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) iz postojećih korisničkih računa. [Uklonite](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) i [ponovno dodijelite](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) licencu Office, a zatim se [prijavite u Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) pomoću zahvaćenog korisničkog računa.
- Pokrenite alat [za otklanjanje poteškoća s aktivacijom](https://aka.ms/SARA-OfficeActivation-Alchemy).
- [Ponovno postavite stanje Office aktivacije .](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state) 
- [Izvođenje mrežnog popravka Office](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b).

Dodatne rješenja za otklanjanje poteškoća potražite u sljedećim člancima: 

- [Pogreške zbog nelicenciranog proizvoda i pogreške s aktivacijom u sustavu Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)
- [Pogreška „Nažalost, ne možemo se povezati s vašim računom. Pokušajte ponovo kasnije” prilikom aktivacije sustava Office](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)