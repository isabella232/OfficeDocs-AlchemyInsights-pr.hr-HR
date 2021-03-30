---
title: Pridruživanje servisa Azure Active Directory
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
- "9003257"
- "9890"
ms.openlocfilehash: 59e3798131956847a61af2416c2e4210199cffa5
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/29/2021
ms.locfileid: "51404364"
---
# <a name="azure-active-directory-join"></a><span data-ttu-id="cb6fc-102">Pridruživanje servisa Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="cb6fc-102">Azure Active Directory join</span></span>

1. <span data-ttu-id="cb6fc-103">Ako prvi put postavljate registracije uređaja, provjerite jeste li pregledali uvod u upravljanje uređajima na servisu [Azure Active Directory](/azure/active-directory/devices/overview) koji će vas voditi o tome kako nabaviti uređaje pod kontrolu za Azure AD.</span><span class="sxs-lookup"><span data-stu-id="cb6fc-103">If you are setting up device registrations for the first time, ensure that you have reviewed [Introduction to device management in Azure Active Directory](/azure/active-directory/devices/overview) that will guide you on how to get Devices under the control to Azure AD.</span></span> 
1. <span data-ttu-id="cb6fc-104">Ako izravno registrirate uređaje na Azure AD i registrirate ih u Intune, morat [](/mem/intune/fundamentals/licenses-assign) ćete biti sigurni da ste [konfigurirali Intune](/mem/intune/enrollment/device-enrollment) i da ste prvo registrirali licencu.</span><span class="sxs-lookup"><span data-stu-id="cb6fc-104">If you are registering devices into Azure AD directly and enrolling them into Intune, you will need to ensure that you have [configured Intune](/mem/intune/enrollment/device-enrollment) and have the [licensing](/mem/intune/fundamentals/licenses-assign) in place first.</span></span>
1. <span data-ttu-id="cb6fc-105">Provjerite imate li ovlasti za izvođenje operacija na servisu Azure AD.</span><span class="sxs-lookup"><span data-stu-id="cb6fc-105">Ensure you are authorized to perform operations in Azure AD.</span></span> <span data-ttu-id="cb6fc-106">Samo globalni administrator na servisu Azure AD može upravljati postavkama za registracije uređaja.</span><span class="sxs-lookup"><span data-stu-id="cb6fc-106">Only a global administrator in Azure AD can manage settings for device registrations.</span></span>
1. <span data-ttu-id="cb6fc-107">Da biste u implementaciju pridruživanja servisa Azure AD udružili, [pogledajte planiranje pridruživanja servisu Azure AD](/azure/active-directory/devices/azureadjoin-plan).</span><span class="sxs-lookup"><span data-stu-id="cb6fc-107">To do Azure AD join implementation, see [Plan Azure AD Join](/azure/active-directory/devices/azureadjoin-plan).</span></span>

<span data-ttu-id="cb6fc-108">Dodatne informacije o rješavanju uobičajenih problema s pridruživanjem servisu Azure AD potražite u članku Najčešća pitanja o pridruživanju azure [oglasa](/azure/active-directory/devices/faq) i za uređaj sa sustavom Windows 10 pro potražite u članku Nije moguće pridružiti se računalu sa sustavom [Windows 10 Pro](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900)na Azure AD – morate nadograditi na – Microsoft Community .</span><span class="sxs-lookup"><span data-stu-id="cb6fc-108">For more details on resolving common issues with Azure AD join, see [Azure Ad Join FAQ](/azure/active-directory/devices/faq) and for Windows 10 pro device, see [Unable to join Windows 10 Pro machine to Azure AD - Need to upgrade to - Microsoft Community](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900).</span></span>
