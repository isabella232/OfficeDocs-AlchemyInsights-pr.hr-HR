---
title: Potvrda Saveza za ADFS
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: a3172bc402a22999a3bf963233cc26db1ddf2a03
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47686706"
---
# <a name="adfs-federation-certificate-expiring"></a>Potvrda Saveza za ADFS

Da biste riješili taj problem, slijedite ove korake:
  
1. Instalirajte modul Microsoft Azure Active Directory za Windows PowerShell na računalu (ako modul već nije instaliran). Da biste to učinili, idite na [Upravljanje programom Azure ad pomoću komponente Windows PowerShell](https://aka.ms/aadposh).

2. Slijedite korake u odjeljku "scenarij 1: certifikat za potpisivanje tokena za AD FS istekao je" u odjeljku ["došlo je do problema prilikom pristupanja web-mjestu" u APLIKACIJI AD FS kada se združeni korisnik prijavljuje u Microsoft 365, Azure ili Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).

3. Slijedite korake u [članku ažuriranje ili popravak postavki udruženu domene u programu Microsoft, Azure ili Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).

    Dodatne informacije o obnavljanju certifikata Federacije potražite u članku [obnavljanje certifikata Federacije za Microsoft 365 i Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
