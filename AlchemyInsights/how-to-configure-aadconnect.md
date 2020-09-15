---
title: 646 kako konfigurirati AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "646"
- "1300023"
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 6327e42b74283d732247c9a847c68db72082c56a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47704481"
---
# <a name="configure-sync-features"></a><span data-ttu-id="50464-102">Konfiguriranje značajki sinkronizacije</span><span class="sxs-lookup"><span data-stu-id="50464-102">Configure sync features</span></span>

<span data-ttu-id="50464-103">Azure AD Connect sadrži nekoliko značajki koje su omogućene po zadanom ili koje možete omogućiti kasnije.</span><span class="sxs-lookup"><span data-stu-id="50464-103">Azure AD Connect includes several features that are enabled by default, or that you can enable later.</span></span> <span data-ttu-id="50464-104">Za neke je značajke potrebna dodatna konfiguracija u određenim okruženjima.</span><span class="sxs-lookup"><span data-stu-id="50464-104">Some features require additional configuration in specific environments.</span></span>

- <span data-ttu-id="50464-105">[Filtriranje](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) ograničava objekte sinkroniziraju s Azure AD.</span><span class="sxs-lookup"><span data-stu-id="50464-105">[Filtering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) limits the objects are synchronized to Azure AD.</span></span> <span data-ttu-id="50464-106">Po zadanom se sinkroniziraju svi korisnici, kontakti, grupe i računi računala sa sustavom Windows 10.</span><span class="sxs-lookup"><span data-stu-id="50464-106">By default, all users, contacts, groups, and Windows 10 computer accounts are synchronized.</span></span> <span data-ttu-id="50464-107">Objekte možete uvrstiti ili isključiti na temelju domena, tih ili drugih atributa.</span><span class="sxs-lookup"><span data-stu-id="50464-107">You can include or exclude objects based on domains, OUs, or other attributes.</span></span>

- <span data-ttu-id="50464-108">[Sinkronizacija zaporke za lozinke](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) sinkronizira dodatak za lozinke iz lokalnog servisa Active Directory na Azure AD.</span><span class="sxs-lookup"><span data-stu-id="50464-108">[Password hash synchronization](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synchronizes the password hash from the on-premises Active Directory to Azure AD.</span></span> <span data-ttu-id="50464-109">Time se omogućuje upravljanje lozinkama na jednom mjestu, no korištenje iste lozinke u lokalnim i okruženjima oblaka.</span><span class="sxs-lookup"><span data-stu-id="50464-109">This allows password management in one location, but use of the same password in both on-premises and cloud environments.</span></span> <span data-ttu-id="50464-110">Budući da je Active Directory Autoritativni izvor, možete koristiti vlastite pravilnike za lozinku.</span><span class="sxs-lookup"><span data-stu-id="50464-110">Because Active Directory is the authoritative source, you can use your own password policies.</span></span>

- <span data-ttu-id="50464-111">[Samoposlužno ponovno postavljanje lozinke (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) korisnicima omogućuje ponovno postavljanje vlastitih lozinki u oblaku dok se i dalje primjenjuje pravilnik o lozinci za lokalnu lozinku.</span><span class="sxs-lookup"><span data-stu-id="50464-111">[Self-service password reset (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) allows users to reset their own passwords in the cloud while still applying your on-premises password policy.</span></span>

- <span data-ttu-id="50464-112">[Nepotvrđenim uređaja](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) omogućuje pisanje registriranih uređaja u servisu Azure ad u lokalni aktivni direktorij da bi se mogli koristiti za uvjetni pristup.</span><span class="sxs-lookup"><span data-stu-id="50464-112">[Device writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) allows registered devices in Azure AD to be written back to the on-premises Active Directory so they can be used for conditional access.</span></span>

- <span data-ttu-id="50464-113">[Onemogućivanje slučajnog](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) brisanja po zadanom je omogućeno da bi se spriječilo previše brisanje istovremenih objekata (više od 500 objekata po sinkronizaciji).</span><span class="sxs-lookup"><span data-stu-id="50464-113">[Prevent accidental deletes](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) is enabled by default to help prevent too many simultaneous object deletions (more than 500 objects per synchronization).</span></span> <span data-ttu-id="50464-114">Tu postavku možete promijeniti tako da udovoljite potrebama tvrtke ili ustanove.</span><span class="sxs-lookup"><span data-stu-id="50464-114">You can change this setting to meet the needs of your organization.</span></span>

- <span data-ttu-id="50464-115">[Automatska nadogradnja](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) omogućena je prema zadanim postavkama za ekspresne instalacije te omogućuje da vaša verzija servisa Azure ad Connect uvijek bude aktivna.</span><span class="sxs-lookup"><span data-stu-id="50464-115">[Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) is enabled by default for express installations and helps ensure your version of Azure AD Connect is always current.</span></span>
