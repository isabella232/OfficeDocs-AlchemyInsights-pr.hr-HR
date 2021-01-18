---
title: Dodjela grupa za Azure AD ulogu
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7898"
- "9003230"
ms.openlocfilehash: feca81fe785bc45e47f6faa876230b5c7701713d
ms.sourcegitcommit: 6dc6f999e840c90694a246b90062950205679420
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 01/15/2021
ms.locfileid: "49884829"
---
# <a name="assigning-groups-to-azure-ad-role"></a><span data-ttu-id="2801b-102">Dodjela grupa za Azure AD ulogu</span><span class="sxs-lookup"><span data-stu-id="2801b-102">Assigning groups to Azure AD role</span></span>

<span data-ttu-id="2801b-103">Da biste grupi Azure oglasa dodijelili izvor autoriteta u servisu Azure ad na ulogu Azure AD, slijedite sljedeće korake:</span><span class="sxs-lookup"><span data-stu-id="2801b-103">To assign an Azure AD group with source of authority in Azure AD to an Azure AD role, perform the following steps:</span></span>

1. <span data-ttu-id="2801b-104">Stvaranje nove grupe – stvaranje nove grupe:</span><span class="sxs-lookup"><span data-stu-id="2801b-104">Create a new group - To create a new group:</span></span>

    <span data-ttu-id="2801b-105">je.</span><span class="sxs-lookup"><span data-stu-id="2801b-105">a.</span></span> <span data-ttu-id="2801b-106">Prijavite se u centar za administratore servisa Azure s **povlaštenim administratorima** i dozvolama za **globalne administratore** .</span><span class="sxs-lookup"><span data-stu-id="2801b-106">Sign in to the Azure AD admin center with **privileged role administrator** or **global administrator** permissions.</span></span>
    <span data-ttu-id="2801b-107">b.</span><span class="sxs-lookup"><span data-stu-id="2801b-107">b.</span></span> <span data-ttu-id="2801b-108">Odaberite **Azure Active Directory > grupe > sve grupe > nova grupa**.</span><span class="sxs-lookup"><span data-stu-id="2801b-108">Select **Azure Active Directory > Groups > All groups > New group**.</span></span>
    <span data-ttu-id="2801b-109">c.</span><span class="sxs-lookup"><span data-stu-id="2801b-109">c.</span></span> <span data-ttu-id="2801b-110">Stvaranje grupe.</span><span class="sxs-lookup"><span data-stu-id="2801b-110">Create the group.</span></span>

2. <span data-ttu-id="2801b-111">Dodijelite ulogu grupi bilo tijekom stvaranja grupe ili nakon stvaranja grupe.</span><span class="sxs-lookup"><span data-stu-id="2801b-111">Assign the role to the group either during group creation or after the group is created.</span></span>

    <span data-ttu-id="2801b-112">je.</span><span class="sxs-lookup"><span data-stu-id="2801b-112">a.</span></span> <span data-ttu-id="2801b-113">Da biste grupi dodijelili ulogu u vrijeme stvaranja grupe, odaberite grupu za uključivanje i isključivanje servisa **Azure** , a zatim stvorite grupu.</span><span class="sxs-lookup"><span data-stu-id="2801b-113">To assign a role to the group at the time of group creation, switch on the toggle **Azure AD roles can be assigned to the group** and create the group.</span></span>
    <span data-ttu-id="2801b-114">b.</span><span class="sxs-lookup"><span data-stu-id="2801b-114">b.</span></span> <span data-ttu-id="2801b-115">Da biste grupi dodijelili ulogu nakon stvaranja, dođite do kartice **dodijeljene uloge** za novostvorenu grupu i dodijelite ulogu grupi.</span><span class="sxs-lookup"><span data-stu-id="2801b-115">To assign a role to the group after it has been created, navigate to the **Assigned roles** tab for the newly created group, and assign the role to the group.</span></span>  

<span data-ttu-id="2801b-116">**Upravljanje članovima grupe koja je dodijeljena ulozi za Azure AD**</span><span class="sxs-lookup"><span data-stu-id="2801b-116">**Manage membership of a group that is assigned to Azure AD role**</span></span>

<span data-ttu-id="2801b-117">Da biste spriječili povećanje privilegija, prema zadanim postavkama, samo administratorske uloge i globalni administratori mogu izmijeniti članstvo grupe dodijeljenu ulozi.</span><span class="sxs-lookup"><span data-stu-id="2801b-117">To prevent elevation of privileges, by default, only privileged role administrators and global administrators can modify the membership of a group that is assigned to a role.</span></span> <span data-ttu-id="2801b-118">Oni mogu, međutim, odabrati dodjelu vlasnika za takvu grupu i delegirati taj zadatak.</span><span class="sxs-lookup"><span data-stu-id="2801b-118">They can, however, choose to assign an owner for such a group and delegate this task.</span></span>

<span data-ttu-id="2801b-119">Dodatne informacije o dodjeljivanju grupa oblaka za Azure oglase potražite u članku [Dodjela uloga oglasa grupi Cloud](https://docs.microsoft.com/azure/active-directory/roles/groups-concept).</span><span class="sxs-lookup"><span data-stu-id="2801b-119">For more details on assigning cloud groups to Azure AD roles, see [Assign a AD roles to Cloud Group](https://docs.microsoft.com/azure/active-directory/roles/groups-concept).</span></span> <span data-ttu-id="2801b-120">Dodatne informacije o ulogama otklanjanja poteškoća dodijeljenim grupama oblaka potražite u članku [Otklanjanje poteškoća s ulogama koje su dodijeljene grupama oblaka](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting).</span><span class="sxs-lookup"><span data-stu-id="2801b-120">For more details on troubleshooting roles assigned to cloud groups, see [Troubleshoot roles assigned to cloud groups](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting).</span></span>





