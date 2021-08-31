---
title: Problemi prilikom prijave u Microsoft 365 aplikacije
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
- "9000571"
- "2574"
ms.openlocfilehash: f8f2824cc4a575ab7d7c9adec5b75e5955ec9fb5
ms.sourcegitcommit: b6dd6ae628a02ea6b997a993c49de083465bc2ac
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/30/2021
ms.locfileid: "58744628"
---
# <a name="issues-signing-into-microsoft-365-apps"></a>Problemi prilikom prijave u Microsoft 365 Apps

Napomena: ako koristite stariju verziju sustava Windows (npr. Windows 7 SP1, Windows Server 2008 R2), kao [](https://download.microsoft.com/download/0/6/5/0658B1A7-6D2E-474F-BC2C-D69E5B9E9A68/MicrosoftEasyFix51044.msi) zadano omogućite TLS 1.2 pomoću jednostavnog popravka. Dodatne informacije potražite u članku Ažuriranje radi omogućivanja [TLS 1.1 i TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)kao zadanih sigurnih protokola u aplikaciji WinHTTP u Windows .

Da biste riješili probleme s prijavama Microsoft 365 aplikacijama, isprobajte sljedeće mogućnosti na zahvaćenom uređaju:  

- Dodatne Windows, Preporuke [o rješavanju uobičajenih](https://docs.microsoft.com/office365/troubleshoot/administration/disabling-adal-wam-not-recommended#recommendations-on-resolving-common-sign-in-issues) problema s prijavi
- Za Mac pogledajte ne [mogu se prijaviti u aplikaciju Office 2016 za Mac](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail)

**Savjet** Na Windows uređajima možemo dijagnosticirati i automatski riješiti nekoliko uobičajenih Office problema prilikom prijave. Preuzmite i pokrenite **[Microsoftovu pomoćnik za podršku i oporavak da](https://aka.ms/SaRA-OfficeSignInScenario)** biste koristili naš automatizirani alat.

**Napomena:** Ne preporučuje se onemogućiti modernu provjeru autentičnosti (ADAL) ili upravljanje web-računom (WAM) radi rješavanja problema prilikom prijave **ili aktivacije.** Ako se prilikom povezivanja s Microsoft 365 2013 Office 2013 pojave pogreške, provjerite omogućujete li modernu provjeru [autentičnosti](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication) za Office klijenta.

Za određene akcije otklanjanja poteškoća pogledajte sljedeće:

[Problemi s povezivanjem prilikom prijave nakon ažuriranja za Office međuverziju 2016 16.0.7967 na Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)  

[Ne možete se prijaviti na račun tvrtke ili ustanove kao što su Office 365, Azure ili Intune](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)

[Otklanjanje poteškoća s aplikacijama koje nisu u pregledniku koje se ne mogu prijaviti u Office 365, Azure ili Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1?ui=en-US&rs=en-US&ad=US)

[U programu Office](https://docs.microsoft.com/office365/troubleshoot/authentication/access-denied-when-connect-to-office-365)