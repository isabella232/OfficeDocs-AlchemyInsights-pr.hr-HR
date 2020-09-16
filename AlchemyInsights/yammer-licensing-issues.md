---
title: Problemi s licenciranjem servisa Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5900"
- "9003071"
ms.openlocfilehash: f0a7625c7b77860e5ba0e29f2df47101749aace3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47657268"
---
# <a name="yammer-licensing-issues"></a>Problemi s licenciranjem servisa Yammer

Svi korisnici moraju imati licencu za korištenje servisa Yammer Enterprise, ali po zadanom Yammer ne zahtijeva da korisnici imaju licencu za pristup servisu. Kada administrator promijeni postavku da bi blokirao korisnike tvrtke Microsoft 365 bez licenci za Yammer, korisnici koji nisu dodijelili licencu za Yammer Enterprise ne mogu pristupiti servisu Yammer. Dodatne informacije potražite u članku [Upravljanje korisničkim dozvolama za Yammer u sustavu Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365) 

Kada se licence uklanjaju od korisnika, pločica servisa Yammer više se ne prikazuje, a drugi servisi mogu koristiti licencu za uklanjanje za sakrivanje značajki. U drugim slučajevima značajke se i dalje mogu prikazivati, no potrebna je dodjela licenci za rad.  

**Licenca nije ažurirana za korisnika**  

Korisniku se povremeno dodjeljuje licenca, ali i dalje ne može pristupiti servisu Yammer. Veća je vjerojatnost da će kašnjenja nastati kada je u tijeku dodjela licence za masovnu licencu. Korisnici servisa Yammer možda se neće ažurirati istim redoslijedom kada se licence promijene u servisu Azure AD jer sustav radi asinkrono. Pričekajte do 24 sata prije otvaranja slučaja podrške da biste prijavili probleme s sinkronizacijom licenci.  

**Dodjela skupnih dozvola**  

Licence se mogu dodijeliti putem centra za administratore ili skripte za PowerShell. Dodatne informacije potražite u članku [dodjeljivanje licenci korisnicima](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) i [dodjeljivanje licenci korisničkim računima pomoću komponente Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell). 

Microsoftova podrška ne nudi pomoć za stvaranje skripti, ali je dostupna dokumentacija na dodjeli licenci za Yammer. Dodatne informacije potražite u članku [Upravljanje licencama servisa Yammer pomoću komponente Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).