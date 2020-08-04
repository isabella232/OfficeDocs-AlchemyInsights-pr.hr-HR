---
title: Intune Wi-Fi profili
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1548"
- "9000076"
ms.openlocfilehash: e5e1007abadb8ddb30ca110d465131ec791e44b7
ms.sourcegitcommit: e90b918f02102cd9764881c2d8c914567c6b070e
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 07/29/2020
ms.locfileid: "46554857"
---
# <a name="intune-wi-fi-profiles"></a><span data-ttu-id="32288-102">Intune Wi-Fi profili</span><span class="sxs-lookup"><span data-stu-id="32288-102">Intune Wi-Fi profiles</span></span>

<span data-ttu-id="32288-103">Uspješna implementacija Wi-Fi veze za MDM klijente ovisi o ispravno uvedenom profilu koji odražava zahtjeve korporacijske Wi-Fi infrastrukture.</span><span class="sxs-lookup"><span data-stu-id="32288-103">Successful implementation of Wi-Fi connectivity for MDM clients depends on a correctly deployed profile that reflects the requirements of the corporate Wi-Fi infrastructure.</span></span> <span data-ttu-id="32288-104">Da biste pregledali odgovarajuće postavke za klijentske platforme koje istražujete, pogledajte:</span><span class="sxs-lookup"><span data-stu-id="32288-104">To review the appropriate settings for the client platforms you are investigating, see:</span></span> 

[<span data-ttu-id="32288-105">Dodavanje Wi-Fi postavki za uređaje sa sustavom Android u programu Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="32288-105">Add Wi-Fi settings for devices running Android in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-android)

[<span data-ttu-id="32288-106">Dodavanje Wi-Fi postavki za android enterprise namjenske i potpuno upravljane uređaje u programu Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="32288-106">Add Wi-Fi settings for Android Enterprise dedicated and fully managed devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-android-enterprise)

[<span data-ttu-id="32288-107">Dodavanje Wi-Fi postavki za iOS i iPadOS uređaje u sustavu Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="32288-107">Add Wi-Fi settings for iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-ios)

[<span data-ttu-id="32288-108">Dodavanje Wi-Fi postavki za Windows 10 i novije uređaje u aplikaciji Intune</span><span class="sxs-lookup"><span data-stu-id="32288-108">Add Wi-Fi settings for Windows 10 and later devices in Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-windows)

[<span data-ttu-id="32288-109">Uvoz Wi-Fi postavki za uređaje sa sustavom Windows u intune</span><span class="sxs-lookup"><span data-stu-id="32288-109">Import Wi-Fi settings for Windows devices in Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-import-windows-8-1)

<span data-ttu-id="32288-110">**Uobičajena pitanja**</span><span class="sxs-lookup"><span data-stu-id="32288-110">**Common Issues**</span></span>

<span data-ttu-id="32288-111">**Uvodim Wi-Fi profil koji ovisi o implementiranom certifikatu navedenom u Wi-Fi profilu. Međutim, konfiguracijski profili prikazuju status pogreške.**</span><span class="sxs-lookup"><span data-stu-id="32288-111">**I'm deploying a Wi-Fi profile that is dependent on a deployed certificate specified in the Wi-Fi profile. However, the configuration profiles are showing an error status.**</span></span>

<span data-ttu-id="32288-112">Provjerite je li uređaj primio certifikat.</span><span class="sxs-lookup"><span data-stu-id="32288-112">Check that your device received the certificate.</span></span>

1. <span data-ttu-id="32288-113">U odjeljku Intune idite na **Svi uređaji** i odaberite uređaj > **konfiguracija uređaja**.</span><span class="sxs-lookup"><span data-stu-id="32288-113">In Intune, go to **All Devices** and select the device > **Device configuration**.</span></span>

2. <span data-ttu-id="32288-114">Provjerite jesu li navedeni svi očekivani profili i u uspješnom stanju.</span><span class="sxs-lookup"><span data-stu-id="32288-114">Check that all expected profiles are listed and in a successful state.</span></span>

3. <span data-ttu-id="32288-115">Za Android profil, ako imate međurezultate u lancu certifikata, provjerite jesu li implementirani na Android uređaje.</span><span class="sxs-lookup"><span data-stu-id="32288-115">For an Android profile, if you have intermediate certificates in your certificate chain, make sure they are deployed to Android devices.</span></span>

    <span data-ttu-id="32288-116">Da biste provjerili status certifikata, idite na **Profili za konfiguraciju uređaja**  >  **Profiles**  >  **Android srednji CA**  >  **Properties**  >  **Svojstva Pouzdani certifikat**.</span><span class="sxs-lookup"><span data-stu-id="32288-116">To check the certificate status, go to **Device configuration** > **Profiles** > **Android intermediate CA** > **Properties** > **Trusted Certificate**.</span></span>

<span data-ttu-id="32288-117">Ako se pogreškama i dalje prikazuje, pregledajte odjeljke za postupke i otklanjanje poteškoća.</span><span class="sxs-lookup"><span data-stu-id="32288-117">If you continue to see errors, review the procedures and troubleshooting sections.</span></span> <span data-ttu-id="32288-118">Dodatne informacije potražite u [odjeljku Pregled otklanjanja poteškoća s profilima certifikata SCEP-a pomoću programa Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="32288-118">For more info, see [Overview for troubleshooting SCEP certificate profiles with Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune).</span></span>

<span data-ttu-id="32288-119">**Implementirao sam Wi-Fi profil na uređaj. Intune pokazuje da je bio uspješan, ali uređaj se ne povezuje s Wi-Fi.**</span><span class="sxs-lookup"><span data-stu-id="32288-119">**I deployed a Wi-Fi profile to a device. Intune is showing that it was successful, but the device is not connecting to the Wi-Fi.**</span></span>

<span data-ttu-id="32288-120">Uspješan status znači da je Intune uspješno uveo profil kao konfiguriran.</span><span class="sxs-lookup"><span data-stu-id="32288-120">A successful status means that Intune has successfully deployed the profile as configured.</span></span> <span data-ttu-id="32288-121">Međutim, te konfiguracije možda ne odgovaraju vašim zahtjevima mreže i/ili provjere autentičnosti.</span><span class="sxs-lookup"><span data-stu-id="32288-121">However, these configurations might not match your network and/or authentication requirements.</span></span> <span data-ttu-id="32288-122">Dodatne informacije o pokušaju povezivanja pregledajte zapisnike u infrastrukturi i servisu za provjeru autentičnosti (na kontroleru točke Wi-Fi pristup i NPS/Radius poslužitelju).</span><span class="sxs-lookup"><span data-stu-id="32288-122">For more details about the attempted connection, review logs in the infrastructure and authentication service (on the Wi-Fi Access point controller and NPS/Radius server).</span></span> <span data-ttu-id="32288-123">Možda ćete morati surađivati s timom za mrežnu infrastrukturu ili dobavljačem Wi-Fi-ja treće strane da biste prikupili i pregledali zapisnike.</span><span class="sxs-lookup"><span data-stu-id="32288-123">You might have to work with your network infrastructure team, or the third-party Wi-Fi vendor, to gather and review logs.</span></span>