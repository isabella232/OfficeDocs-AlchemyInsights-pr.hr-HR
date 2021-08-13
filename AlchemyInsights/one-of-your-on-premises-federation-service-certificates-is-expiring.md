---
title: Jedan od vaših lokalnog certifikata o servisu za Federation istječe
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 172084b7-68a1-42a5-944d-2e871eaa2972
ms.openlocfilehash: d0658b05b81ac45e7ce80323ad29898599482c4d3430d886627af6e9f8d136f6
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53985209"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a>Jedan od vaših lokalnog certifikata o servisu za Federation istječe

Da biste riješili taj problem, slijedite ove korake:
  
- Instalirajte modul Microsoft Azure Active Directory za Windows PowerShell na računalo (ako modul još nije instaliran). Da biste to Azure Active Directory [powershell Graph](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)
    
- Slijedite korake u odjeljku "Scenarij 1: certifikat za potpisivanje tokena za AD FS istekao" u odjeljku "Došlo je do problema prilikom pristupa web-mjestu" iz AD FS-a kada se vanjski korisnik prijavi [u Microsoft 365, Azure ili Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).
    
- Slijedite korake u odjeljku Ažuriranje ili popravak postavki vanjske domene na [servisu Microsoft 365, Azure ili Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).
    
Dodatne informacije o obnovi certifikata za Federation potražite u članku [Obnavljanje certifikata za O365 i Azure AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
  

