---
title: Otklanjanje poteškoća s hibridnim pridruživanjem servisa Azure AD
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/06/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6162"
- "6158"
- "9003244"
- "9003246"
ms.openlocfilehash: 18d0ce6bdf3df96e07cc6607b9ae6142d548dabe
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/29/2021
ms.locfileid: "51401899"
---
# <a name="troubleshoot-hybrid-azure-ad-join"></a><span data-ttu-id="89475-102">Otklanjanje poteškoća s hibridnim pridruživanjem servisa Azure AD</span><span class="sxs-lookup"><span data-stu-id="89475-102">Troubleshoot Hybrid Azure AD join</span></span>

<span data-ttu-id="89475-103">Preporučuje se da uređaj može pristupati krajnjim točkama registracije uređaja u odjeljku računa sustava pomoću skripte [Test Device Registration Connectivity](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/).</span><span class="sxs-lookup"><span data-stu-id="89475-103">Highly Recommended Ensure that a device can access Device Registration endpoints under the system account by using the [Test Device Registration Connectivity script](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/).</span></span>

1. <span data-ttu-id="89475-104">Ako prvi put postavljate registracije uređaja, obavezno pregledajte[ntroduction](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) za upravljanje uređajima na servisu Azure Active Directory da biste saznali kako nabaviti uređaje pod kontrolom servisa Azure AD.</span><span class="sxs-lookup"><span data-stu-id="89475-104">If you are setting up device registrations for the first time, be sure to review I[ntroduction to device management in Azure Active Directory](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) to learn how to get devices under the control of Azure AD.</span></span>
1. <span data-ttu-id="89475-105">Ako izravno registrirate uređaje na Azure AD i upisujete ih u Intune, provjerite jeste li [konfigurirali Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) i imate [li](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) prvo licencu.</span><span class="sxs-lookup"><span data-stu-id="89475-105">If you are registering devices into Azure AD directly and enrolling them into Intune, be sure that you've [configured Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) and have the [licensing](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) in place first.</span></span>
1. <span data-ttu-id="89475-106">Provjerite jeste li ovlašteni za izvođenje operacija na servisu Azure AD i lokalnom servisu AD.</span><span class="sxs-lookup"><span data-stu-id="89475-106">Ensure that you are authorized to perform operations in Azure AD and on-premises AD.</span></span> <span data-ttu-id="89475-107">Samo globalni administrator na servisu Azure AD može upravljati postavkama za registracije uređaja.</span><span class="sxs-lookup"><span data-stu-id="89475-107">Only a global administrator in Azure AD can manage settings for device registrations.</span></span> <span data-ttu-id="89475-108">Osim toga, ako postavljate automatske registracije u lokalnom servisu Active Directory, morat ćete biti administrator servisa Active Directory i AD FS (ako je primjenjivo).</span><span class="sxs-lookup"><span data-stu-id="89475-108">In addition, if you are setting up automatic registrations in your on-premises Active Directory, you will need to be an administrator of Active Directory and AD FS (if applicable).</span></span>

<span data-ttu-id="89475-109">Dodatne informacije o rješavanju potencijalnih [](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current) problema s hibridnim pridruživanjem potražite u članku Otklanjanje poteškoća s hibridnim pridruživanjem za postavljanje hibridnih uređaja pridruženih servisu Azure AD i upravljanje uređajima pomoću portala Azure Ad, pogledajte postavljanje hibridnih uređaja pridruženih servisu [Azure AD (lokalno](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan?WT.mc_id=Portal-Microsoft_Azure_Support) pridruženim domenama) i Upravljanje uređajima pomoću [portala Azure](https://docs.microsoft.com/azure/active-directory/devices/device-management-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="89475-109">For more details on resolve potential issues with Hybrid join, see [Troubleshoot Hybrid Join](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current) for set up hybrid Azure AD joined and Manage Devices using Azure Ad portal, see [Set up hybrid Azure AD joined (on-premises domain-joined) devices](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan?WT.mc_id=Portal-Microsoft_Azure_Support) and [Manage devices using the Azure portal](https://docs.microsoft.com/azure/active-directory/devices/device-management-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="89475-110">Da biste riješili uobičajene probleme s hibridnim pridruživanjem servisa Azure Active Directory (AD), pogledajte najčešća pitanja o [hibridnom pridruživanju servisa Azure AD](https://docs.microsoft.com/azure/active-directory/devices/faq#hybrid-azure-ad-join-faq).</span><span class="sxs-lookup"><span data-stu-id="89475-110">To resolve common issues with Hybrid Azure Active Directory (AD) join, see [Hybrid Azure AD join FAQ](https://docs.microsoft.com/azure/active-directory/devices/faq#hybrid-azure-ad-join-faq).</span></span>
