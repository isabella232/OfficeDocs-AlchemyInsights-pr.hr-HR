---
title: Stvaranje grupe
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003234"
- "7230"
ms.openlocfilehash: b8cb3f1de991bfe7197607d5e8964a018e31c122
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 11/17/2020
ms.locfileid: "49088576"
---
# <a name="create-a-group"></a><span data-ttu-id="9fd34-102">Stvaranje grupe</span><span class="sxs-lookup"><span data-stu-id="9fd34-102">Create a group</span></span>

<span data-ttu-id="9fd34-103">U ovoj se temi opisuje stvaranje grupe.</span><span class="sxs-lookup"><span data-stu-id="9fd34-103">This topic describes group creation.</span></span>

<span data-ttu-id="9fd34-104">**Dozvola za stvaranje grupe**</span><span class="sxs-lookup"><span data-stu-id="9fd34-104">**Permission to Create a Group**</span></span>

<span data-ttu-id="9fd34-105">Provjerite jeste li ovlašteni za stvaranje nove grupe.</span><span class="sxs-lookup"><span data-stu-id="9fd34-105">Ensure you are authorized to create a new group.</span></span> <span data-ttu-id="9fd34-106">Globalni administratori mogu onemogućiti stvaranje grupe na portalu Azure ili na ploči programa Access.</span><span class="sxs-lookup"><span data-stu-id="9fd34-106">Global administrators can disable group creation in the Azure portal or Access Panel.</span></span> <span data-ttu-id="9fd34-107">Da biste stvorili novu grupu za vas, možda će vam trebati administrator ili vam dati odgovarajuće dozvole.</span><span class="sxs-lookup"><span data-stu-id="9fd34-107">You may need an administrator to create the new group for you, or to give you appropriate permissions.</span></span>

<span data-ttu-id="9fd34-108">**Upravljanje dozvolama za stvaranje grupa**</span><span class="sxs-lookup"><span data-stu-id="9fd34-108">**Manage Group creation permissions**</span></span>

1. <span data-ttu-id="9fd34-109">Globalni administratori mogu upravljati dozvolama za stvaranje grupe (zbog sigurnosnih razloga) ili grupa sustava Office 365 stvorenih na portalu Azure ili na ploči programa Access, odabirom mogućnosti "korisnici mogu stvarati sigurnosne grupe na servisu Azure portali" ili "korisnici mogu stvarati grupe sustava Office 365 u sustavima Azure portali" u **svim**  >  **općim grupama (postavke)**.</span><span class="sxs-lookup"><span data-stu-id="9fd34-109">Global administrators can manage group creation permissions (for security-related reasons) or Office 365 groups created in the Azure portal or Access Panel, by choosing "Users can create security groups in Azure portals" or "Users can create Office 365 groups in Azure portals" options in **All groups** > **General (Settings)**.</span></span>
2. <span data-ttu-id="9fd34-110">Možete i ograničiti Stvaranje grupe da biste odabrali grupu korisnika ako imate licencu za Azure Active Directory P1 Premium.</span><span class="sxs-lookup"><span data-stu-id="9fd34-110">You can also restrict group creation to select a group of users if you have an Azure Active Directory P1 Premium license.</span></span>

<span data-ttu-id="9fd34-111">**Onemogućivanje obavijesti dobrodošlice za nove članove grupe sustava Office 365**</span><span class="sxs-lookup"><span data-stu-id="9fd34-111">**Disabling welcome notification for new Office 365 group members**</span></span>

<span data-ttu-id="9fd34-112">Obavijest dobrodošlice koja se šalje korisnicima koji su dodani u grupe sustava Office 365 može se onemogućiti postavljanjem **Unifiedgroupwelcomemessageenabled** u FALSE u komponenti PowerShell.</span><span class="sxs-lookup"><span data-stu-id="9fd34-112">The welcome notification sent to users who are added to Office 365 groups can be disabled by setting **UnifiedGroupWelcomeMessageEnabled** to False in Powershell.</span></span> <span data-ttu-id="9fd34-113">Saznajte više o ovoj [postavci](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="9fd34-113">Learn about this setting [here](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).</span></span>

