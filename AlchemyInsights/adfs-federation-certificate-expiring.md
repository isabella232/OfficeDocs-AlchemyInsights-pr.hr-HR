---
title: Istječe certifikat ADFS federacije
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: 14e7da6220dfa96edca5d9ec5c32e003480a9eaf
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43710399"
---
# <a name="adfs-federation-certificate-expiring"></a>Istječe certifikat ADFS federacije

Da biste riješili taj problem, slijedite ove korake:
  
1. Instalirajte Modul servisa Microsoft Azure Active Directory za Windows PowerShell na računalu (ako modul već nije instaliran). Da biste to učinili, idite na [Upravljanje Azure AD pomoću komponente Windows PowerShell](https://aka.ms/aadposh).

2. Slijedite korake u odjeljku "Scenarij 1: Certifikat za potpisivanje tokena AD FS istekao" pogreške "Došlo je do [problema s pristupom web-mjestu" iz AD FS-a kada se vanjski korisnik prijavi u Microsoft 365, Azure ili Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).

3. Slijedite korake u [odjeljku Ažuriranje ili popravak postavki združene domene u microsoft, azure ili intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).

    Dodatne informacije o obnovi certifikata federacije potražite u članku [Obnavljanje certifikata za federaciju za Microsoft 365 i Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
