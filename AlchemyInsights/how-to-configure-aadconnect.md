---
title: 646 kako konfigurirati AADConnect
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 646
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 6cc4afb4b0f67fb76ecc7ff8f564b1cd36cc291c
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/22/2019
ms.locfileid: "30779504"
---
# <a name="configure-sync-features"></a><span data-ttu-id="32b68-102">Konfiguriranje značajke sinkronizacije</span><span class="sxs-lookup"><span data-stu-id="32b68-102">Configure sync features</span></span>

<span data-ttu-id="32b68-103">Povezivanje Azure AD uključuje nekoliko značajki koje su omogućena po zadanom ili koje kasnije možete omogućiti.</span><span class="sxs-lookup"><span data-stu-id="32b68-103">Azure AD Connect includes several features that are enabled by default, or that you can enable later.</span></span> <span data-ttu-id="32b68-104">Neke značajke zahtijevaju dodatnu konfiguraciju u određenim okruženjima.</span><span class="sxs-lookup"><span data-stu-id="32b68-104">Some features require additional configuration in specific environments.</span></span>
  
- <span data-ttu-id="32b68-105">[Filtriranje](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) ograničenja objekata se sinkroniziraju Azure AD.</span><span class="sxs-lookup"><span data-stu-id="32b68-105">[Filtering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) limits the objects are synchronized to Azure AD.</span></span> <span data-ttu-id="32b68-106">Po zadanom, sve korisnici, kontakti, grupe i Windows 10 sinkroniziraju se računi na računalu.</span><span class="sxs-lookup"><span data-stu-id="32b68-106">By default, all users, contacts, groups, and Windows 10 computer accounts are synchronized.</span></span> <span data-ttu-id="32b68-107">Možete uključiti ili isključiti na temelju domene, organizacijske jedinice ili druge atribute objekata.</span><span class="sxs-lookup"><span data-stu-id="32b68-107">You can include or exclude objects based on domains, OUs, or other attributes.</span></span> 
    
- <span data-ttu-id="32b68-108">[Lozinka raspršivanja sinkronizacije](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) sinkronizira raspršivanja lozinku iz lokalno servisa Active Directory za Azure AD.</span><span class="sxs-lookup"><span data-stu-id="32b68-108">[Password hash syncronization](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synchronizes the password hash from the on-premises Active Directory to Azure AD.</span></span> <span data-ttu-id="32b68-109">To omogućuje upravljanje lozinkom na jedno mjesto, ali koristi istu lozinku u oba lokalno i oblak okruženjima.</span><span class="sxs-lookup"><span data-stu-id="32b68-109">This allows password management in one location, but use of the same password in both on-premises and cloud environments.</span></span> <span data-ttu-id="32b68-110">Jer je Active Directory mjerodavne izvora, možete koristiti vlastite pravila lozinke.</span><span class="sxs-lookup"><span data-stu-id="32b68-110">Because Active Directory is the authoritative source, you can use your own password policies.</span></span> 
    
- <span data-ttu-id="32b68-111">[(SSPR) za vraćanje izvorne lozinke samoposlužno](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) omogućava korisnicima da Vrati svoje vlastite lozinke oblak dok još uvijek se primjenjuju pravila za lozinke lokalno.</span><span class="sxs-lookup"><span data-stu-id="32b68-111">[Self-service password reset (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) allows users to reset their own passwords in the cloud while still applying your on-premises password policy.</span></span> 
    
- <span data-ttu-id="32b68-112">[Writeback uređaj](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) dopušta registrirani uređaji u Azure AD budu napisani natrag na lokalno Active Directory pa se može koristiti za uvjetno pristup.</span><span class="sxs-lookup"><span data-stu-id="32b68-112">[Device writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) allows registered devices in Azure AD to be written back to the on-premises Active Directory so they can be used for conditional access.</span></span> 
    
- <span data-ttu-id="32b68-113">[Briše spriječi slučajnog](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) po zadanom je omogućena za sprečavanje brisanja previše istodobnih objekt (više od 500 objekata po sinkronizacije).</span><span class="sxs-lookup"><span data-stu-id="32b68-113">[Prevent accidental deletes](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) is enabled by default to help prevent too many simultaneous object deletions (more than 500 objects per synchronization).</span></span> <span data-ttu-id="32b68-114">Možete promijeniti ovu postavku potrebama vaše organizacije.</span><span class="sxs-lookup"><span data-stu-id="32b68-114">You can change this setting to meet the needs of your organization.</span></span> 
    
- <span data-ttu-id="32b68-115">[Automatske nadogradnje](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) omogućena je po zadanom express instalacijama i osigurava vaša verzija Azure AD povezivanje uvijek je trenutni.</span><span class="sxs-lookup"><span data-stu-id="32b68-115">[Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) is enabled by default for express installations and helps ensure your version of Azure AD Connect is always current.</span></span> 
    

