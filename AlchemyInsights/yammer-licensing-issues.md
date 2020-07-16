---
title: Problemi s licenciranjem servisa Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5900"
- "9003071"
ms.openlocfilehash: 6d9b2126dc1ed90968738ddb2e249dce9857f1db
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148180"
---
# <a name="yammer-licensing-issues"></a>Problemi s licenciranjem servisa Yammer

Svi korisnici moraju imati licencu za korištenje servisa Yammer Enterprise, ali na zadanom servis Yammer ne zahtijeva da korisnici imaju licencu za pristup servisu. Kada administrator promijeni postavku da blokira korisnike sustava Microsoft 365 bez licenci servisa Yammer, korisnicima koji nisu dodijeljeni licenci za Yammer Enterprise ne mogu pristupiti servisu servisa Yammer. Dodatne informacije [potražite u članku Upravljanje korisničkim licencama servisa Yammer u sustavu Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365) 

Kada se licence uklanjaju iz korisnika, pločica servisa Yammer više se ne prikazuje, a drugi servisi mogu koristiti uklanjanje licenci da bi sakrili značajke. U drugim slučajevima značajke se i dalje mogu pojaviti, ali zahtijevaju da dodjela dozvola radi.  

**Licenca se ne ažurira za korisnika**  

Korisniku se povremeno dodjeljuje licenca, ali i dalje ne može pristupiti servisu Yammer. Veća je vjerojatnost da će doći do kašnjenja kada je dodjela masovne licence u tijeku. Korisnici servisa Yammer možda se neće ažurirati istim redoslijedom kao i licence u azure AD jer sustav izvodi asinkrono. Pričekajte do 24 sata prije otvaranja slučaja podrške da biste prijavili probleme sa sinkronizacijom licence.  

**Dodjela skupne dozvole**  

Licence se mogu dodijeliti putem centra za administratore ili skriptiranja u powershellu. Dodatne informacije potražite u članku [Dodjela licenci korisnicima](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) i [Dodjela licenci korisničkim računima pomoću komponente Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell). 

Microsoftova podrška ne pruža pomoć pri stvaranju skripti, ali dostupna je dokumentacija o dodjeli licence za Yammer. Dodatne informacije [potražite u odjeljku Upravljanje licencama za Yammer pomoću komponente Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).