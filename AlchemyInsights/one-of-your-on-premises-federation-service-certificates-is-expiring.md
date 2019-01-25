---
title: Jedan od vaše potvrde servis lokalno Federacija istječu
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 172084b7-68a1-42a5-944d-2e871eaa2972
ms.openlocfilehash: 89a4dd910d43d70e849be19d5f88e281f6d19834
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29461582"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a>Jedan od vaše potvrde servis lokalno Federacija istječu

Da biste riješili taj problem, slijedite ove korake:
  
- Na računalo instalirajte na Microsoft Azure Active Directory modul za Windows PowerShell (Ako već nije instaliran modul). Da biste to učinili, idite na [Azure Active Directory PowerShell za Graph](https://docs.microsoft.com/en-us/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)
    
- Slijedite korake u u "scenariju 1: ADFS token potpisni certifikat istekao" sekcije ["Došlo je do problema prilikom pristupa web-mjestu" Pogreška iz ADFS kada vanjsko korisnik potpiše Office 365, Azure, ili Intune](https://support.microsoft.com/en-us/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).
    
- Slijedite korake u t[kako ažuriranje ili popravak postavke vanjsko domene u Office 365, Azure, ili Intune](https://support.microsoft.com/en-us/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).
    
Dodatne informacije o obnavljanje certifikata Federacija pogledajte [obnove certifikata za O365 i Azure AD](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
  

