---
title: ADFS Federation Certificate Expiring
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
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: 48d4ccbbc0ed3dc54cbcd17ae7b9040bfd9ecc426897c06b653bf40bc7d5e9b2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53952961"
---
# <a name="adfs-federation-certificate-expiring"></a>ADFS Federation Certificate Expiring

Da biste riješili taj problem, slijedite ove korake:
  
1. Instalirajte modul Microsoft Azure Active Directory za Windows PowerShell na računalo (ako modul još nije instaliran). Da biste to učiniti, idite [na Upravljanje servisom Azure AD pomoću Windows PowerShell](https://aka.ms/aadposh).

2. Slijedite korake u odjeljku "Scenarij 1: certifikat za potpisivanje tokena za AD FS istekao" u odjeljku "Došlo je do problema prilikom pristupa web-mjestu" iz AD FS-a kada se vanjski korisnik prijavi [u Microsoft 365, Azure ili Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).

3. Slijedite korake u [odjeljku Ažuriranje ili popravak postavki vanjske domene u sustavu Microsoft, Azure ili Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).

    Dodatne informacije o obnovi certifikata o federaciji potražite u članku Obnavljanje [certifikata](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)za Microsoft 365 i Azure Active Directory .
