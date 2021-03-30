---
title: Otklanjanje poteškoća s pridruživanjem servisa Azure AD
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003246"
- "6157"
ms.openlocfilehash: 0e9f7c95cf522340e9976f668c1d1a9eaff71910
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/29/2021
ms.locfileid: "51404381"
---
# <a name="troubleshoot-azure-ad-join-issues"></a><span data-ttu-id="247e8-102">Otklanjanje poteškoća s pridruživanjem servisa Azure AD</span><span class="sxs-lookup"><span data-stu-id="247e8-102">Troubleshoot Azure AD join issues</span></span>

1. <span data-ttu-id="247e8-103">Ako prvi put postavljate registracije uređaja, provjerite jeste li pregledali uvod u upravljanje uređajima na servisu [Azure Active Directory](https://docs.microsoft.com/azure/active-directory/devices/overview) koji će vas voditi o tome kako nabaviti uređaje pod kontrolu za Azure AD.</span><span class="sxs-lookup"><span data-stu-id="247e8-103">If you are setting up device registrations for the first time, ensure that you have reviewed [Introduction to device management in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/devices/overview) that will guide you on how to get Devices under the control to Azure AD.</span></span> 
1. <span data-ttu-id="247e8-104">Ako izravno registrirate uređaje na Azure AD i registrirate ih u Intune, morat [](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign) ćete biti sigurni da ste [konfigurirali Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment) i da ste prvo registrirali licencu.</span><span class="sxs-lookup"><span data-stu-id="247e8-104">If you are registering devices into Azure AD directly and enrolling them into Intune, you will need to ensure that you have [configured Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment) and have the [licensing](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign) in place first.</span></span>
1. <span data-ttu-id="247e8-105">Provjerite imate li ovlasti za izvođenje operacija na servisu Azure AD.</span><span class="sxs-lookup"><span data-stu-id="247e8-105">Ensure you are authorized to perform operations in Azure AD.</span></span> <span data-ttu-id="247e8-106">Samo globalni administrator na servisu Azure AD može upravljati postavkama za registracije uređaja.</span><span class="sxs-lookup"><span data-stu-id="247e8-106">Only a global administrator in Azure AD can manage settings for device registrations.</span></span>
1. <span data-ttu-id="247e8-107">Da biste u implementaciju pridruživanja servisa Azure AD udružili, [pogledajte planiranje pridruživanja servisu Azure AD](https://docs.microsoft.com/azure/active-directory/devices/azureadjoin-plan).</span><span class="sxs-lookup"><span data-stu-id="247e8-107">To do Azure AD join implementation, see [Plan Azure AD Join](https://docs.microsoft.com/azure/active-directory/devices/azureadjoin-plan).</span></span>

<span data-ttu-id="247e8-108">Dodatne informacije o rješavanju uobičajenih problema s pridruživanjem servisa Azure AD potražite u članku [Najčešća](https://docs.microsoft.com/azure/active-directory/devices/faq#azure-ad-join-faq) pitanja o pridruživanju servisu Azure Ad i uređaju sa sustavom Windows 10 pro potražite u članku Nemogućnost pridruživanja računalu sa sustavom Windows 10 Pro na Azure AD – potrebno je nadograditi [na Microsoftovu zajednicu](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900)</span><span class="sxs-lookup"><span data-stu-id="247e8-108">For more details on resolving  common issues with Azure AD join see [Azure Ad Join FAQ](https://docs.microsoft.com/azure/active-directory/devices/faq#azure-ad-join-faq) and for Windows 10 pro device, see [Unable to join Windows 10 Pro machine to Azure AD - Need to upgrade to - Microsoft Community](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900)</span></span>
