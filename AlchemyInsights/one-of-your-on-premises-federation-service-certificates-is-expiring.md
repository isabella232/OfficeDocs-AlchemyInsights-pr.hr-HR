---
title: Jedan od lokalnih certifikata servisa za Federaciju istječe
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
ms.custom: ''
ms.assetid: 172084b7-68a1-42a5-944d-2e871eaa2972
ms.openlocfilehash: a4c78f3fdbba7786785f31098c9e80e77a165623
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47673489"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a>Jedan od lokalnih certifikata servisa za Federaciju istječe

Da biste riješili taj problem, slijedite ove korake:
  
- Instalirajte modul Microsoft Azure Active Directory za Windows PowerShell na računalu (ako modul već nije instaliran). Da biste to učinili, otvorite odjeljak [Azure Active Directory PowerShell za Graph ](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)
    
- Slijedite korake u odjeljku "scenarij 1: certifikat za potpisivanje tokena za AD FS istekao je" u odjeljku ["došlo je do problema prilikom pristupanja web-mjestu" u APLIKACIJI AD FS kada se združeni korisnik prijavljuje u Microsoft 365, Azure ili Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).
    
- Slijedite korake u [odjeljku Kako ažurirati ili popraviti postavke udruženu domene u programu Microsoft 365, Azure ili Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).
    
Dodatne informacije o obnavljanju certifikata Federacije potražite u članku [obnova certifikata za O365 i Azure ad](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
  

