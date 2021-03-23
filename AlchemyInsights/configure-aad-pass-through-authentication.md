---
title: Konfiguriranje provjere autentičnosti servisa Azure Active Directory
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6970"
- "9003915"
ms.openlocfilehash: be993b1f22d89a92afb099937dae815dc9c09e0e
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035141"
---
# <a name="configure-azure-active-directory-pass-through-authentication"></a><span data-ttu-id="b2722-102">Konfiguriranje provjere autentičnosti servisa Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="b2722-102">Configure Azure Active Directory pass-through authentication</span></span>

<span data-ttu-id="b2722-103">Evo nekoliko vodiča koji će vam pomoći pri konfiguriranju provjere autentičnosti u prolazu:</span><span class="sxs-lookup"><span data-stu-id="b2722-103">Here are some guides to help you configure pass-through authentication:</span></span>

- <span data-ttu-id="b2722-104">**Da biste postavili Azure Active Directory Connect**: [Sinkronizacijski korisnici u vodiču za direktorij](https://admin.microsoft.com/AdminPortal/Home) pomažu vam da konfigurirate sinkronizaciju lozinki i prolaznu provjeru autentičnosti.</span><span class="sxs-lookup"><span data-stu-id="b2722-104">**To set up Azure Active Directory Connect**: The [Sync users to your directory](https://admin.microsoft.com/AdminPortal/Home) guide helps you configure password hash synchronization or pass-through authentication.</span></span> <span data-ttu-id="b2722-105">Ta konfiguracija korisnicima omogućuje prijavu u svoju e-poštu i lokalni Active Directory (kontroler domene) pomoću iste lozinke.</span><span class="sxs-lookup"><span data-stu-id="b2722-105">This configuration enables users to sign in to their email and to your on-premises Active Directory (domain controller) using the same password.</span></span>  <span data-ttu-id="b2722-106">[Sinkronizacijski korisnici u vodiču za direktorije](https://admin.microsoft.com/AdminPortal/Home) obuhvaćaju i prijavu u Federaciji uz servis Active Directory Federation Services (AD FS).</span><span class="sxs-lookup"><span data-stu-id="b2722-106">The [Sync users to your directory](https://admin.microsoft.com/AdminPortal/Home) guide also covers federation sign-in with Active Directory Federation Services (AD FS), too.</span></span>

- <span data-ttu-id="b2722-107">**Da biste postavili značajke Azure**: [Vodič za postavljanje Azure ad vas vodi](https://admin.microsoft.com/adminportal/home#/modernonboarding/azureadsetup) kroz postavljanje značajki u servisu Azure Active Directory Basic, kao što je upravljanje pristupom temeljeno na grupi, samoposlužno vraćanje lozinke za aplikacije Cloud i Azure Active Directory proxy aplikacije za objavljivanje lokalnih web-aplikacija.</span><span class="sxs-lookup"><span data-stu-id="b2722-107">**To set up Azure features**: The [Azure AD setup guide](https://admin.microsoft.com/adminportal/home#/modernonboarding/azureadsetup) walks you through setting up the features in Azure Active Directory Basic, like group-based access management, self-service password reset for cloud apps, and Azure Active Directory Application Proxy for publishing on-premises web apps.</span></span>


