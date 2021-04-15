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
ms.openlocfilehash: eebfb7cea7ae97921bf3c3667818400a17b5e52e
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51786841"
---
# <a name="suggestions-for-solving-unlicensed-product-errors"></a>Prijedlozi za rješavanje pogrešaka "Nelicencirani proizvod"

Da biste riješili pogreške o "nelicenciranom proizvodu", pokušajte sljedeće:

- Provjerite je li status pretplate istekao.
- Provjerite imate li pretplatu koja omogućuje klijentske licence, kao što su Aplikacije Microsoft 365 za tvrtke ili Business Premium, te provjerite je li korisniku [dodijeljena licenca](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users). 
- Provjerite prijavljuje li se korisnik u Office pomoću istog računa koji ima dodijeljenu licencu.
- Na [stranici Stanje servisa](https://docs.microsoft.com/office365/enterprise/view-service-health) provjerite postoje li neki poznati problemi sa servisom.
- Provjerite postavke vatrozida, antivirusnog softvera i proxyja da biste provjerili ne blokiraju li aplikacije Microsoft 365 pristup internetu. Pogledajte [URL-ove i raspone IP adresa](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

Možete isprobati i sljedeće akcije otklanjanja poteškoća: 

- Otvorite aplikaciju sustava Office i [odjavite se](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) iz postojećih korisničkih računa. [Uklonite](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) i [ponovno dodijelite licencu](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) za Office, a zatim [se prijavite u Office pomoću](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) zahvaćenog korisničkog računa.
- Pokrenite alat [za otklanjanje poteškoća s aktivacijom](https://aka.ms/SARA-OfficeActivation-Alchemy).
- [Ponovno postavite stanje aktivacije sustava Office](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state). 
- [Izvođenje mrežnog popravka sustava Office](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b).

Dodatne rješenja za otklanjanje poteškoća potražite u sljedećim člancima: 

- [Pogreške zbog nelicenciranog proizvoda i pogreške s aktivacijom u sustavu Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)
- [Pogreška „Nažalost, ne možemo se povezati s vašim računom. Pokušajte ponovo kasnije” prilikom aktivacije sustava Office](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)