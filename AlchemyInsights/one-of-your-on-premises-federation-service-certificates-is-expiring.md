---
title: Jedan od vaših lokalnih certifikata federacijske službe istječe
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 172084b7-68a1-42a5-944d-2e871eaa2972
ms.openlocfilehash: dafa344ec649002900e98a5e183b3e5f759707e1
ms.sourcegitcommit: 6a3748f5c05693ca0c19a829287cb8f30635940c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43785295"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a>Jedan od vaših lokalnih certifikata federacijske službe istječe

Da biste riješili taj problem, slijedite ove korake:
  
- Instalirajte Modul servisa Microsoft Azure Active Directory za Windows PowerShell na računalu (ako modul već nije instaliran). Da biste to učinili, idite na [Azure Active Directory PowerShell za Graph](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)
    
- Slijedite korake u odjeljku "Scenarij 1: Certifikat za potpisivanje tokena AD FS istekao" pogreške "Došlo je do [problema s pristupom web-mjestu" iz AD FS-a kada se vanjski korisnik prijavi u Microsoft 365, Azure ili Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).
    
- Slijedite korake u [odjeljku Ažuriranje ili popravak postavki vanjske domene u sustavima Microsoft 365, Azure ili Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).
    
Dodatne informacije o obnavljanju certifikata federacije potražite u članku [Obnavljanje certifikata za O365 i Azure AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
  

