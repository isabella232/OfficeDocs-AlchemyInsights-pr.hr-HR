---
title: Intune Wi-Fi profili
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1548"
- "9000076"
ms.openlocfilehash: afc8142a635b8a9d715eb4325b570be20ad26645
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696253"
---
# <a name="intune-wi-fi-profiles"></a><span data-ttu-id="a4857-102">Intune Wi-Fi profili</span><span class="sxs-lookup"><span data-stu-id="a4857-102">Intune Wi-Fi profiles</span></span>

<span data-ttu-id="a4857-103">Uspješna implementacija Wi-Fi veze za klijente MDM-a ovisi o pravilno raspoređeni profil koji odražava preduvjete korporativnih Wi-Fi infrastrukture.</span><span class="sxs-lookup"><span data-stu-id="a4857-103">Successful implementation of Wi-Fi connectivity for MDM clients depends on a correctly deployed profile that reflects the requirements of the corporate Wi-Fi infrastructure.</span></span> <span data-ttu-id="a4857-104">Da biste pregledali odgovarajuće postavke za klijentske platforme koje istražujete, pročitajte sljedeće:</span><span class="sxs-lookup"><span data-stu-id="a4857-104">To review the appropriate settings for the client platforms you are investigating, see:</span></span> 

[<span data-ttu-id="a4857-105">Dodavanje Wi-Fi postavki za uređaje sa sustavom Android u programu Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="a4857-105">Add Wi-Fi settings for devices running Android in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-android)

[<span data-ttu-id="a4857-106">Dodavanje Wi-Fi postavki za tvrtke sa sustavom Android i potpuno upravljanih uređaja u programu Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="a4857-106">Add Wi-Fi settings for Android Enterprise dedicated and fully managed devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-android-enterprise)

[<span data-ttu-id="a4857-107">Dodavanje Wi-Fi postavki za uređaje sa sustavom iOS i iPadOS u programu Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="a4857-107">Add Wi-Fi settings for iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-ios)

[<span data-ttu-id="a4857-108">Dodavanje Wi-Fi postavki za uređaje sa sustavom Windows 10 i novije verzije u programu Intune</span><span class="sxs-lookup"><span data-stu-id="a4857-108">Add Wi-Fi settings for Windows 10 and later devices in Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-windows)

[<span data-ttu-id="a4857-109">Uvoz Wi-Fi postavki za uređaje sa sustavom Windows u programu Intune</span><span class="sxs-lookup"><span data-stu-id="a4857-109">Import Wi-Fi settings for Windows devices in Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-import-windows-8-1)

<span data-ttu-id="a4857-110">**Česti problemi**</span><span class="sxs-lookup"><span data-stu-id="a4857-110">**Common Issues**</span></span>

<span data-ttu-id="a4857-111">**Implementiram Wi-Fi profil koji ovisi o raspoređenim certifikatu navedenom u profilu Wi-Fi. No profili za konfiguraciju prikazuju status pogreške.**</span><span class="sxs-lookup"><span data-stu-id="a4857-111">**I'm deploying a Wi-Fi profile that is dependent on a deployed certificate specified in the Wi-Fi profile. However, the configuration profiles are showing an error status.**</span></span>

<span data-ttu-id="a4857-112">Provjerite je li vaš uređaj primio certifikat.</span><span class="sxs-lookup"><span data-stu-id="a4857-112">Check that your device received the certificate.</span></span>

1. <span data-ttu-id="a4857-113">U programu Intune otvorite **sve uređaje** i odaberite uređaj > **konfiguraciji uređaja**.</span><span class="sxs-lookup"><span data-stu-id="a4857-113">In Intune, go to **All Devices** and select the device > **Device configuration**.</span></span>

2. <span data-ttu-id="a4857-114">Provjerite jesu li svi očekivani profili navedeni i u uspješnom stanju.</span><span class="sxs-lookup"><span data-stu-id="a4857-114">Check that all expected profiles are listed and in a successful state.</span></span>

3. <span data-ttu-id="a4857-115">Ako imate profil za Android, ako imate posredne certifikate u lancu certifikata, provjerite jesu li razmješteni na uređaje sa sustavom Android.</span><span class="sxs-lookup"><span data-stu-id="a4857-115">For an Android profile, if you have intermediate certificates in your certificate chain, make sure they are deployed to Android devices.</span></span>

    <span data-ttu-id="a4857-116">Da biste provjerili status certifikata, idite na **profile konfiguracije uređaja**  >  **Profiles**  >  **Android Intermedijarni**  >  **Properties**  >  **certifikat**za svojstva.</span><span class="sxs-lookup"><span data-stu-id="a4857-116">To check the certificate status, go to **Device configuration** > **Profiles** > **Android intermediate CA** > **Properties** > **Trusted Certificate**.</span></span>

<span data-ttu-id="a4857-117">Ako i dalje vidite pogreške, pregledajte procedure i sekcije otklanjanja poteškoća.</span><span class="sxs-lookup"><span data-stu-id="a4857-117">If you continue to see errors, review the procedures and troubleshooting sections.</span></span> <span data-ttu-id="a4857-118">Dodatne informacije potražite u članku [Pregled rješenja otklanjanja poteškoća s profilima certifikata u programu Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="a4857-118">For more info, see [Overview for troubleshooting SCEP certificate profiles with Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune).</span></span>

<span data-ttu-id="a4857-119">**Rasporedio sam Wi-Fi profil na uređaj. Intune pokazuje da je bila uspješna, no uređaj se ne povezuje s Wi-Fi-jem.**</span><span class="sxs-lookup"><span data-stu-id="a4857-119">**I deployed a Wi-Fi profile to a device. Intune is showing that it was successful, but the device is not connecting to the Wi-Fi.**</span></span>

<span data-ttu-id="a4857-120">Uspješan status znači da je Intune uspješno implementirao profil kao konfiguriran.</span><span class="sxs-lookup"><span data-stu-id="a4857-120">A successful status means that Intune has successfully deployed the profile as configured.</span></span> <span data-ttu-id="a4857-121">No te se konfiguracije možda neće podudarati s vašim zahtjevima za mrežu i/ili provjeru autentičnosti.</span><span class="sxs-lookup"><span data-stu-id="a4857-121">However, these configurations might not match your network and/or authentication requirements.</span></span> <span data-ttu-id="a4857-122">Dodatne informacije o pokusaju veze potražite u evidenciji za infrastrukturu i provjeru autentičnosti (na kontroleru za Wi-Fi Access Point i NPS/radius Server).</span><span class="sxs-lookup"><span data-stu-id="a4857-122">For more details about the attempted connection, review logs in the infrastructure and authentication service (on the Wi-Fi Access point controller and NPS/Radius server).</span></span> <span data-ttu-id="a4857-123">Možda ćete morati raditi s tim mrežnim infrastrukturom ili drugim dobavljačima wi-fija, da biste prikupili i pregledavali zapisnike.</span><span class="sxs-lookup"><span data-stu-id="a4857-123">You might have to work with your network infrastructure team, or the third-party Wi-Fi vendor, to gather and review logs.</span></span>