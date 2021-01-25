---
title: Problem s dodjelom resursa za SCIM
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/22/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7854"
- "9004348"
ms.openlocfilehash: aa5b4cbb99cb1a5a323b39101766bea55fd49064
ms.sourcegitcommit: 953a8567ebcd9835f8c5c49472b223107c92549b
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 01/22/2021
ms.locfileid: "49949671"
---
# <a name="scim-provisioning-issue"></a><span data-ttu-id="55e1b-102">Problem s dodjelom resursa za SCIM</span><span class="sxs-lookup"><span data-stu-id="55e1b-102">SCIM provisioning issue</span></span>

<span data-ttu-id="55e1b-103">Automatska dodjela resursa odnosi se na stvaranje korisničkih identiteta i uloga u aplikacijama u oblaku kojima je korisniku potreban pristup.</span><span class="sxs-lookup"><span data-stu-id="55e1b-103">Automatic provisioning refers to creating user identities and roles in the cloud applications that users need access to.</span></span> <span data-ttu-id="55e1b-104">Osim stvaranja korisničkih identiteta, automatska dodjela resursa obuhvaća održavanje i uklanjanje korisničkih identiteta kao promjene statusa ili uloga.</span><span class="sxs-lookup"><span data-stu-id="55e1b-104">In addition to creating user identities, automatic provisioning includes the maintenance and removal of user identities as status or roles change.</span></span> <span data-ttu-id="55e1b-105">Prije nego što započnete implementaciju, možete pregledati [način dodjele](https://docs.microsoft.com/azure/active-directory/app-provisioning/how-provisioning-works) resursa da biste doznali kako funkcionira Azure Active Directory (AD) i dobili preporuke za konfiguriranje.</span><span class="sxs-lookup"><span data-stu-id="55e1b-105">Before you start a deployment, you can review [How provisioning works](https://docs.microsoft.com/azure/active-directory/app-provisioning/how-provisioning-works) to learn how Azure Active Directory (AD) provision works, and get configuration recommendations.</span></span>

<span data-ttu-id="55e1b-106">Kao programer aplikacija možete koristiti sustav za upravljanje upravljanjem identitetima (SCIM) da biste omogućili automatsko dodjeljivanje korisnika i grupa između aplikacija i servisa Azure AD.</span><span class="sxs-lookup"><span data-stu-id="55e1b-106">As an application developer, you can use the System for Cross-Domain Identity Management (SCIM) user management API to enable automatic provisioning of users and groups between your application and Azure AD.</span></span> <span data-ttu-id="55e1b-107">[Stvaranje scim krajnje točke i konfiguriranje dodjele korisnika pomoću članka Azure ad](https://docs.microsoft.com/azure/active-directory/app-provisioning/use-scim-to-provision-users-and-groups) opisuje kako stvoriti krajnju točku scim i integrirati je pomoću servisa za dodjelu resursa za Azure AD.</span><span class="sxs-lookup"><span data-stu-id="55e1b-107">The [Build a SCIM endpoint and configure user provisioning with Azure AD](https://docs.microsoft.com/azure/active-directory/app-provisioning/use-scim-to-provision-users-and-groups) article describes how to build an SCIM endpoint and integrate it with the Azure AD provisioning service.</span></span>



