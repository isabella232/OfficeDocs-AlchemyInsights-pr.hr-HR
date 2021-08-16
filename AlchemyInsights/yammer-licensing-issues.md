---
title: Yammer problema s licenciranjem
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
ms.openlocfilehash: 3ec764ece9cb7be933e9e2cd002379898522790528b0fa586ab501424b00cd7b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53989721"
---
# <a name="yammer-licensing-issues"></a>Yammer problema s licenciranjem

Svi korisnici moraju imati licencu za korištenje servisa Yammer Enterprise, ali po zadanom Yammer ne zahtijeva da korisnici imaju licencu za pristup servisu. Kada administrator promijeni postavku tako da Microsoft 365 korisnike bez Yammer licenci, korisnici koji nisu dodijelili licencu za Yammer Enterprise ne mogu pristupiti servisu Yammer. Dodatne informacije potražite u članku [Upravljanje korisničkim Yammer licencama u sustavu Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365) 

Kada se licence uklone s korisnika, Yammer se više ne prikazuje, a drugi servisi mogu koristiti uklanjanje licenci da bi sakrili značajke. U drugim se slučajevima značajke i dalje mogu prikazivati, ali za rad je potreban dodjela licence.  

**Licenca se ne ažurira za korisnika**  

Korisniku se povremeno dodjeljuje licenca, ali i dalje ne može pristupiti Yammer. Kašnjenja će se vjerojatno pojaviti kada je u tijeku dodjela masovne licence. Yammer se korisnici možda neće ažurirati istim redoslijedom kao licence u sustavu Azure AD jer se sustav pokreće asinkrono. Pričekajte do 24 sata prije otvaranja slučaja podrške da biste prijavili probleme sa sinkronizacijom licenci.  

**Dodjela masovne licence**  

Licence se mogu dodijeliti putem centra za administratore ili skripte komponente PowerShell. Dodatne informacije potražite u članku [Dodjela licenci korisnicima i](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) [Dodjela licenci korisničkim računima Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell). 

Microsoftova podrška ne pruža pomoć pri stvaranju skripti, ali je dostupna Yammer o dodjeli licenci. Dodatne informacije potražite u članku [Upravljanje Yammer licencama pomoću Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).