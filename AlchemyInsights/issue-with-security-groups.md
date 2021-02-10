---
title: Problem s sigurnosnim grupama
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8252"
- "9004397"
ms.openlocfilehash: 1198b79c3301bd2752a7385a6ba6746c8f0c2b5b
ms.sourcegitcommit: 22eaf0a151ab95414476f596db8d318b6540ff31
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50177385"
---
# <a name="issue-with-security-groups"></a><span data-ttu-id="e6eb7-102">Problem s sigurnosnim grupama</span><span class="sxs-lookup"><span data-stu-id="e6eb7-102">Issue with security groups</span></span>

<span data-ttu-id="e6eb7-103">**Ako vam se prikazuje Mrežna pogreška AADDS104**</span><span class="sxs-lookup"><span data-stu-id="e6eb7-103">**If you are getting Network Error AADDS104**</span></span>

<span data-ttu-id="e6eb7-104">Nevaljana pravila grupe za mrežnu sigurnost najčešći su uzrok mrežnih pogrešaka za Azure Active Directory domene Services (AD DS).</span><span class="sxs-lookup"><span data-stu-id="e6eb7-104">Invalid network security group rules are the most common cause of network errors for Azure Active Directory Domain Services (AD DS).</span></span> <span data-ttu-id="e6eb7-105">Mrežna sigurnost grupa za virtualnu mrežu mora dopustiti pristup određenim lukama i protokoli.</span><span class="sxs-lookup"><span data-stu-id="e6eb7-105">The network security group for the virtual network must allow access to specific ports and protocols.</span></span> <span data-ttu-id="e6eb7-106">Ako su ovi priključci blokirani, platforma Azure ne može nadzirati ni ažurirati upravljane domene.</span><span class="sxs-lookup"><span data-stu-id="e6eb7-106">If these ports are blocked, the Azure platform can't monitor or update the managed domain.</span></span> <span data-ttu-id="e6eb7-107">Usklañeno je i sinkronizacija između Azure i Azure AD DS-a.</span><span class="sxs-lookup"><span data-stu-id="e6eb7-107">The synchronization between the Azure AD and Azure AD DS is also impacted.</span></span> <span data-ttu-id="e6eb7-108">Pobrinite se da zadani portovi ostanu otvoreni da biste izbjegli prekid servisa.</span><span class="sxs-lookup"><span data-stu-id="e6eb7-108">Ensure you keep the default ports open to avoid interruption in service.</span></span>

<span data-ttu-id="e6eb7-109">Da biste razumjeli i riješili najčešća upozorenja o problemima s konfiguracijom mrežne sigurnosne grupe, pročitajte članak [Dodavanje i provjera sigurnosnih grupa](https://docs.microsoft.com/azure/active-directory-domain-services/alert-nsg#verify-and-edit-existing-security-rules).</span><span class="sxs-lookup"><span data-stu-id="e6eb7-109">To understand and to resolve common alerts for network security group configuration issues, see [Add and Verify Security Groups](https://docs.microsoft.com/azure/active-directory-domain-services/alert-nsg#verify-and-edit-existing-security-rules).</span></span>
