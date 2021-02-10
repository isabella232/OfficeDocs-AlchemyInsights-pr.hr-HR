---
title: Sinkronizacija zaporke za servis domena
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
- "8248"
- "9004400"
- "8249"
- "9003245"
ms.openlocfilehash: 7f138837b720926c5b687285a105eb0417ca5b39
ms.sourcegitcommit: 22eaf0a151ab95414476f596db8d318b6540ff31
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50177384"
---
# <a name="password-hash-synchronization-for-domain-service"></a><span data-ttu-id="5a723-102">Sinkronizacija zaporke za servis domena</span><span class="sxs-lookup"><span data-stu-id="5a723-102">Password hash synchronization for domain service</span></span>

<span data-ttu-id="5a723-103">**Ako vam je instanca servisa Azure AD DS potakla da omogućite sinkronizaciju lozinki za lozinke**</span><span class="sxs-lookup"><span data-stu-id="5a723-103">**If your Azure AD DS instance is prompting you to enable password hash synchronization**</span></span>

<span data-ttu-id="5a723-104">Naiđete na scenarij u kojem se prikazuju hibridno okruženje s sinkronizacijom korisnika iz lokalnog okruženja Azure Active Directory domena Services (AD DS).</span><span class="sxs-lookup"><span data-stu-id="5a723-104">You encounter a scenario in which you are running a hybrid environment with users synchronizing from an on-premises Azure Active Directory Domain Services (AD DS) environment.</span></span> <span data-ttu-id="5a723-105">Ovaj se scenarij susreće unatoč tome što ste sinkroniziranje lozinke iz lokalnog servisa AD DS uključili u zakupac Azure oglasa.</span><span class="sxs-lookup"><span data-stu-id="5a723-105">This scenario is encountered despite you having password hash synchronization from the on-premises AD DS to your Azure AD tenant.</span></span>

<span data-ttu-id="5a723-106">**Jer**</span><span class="sxs-lookup"><span data-stu-id="5a723-106">**Cause**</span></span>

<span data-ttu-id="5a723-107">To se događa budući da se Azure AD Connect po zadanom ne sinkronizira s novim tehnologijama za upravljanje lancima (NTLM) i Kerberos lozinkama koje su potrebne za Azure AD DS.</span><span class="sxs-lookup"><span data-stu-id="5a723-107">This is happening because Azure AD Connect by default does not synchronize legacy New Technology LAN Manager (NTLM) and Kerberos password hashes that are needed for Azure AD DS.</span></span>

<span data-ttu-id="5a723-108">**Workaround**</span><span class="sxs-lookup"><span data-stu-id="5a723-108">**Workaround**</span></span> 

<span data-ttu-id="5a723-109">Morate konfigurirati Azure AD Connect da biste sinkronizirali lozinke koje su potrebne za provjeru autentičnosti NTLM i Kerberos.</span><span class="sxs-lookup"><span data-stu-id="5a723-109">You would need to configure Azure AD Connect to synchronize those password hashes required for NTLM and Kerberos authentication.</span></span>

<span data-ttu-id="5a723-110">Kada je konfigurirana Azure AD Connect, lokalno stvaranje računa ili događaj promjene lozinke također sinkronizira nasljeđene lozinke za Azure AD.</span><span class="sxs-lookup"><span data-stu-id="5a723-110">After Azure AD Connect is configured, an on-premises account creation or password change event also then synchronizes the legacy password hashes to Azure AD.</span></span> <span data-ttu-id="5a723-111">Dodatne informacije o tome potražite [u članku upute](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-password-hash-sync) za omogućivanje sinkronizacije lozinki u hibridnu okruženju Azure AD DS.</span><span class="sxs-lookup"><span data-stu-id="5a723-111">Please see [here](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-password-hash-sync) for more information on this and for guidance on how to enable password synchronization in Azure AD DS hybrid environments.</span></span>