---
title: ADFS Federacija certifikata istječe
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 6/8/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: eafd31e91340b41b7948fb1fe62889731b816d9a
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 10/18/2019
ms.locfileid: "36737181"
---
# <a name="adfs-federation-certificate-expiring"></a><span data-ttu-id="b5cb5-102">ADFS Federacija certifikata istječe</span><span class="sxs-lookup"><span data-stu-id="b5cb5-102">ADFS Federation Certificate Expiring</span></span>

<span data-ttu-id="b5cb5-103">Da biste riješili taj problem, slijedite ove korake:</span><span class="sxs-lookup"><span data-stu-id="b5cb5-103">To resolve this issue, follow these steps:</span></span>
  
1. <span data-ttu-id="b5cb5-104">Instalirajte Microsoft Azure Active Directory modul za Windows PowerShell na računalu (ako modul nije već instaliran).</span><span class="sxs-lookup"><span data-stu-id="b5cb5-104">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed).</span></span> <span data-ttu-id="b5cb5-105">Da biste to učinili, idite na [Upravljanje uslugom Azure ad pomoću sustava Windows PowerShell](https://aka.ms/aadposh).</span><span class="sxs-lookup"><span data-stu-id="b5cb5-105">To do this, go to [Manage Azure AD using Windows PowerShell](https://aka.ms/aadposh).</span></span>

2. <span data-ttu-id="b5cb5-106">Slijedite korake u odjeljku "scenarij 1.: istekao je rok valjanosti certifikata potpisa AD FS-a" u sekciji ["došlo je do problema pri pristupu web-mjestu" od AD FS-a kada se vanjski korisnik prijavljuje u Office 365, Azure ili Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span><span class="sxs-lookup"><span data-stu-id="b5cb5-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Office 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>

3. <span data-ttu-id="b5cb5-107">Slijedite korake u [ažuriranju ili popravite postavke savezne domene u sustavu Office 365, Azure ili Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).</span><span class="sxs-lookup"><span data-stu-id="b5cb5-107">Follow the steps in [Update or repair the settings of a federated domain in Office 365, Azure, or Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).</span></span>

    <span data-ttu-id="b5cb5-108">Da biste saznali više o obnavljanju certifikata Federacije, pogledajte [obnavljanje federacijskih certifikata za Office 365 i Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span><span class="sxs-lookup"><span data-stu-id="b5cb5-108">To learn more about renewing Federation certificates, see [Renew federation certificates for Office 365 and Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
