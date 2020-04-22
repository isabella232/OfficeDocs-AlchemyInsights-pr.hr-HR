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
# <a name="adfs-federation-certificate-expiring"></a><span data-ttu-id="f393c-102">Istječe certifikat ADFS federacije</span><span class="sxs-lookup"><span data-stu-id="f393c-102">ADFS Federation Certificate Expiring</span></span>

<span data-ttu-id="f393c-103">Da biste riješili taj problem, slijedite ove korake:</span><span class="sxs-lookup"><span data-stu-id="f393c-103">To resolve this issue, follow these steps:</span></span>
  
1. <span data-ttu-id="f393c-104">Instalirajte Modul servisa Microsoft Azure Active Directory za Windows PowerShell na računalu (ako modul već nije instaliran).</span><span class="sxs-lookup"><span data-stu-id="f393c-104">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed).</span></span> <span data-ttu-id="f393c-105">Da biste to učinili, idite na [Upravljanje Azure AD pomoću komponente Windows PowerShell](https://aka.ms/aadposh).</span><span class="sxs-lookup"><span data-stu-id="f393c-105">To do this, go to [Manage Azure AD using Windows PowerShell](https://aka.ms/aadposh).</span></span>

2. <span data-ttu-id="f393c-106">Slijedite korake u odjeljku "Scenarij 1: Certifikat za potpisivanje tokena AD FS istekao" pogreške "Došlo je do [problema s pristupom web-mjestu" iz AD FS-a kada se vanjski korisnik prijavi u Microsoft 365, Azure ili Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span><span class="sxs-lookup"><span data-stu-id="f393c-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Microsoft 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>

3. <span data-ttu-id="f393c-107">Slijedite korake u [odjeljku Ažuriranje ili popravak postavki združene domene u microsoft, azure ili intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).</span><span class="sxs-lookup"><span data-stu-id="f393c-107">Follow the steps in [Update or repair the settings of a federated domain in Microsoft, Azure, or Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).</span></span>

    <span data-ttu-id="f393c-108">Dodatne informacije o obnovi certifikata federacije potražite u članku [Obnavljanje certifikata za federaciju za Microsoft 365 i Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span><span class="sxs-lookup"><span data-stu-id="f393c-108">To learn more about renewing Federation certificates, see [Renew federation certificates for Microsoft 365 and Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
