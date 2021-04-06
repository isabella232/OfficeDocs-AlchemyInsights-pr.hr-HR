---
title: Prepoznavanje problema s virtualnom radnom površinom sustava Windows
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O364
ms.custom:
- "9004219"
- "10871"
ms.openlocfilehash: 1e55d9d579c389dfe731f887a2a08c6234de2787
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/05/2021
ms.locfileid: "51595513"
---
# <a name="identify-windows-virtual-desktop-issues"></a>Prepoznavanje problema s virtualnom radnom površinom sustava Windows

Dijagnostika virtualne radne površine sustava Windows koristi samo jedan cmdlet komponente PowerShell, ali sadrži brojne neobavezne parametre za sužavanje i izoliranje problema. Da biste započeli s radom: 

1. Preuzmite i uvezite modul Windows Virtual Desktop PowerShell. Detalje potražite u članku [Cmdleti virtualne radne površine sustava Windows za Windows PowerShell](https://docs.microsoft.com/powershell/windows-virtual-desktop/overview).

1. Pokrenite sljedeći cmdlet da biste se prijavili na račun:
    
    Primjer: `Add-RdsAccount -DeploymentUrl 'https://rdbroker.wvd.microsoft.com'`

**NAPOMENA:** Svi upiti koji koriste PowerShell moraju obuhvaćati parametre -UserName ili -ActivityID. Mogućnosti nadzora pogledajte u članku Korištenje [analitike zapisnika za značajku dijagnostike](https://go.microsoft.com/fwlink/?linkid=2126847).

Da biste filtrirali dijagnostičke aktivnosti po korisniku, pokrenite sljedeći cmdlet:

Primjer: `Get-RdsDiagnosticActivities -TenantName < tenantName > -UserName < UserUPN >`

Postoji popis filtara koje možete pokrenuti da biste dijagnosticirali probleme. Dodatne informacije o dijagnosticiranju problema potražite u članku Prepoznavanje i dijagnosticiranje problema s virtualnom radnom [površinom sustava Windows](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell).

Dodatne informacije o najčešćim pogreškama potražite u članku [Uobičajene pogreške senarios](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#common-error-scenarios).
