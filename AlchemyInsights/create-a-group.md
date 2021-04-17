---
title: Stvaranje grupe
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003234"
- "7230"
ms.openlocfilehash: ec74b7c098d302d3bdeb5a412fad41efe7b82b98
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816340"
---
# <a name="create-a-group"></a><span data-ttu-id="3eba9-102">Stvaranje grupe</span><span class="sxs-lookup"><span data-stu-id="3eba9-102">Create a group</span></span>

<span data-ttu-id="3eba9-103">U ovoj se temi opisuje stvaranje grupe.</span><span class="sxs-lookup"><span data-stu-id="3eba9-103">This topic describes group creation.</span></span>

<span data-ttu-id="3eba9-104">**Dozvola za stvaranje grupe**</span><span class="sxs-lookup"><span data-stu-id="3eba9-104">**Permission to Create a Group**</span></span>

<span data-ttu-id="3eba9-105">Provjerite jeste li ovlašteni za stvaranje nove grupe.</span><span class="sxs-lookup"><span data-stu-id="3eba9-105">Ensure you are authorized to create a new group.</span></span> <span data-ttu-id="3eba9-106">Globalni administratori mogu onemogućiti stvaranje grupe na portalu Azure ili ploči programa Access.</span><span class="sxs-lookup"><span data-stu-id="3eba9-106">Global administrators can disable group creation in the Azure portal or Access Panel.</span></span> <span data-ttu-id="3eba9-107">Možda će vam biti potreban administrator da biste za vas stvorili novu grupu ili vam dali odgovarajuće dozvole.</span><span class="sxs-lookup"><span data-stu-id="3eba9-107">You may need an administrator to create the new group for you, or to give you appropriate permissions.</span></span>

<span data-ttu-id="3eba9-108">**Upravljanje dozvolama za stvaranje grupe**</span><span class="sxs-lookup"><span data-stu-id="3eba9-108">**Manage Group creation permissions**</span></span>

1. <span data-ttu-id="3eba9-109">Globalni administratori mogu upravljati dozvolama za stvaranje grupa (iz sigurnosnih razloga) ili grupama sustava Office 365 stvorenima na portalu Azure ili na ploči programa Access, odabirom mogućnosti "Korisnici mogu stvarati sigurnosne grupe na portalima azure" ili "Korisnici mogu stvarati grupe sustava Office 365 na portalima azure" u odjeljku Sve **grupe**  >  **Općenito (Postavke).**</span><span class="sxs-lookup"><span data-stu-id="3eba9-109">Global administrators can manage group creation permissions (for security-related reasons) or Office 365 groups created in the Azure portal or Access Panel, by choosing "Users can create security groups in Azure portals" or "Users can create Office 365 groups in Azure portals" options in **All groups** > **General (Settings)**.</span></span>
2. <span data-ttu-id="3eba9-110">Ako imate licencu za Azure Active Directory P1 Premium, možete i ograničiti stvaranje grupe da biste odabrali grupu korisnika.</span><span class="sxs-lookup"><span data-stu-id="3eba9-110">You can also restrict group creation to select a group of users if you have an Azure Active Directory P1 Premium license.</span></span>

<span data-ttu-id="3eba9-111">**Onemogućivanje obavijesti o dobrodošlici za nove članove grupe sustava Office 365**</span><span class="sxs-lookup"><span data-stu-id="3eba9-111">**Disabling welcome notification for new Office 365 group members**</span></span>

<span data-ttu-id="3eba9-112">Obavijest dobrodošlice poslana korisnicima koji su dodani u grupe sustava Office 365 može se onemogućiti postavljanjem **UnifiedGroupWelcomeMessageEnabled** na False u ljuski Powershell.</span><span class="sxs-lookup"><span data-stu-id="3eba9-112">The welcome notification sent to users who are added to Office 365 groups can be disabled by setting **UnifiedGroupWelcomeMessageEnabled** to False in Powershell.</span></span> <span data-ttu-id="3eba9-113">Ovdje se informirajte o [ovoj postavki](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="3eba9-113">Learn about this setting [here](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).</span></span>

