---
title: 646 Kako konfigurirati AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "646"
- "1300023"
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 713cda26e55f07f0438cb9ebe5aa9da86c4ebb3a
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43722521"
---
# <a name="configure-sync-features"></a><span data-ttu-id="11c4e-102">Konfiguriranje značajki sinkronizacije</span><span class="sxs-lookup"><span data-stu-id="11c4e-102">Configure sync features</span></span>

<span data-ttu-id="11c4e-103">Azure AD Connect sadrži nekoliko značajki koje su prema zadanim postavkama omogućene ili koje možete omogućiti kasnije.</span><span class="sxs-lookup"><span data-stu-id="11c4e-103">Azure AD Connect includes several features that are enabled by default, or that you can enable later.</span></span> <span data-ttu-id="11c4e-104">Neke značajke zahtijevaju dodatnu konfiguraciju u određenim okruženjima.</span><span class="sxs-lookup"><span data-stu-id="11c4e-104">Some features require additional configuration in specific environments.</span></span>

- <span data-ttu-id="11c4e-105">[Filtriranje](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) ograničava da se objekti sinkroniziraju sa Azure AD-om.</span><span class="sxs-lookup"><span data-stu-id="11c4e-105">[Filtering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) limits the objects are synchronized to Azure AD.</span></span> <span data-ttu-id="11c4e-106">Prema zadanim postavkama, svi korisnici, kontakti, grupe i računi računala sa sustavom Windows 10 sinkroniziraju se.</span><span class="sxs-lookup"><span data-stu-id="11c4e-106">By default, all users, contacts, groups, and Windows 10 computer accounts are synchronized.</span></span> <span data-ttu-id="11c4e-107">Objekte možete uključiti ili izuzeti na temelju domena, OU-ova ili drugih atributa.</span><span class="sxs-lookup"><span data-stu-id="11c4e-107">You can include or exclude objects based on domains, OUs, or other attributes.</span></span>

- <span data-ttu-id="11c4e-108">[Sinkronizacija raspisija](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) lozinkom sinkronizira raspadjevi lozinke iz lokalnog servisa Active Directory u Azure AD.</span><span class="sxs-lookup"><span data-stu-id="11c4e-108">[Password hash synchronization](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synchronizes the password hash from the on-premises Active Directory to Azure AD.</span></span> <span data-ttu-id="11c4e-109">To omogućuje upravljanje lozinkom na jednom mjestu, ali korištenje iste lozinke u lokalnim i cloud okruženjima.</span><span class="sxs-lookup"><span data-stu-id="11c4e-109">This allows password management in one location, but use of the same password in both on-premises and cloud environments.</span></span> <span data-ttu-id="11c4e-110">Budući da je Active Directory autoritativni izvor, možete koristiti vlastita pravila za lozinku.</span><span class="sxs-lookup"><span data-stu-id="11c4e-110">Because Active Directory is the authoritative source, you can use your own password policies.</span></span>

- <span data-ttu-id="11c4e-111">[Samoposlužno ponovno postavljanje lozinke (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) korisnicima omogućuje ponovno postavljanje vlastitih lozinki u oblaku, a da još uvijek primjenjujete pravila lokalne lozinke.</span><span class="sxs-lookup"><span data-stu-id="11c4e-111">[Self-service password reset (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) allows users to reset their own passwords in the cloud while still applying your on-premises password policy.</span></span>

- <span data-ttu-id="11c4e-112">[Povrat podataka uređaja](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) omogućuje vraćanje registriranih uređaja u Azure AD u lokalni Active Directory da bi se mogli koristiti za uvjetni pristup.</span><span class="sxs-lookup"><span data-stu-id="11c4e-112">[Device writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) allows registered devices in Azure AD to be written back to the on-premises Active Directory so they can be used for conditional access.</span></span>

- <span data-ttu-id="11c4e-113">[Sprječavanje slučajnog brisanja](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) omogućeno je prema zadanim postavkama kako bi se spriječilo previše istovremenih brisanja objekata (više od 500 objekata po sinkronizaciji).</span><span class="sxs-lookup"><span data-stu-id="11c4e-113">[Prevent accidental deletes](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) is enabled by default to help prevent too many simultaneous object deletions (more than 500 objects per synchronization).</span></span> <span data-ttu-id="11c4e-114">Tu postavku možete promijeniti tako da odgovara potrebama vaše tvrtke ili ustanove.</span><span class="sxs-lookup"><span data-stu-id="11c4e-114">You can change this setting to meet the needs of your organization.</span></span>

- <span data-ttu-id="11c4e-115">[Automatska nadogradnja](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) omogućena je prema zadanim postavkama za ekspresne instalacije i pomaže vam da vaša verzija usluge Azure AD Connect bude uvijek aktualna.</span><span class="sxs-lookup"><span data-stu-id="11c4e-115">[Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) is enabled by default for express installations and helps ensure your version of Azure AD Connect is always current.</span></span>
