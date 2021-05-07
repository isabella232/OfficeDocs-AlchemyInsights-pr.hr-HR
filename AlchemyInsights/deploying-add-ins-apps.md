---
title: Implementacija dodataka za Microsoft 365 Apps
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/30/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "11107"
- "9005477"
ms.openlocfilehash: a878a35ba9b530ce22ca7c263d20bd942d6896a8
ms.sourcegitcommit: 6c6b0c3885f33b08db929fe0b6496508d31fa2d6
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52233509"
---
# <a name="deploying-add-ins-for-microsoft-365-apps"></a>Implementacija dodataka za Microsoft 365 Apps

Centralizirana implementacija preporučeni je način implementacije Office dodataka korisnicima i grupama u tvrtki ili ustanovi. Da biste implementirati dodatke, slijedite korake u nastavku:

**Napomena:** Da biste instalirali dodatke za Office kao pojedinačnog korisnika, pogledajte prikaz dodataka, upravljanje njima i [instalaciju Office programima](https://support.microsoft.com/topic/view-manage-and-install-add-ins-in-office-programs-16278816-1948-4028-91e5-76dca5380f8d). Osim toga, provjerite je li omogućeno Office pojedinačnih dodataka trgovine Store. Detalje potražite u članku Sprječavanje preuzimanja dodataka tako da isključite Office trgovine u svim [klijentima (osim Outlook).](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center?view=o365-worldwide#prevent-add-in-downloads-by-turning-off-the-office-store-across-all-clients-except-outlook)

1. Provjerite ispunjava li vaše okruženje preduvjete za implementaciju dodataka pomoću centralizirane implementacije. Detalje potražite u odjeljku [Preduvjeti](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?#requirements).
2. Idite **na Postavke**  >  **integrirane**  >  **aplikacije Nabavite aplikacije** u centru Microsoft 365 za administratore da biste implementirani dodatke. 

Napomene: 

- Integrirane aplikacije zahtijevaju da administrator ima dozvole globalnog administratora Exchange administratora.

- Prilikom implementacije dodataka na više korisnika preporučujemo da zadatke postavite pomoću grupa umjesto pojedinačnih korisnika. Detalje potražite u [članku Razmatranja prilikom dodjele dodatka korisnicima i grupama](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins?view=o365-worldwide#considerations-when-assigning-an-add-in-to-users-and-groups).

- Centralizirana implementacija ne podržava korisnike u ugniježđenim grupama ili grupama koje imaju nadređene grupe. Detalje potražite u članku [Korisnički i grupni zadaci](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?view=o365-worldwide#user-and-group-assignments).

- Provjerite je li Microsoft 365 servis za upravljanje aplikacijama (GUID: '0517ffae-825d-4aff-999e-3f2336b8a20a') omogućen za prijavu. Detalje potražite u članku [Konfiguriranje svojstava aplikacije](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure#configure-app-properties).

- Ako se pojave problemi prilikom implementacije dodataka pomoću integriranih aplikacija, pokušajte implementirati pomoću [dodataka](https://admin.microsoft.com/AdminPortal/Home?#/Settings/AddIns).

Dodatne informacije potražite u sljedećim člancima:

[Implementacija dodataka u centru za administratore](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins) 
 [Upravljanje dodacima u centru za administratore](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center) 
 [Upravljanje dodacima pomoću cmdleta komponente PowerShell za centraliziranu implementaciju](https://docs.microsoft.com/microsoft-365/enterprise/use-the-centralized-deployment-powershell-cmdlets-to-manage-add-ins) 
 [Objavljivanje Office dodataka pomoću centralizirane implementacije putem centra za Microsoft 365 administratore](https://docs.microsoft.com/office/dev/add-ins/publish/centralized-deployment#publish-an-office-add-in-via-centralized-deployment) 
 [Otklanjanje poteškoća: korisnik ne vidi dodatke](https://docs.microsoft.com/office365/troubleshoot/access-management/user-not-seeing-add-ins) 
 [Otklanjanje poteškoća s Office dodacima](https://docs.microsoft.com/office/dev/add-ins/testing/testing-and-troubleshooting)