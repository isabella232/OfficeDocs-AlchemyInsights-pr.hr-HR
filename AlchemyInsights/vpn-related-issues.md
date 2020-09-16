---
title: Problemi povezani s VPN-om
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
- "1545"
- "9000076"
ms.openlocfilehash: 3c031725c92f5d7af7c0dd0c37ea34fecf4792c8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47726083"
---
# <a name="vpn-related-issues"></a><span data-ttu-id="146f2-102">Problemi povezani s VPN-om</span><span class="sxs-lookup"><span data-stu-id="146f2-102">VPN related issues</span></span>

<span data-ttu-id="146f2-103">Uspješna implementacija VPN povezivosti za klijente MDM-a zavisi od raspoređenih profila koji pravilno odražava zahtjeve VPN infrastrukture.</span><span class="sxs-lookup"><span data-stu-id="146f2-103">Successful implementation of VPN connectivity for MDM clients depends on a deployed profile that correctly reflects the requirements of the VPN infrastructure.</span></span> <span data-ttu-id="146f2-104">Odgovarajuće postavke za klijentsku platformu koju istražujete potražite u članku:</span><span class="sxs-lookup"><span data-stu-id="146f2-104">For the appropriate settings for the client platforms you are investigating, see:</span></span> 

[<span data-ttu-id="146f2-105">Windows 10 i Windows holo-postavke uređaja za dodavanje VPN veza pomoću aplikacije Intune</span><span class="sxs-lookup"><span data-stu-id="146f2-105">Windows 10 and Windows Holographic device settings to add VPN connections using Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-windows-10)  
[<span data-ttu-id="146f2-106">Dodavanje VPN postavki na uređajima sa sustavom iOS i iPadOS u programu Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="146f2-106">Add VPN settings on iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-ios)  
[<span data-ttu-id="146f2-107">Postavke uređaja sa sustavom Android da biste konfigurirali VPN u programu Intune</span><span class="sxs-lookup"><span data-stu-id="146f2-107">Android device settings to configure VPN in Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-android)  
[<span data-ttu-id="146f2-108">Dodavanje VPN postavki na uređajima macOS u programu Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="146f2-108">Add VPN settings on macOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/mem/intune/configuration/vpn-settings-macos)

<span data-ttu-id="146f2-109">Ako vaš VPN profil koristi provjeru autentičnosti utemeljenu na certifikatu, provjerite jesu li korijenski certifikat i profili certifikata za provjeru autentičnosti povezani s VPN profilom uspješno razmješteni.</span><span class="sxs-lookup"><span data-stu-id="146f2-109">If your VPN profile uses certificate based authentication, make sure that the root certificate and client authentication certificate profiles linked to the VPN profile are deployed successfully.</span></span>

<span data-ttu-id="146f2-110">**Česti problemi**</span><span class="sxs-lookup"><span data-stu-id="146f2-110">**Common Issues**</span></span>

<span data-ttu-id="146f2-111">**Rasporedio sam VPN profil na uređaj. Intune pokazuje da je bila uspješna, no uređaj se ne povezuje s VPN-ovim.**</span><span class="sxs-lookup"><span data-stu-id="146f2-111">**I deployed a VPN profile to a device. Intune is showing that it was successful, but the device is not connecting to the VPN.**</span></span>

<span data-ttu-id="146f2-112">Uspješan status znači da je Intune uspješno implementirao profil kao konfiguriran.</span><span class="sxs-lookup"><span data-stu-id="146f2-112">A successful status means that Intune has successfully deployed the profile as configured.</span></span> <span data-ttu-id="146f2-113">No te se konfiguracije možda neće podudarati s vašim zahtjevima za mrežu i/ili provjeru autentičnosti.</span><span class="sxs-lookup"><span data-stu-id="146f2-113">However, these configurations might not match your network and/or authentication requirements.</span></span> <span data-ttu-id="146f2-114">Pregled zapisnika u servisu za infrastrukturu i provjeru autentičnosti (na poslužitelju VPN poslužitelja i NPS/radius Server) dodatne informacije o pokusaju povezivanja.</span><span class="sxs-lookup"><span data-stu-id="146f2-114">Review logs in the infrastructure and authentication service (on the VPN server and NPS/Radius server) for more details about the attempted connection.</span></span> <span data-ttu-id="146f2-115">Možda ćete morati raditi s tim mrežnim infrastrukturom ili drugim proizvođačima VPN-a, da biste prikupili i pregledavali zapisnike.</span><span class="sxs-lookup"><span data-stu-id="146f2-115">You might need to work with your network infrastructure team, or the third-party VPN vendor, to gather and review logs.</span></span>

<span data-ttu-id="146f2-116">**Kada Konfiguriram prilagođeni VPN za iOS, značajka VPN-a po aplikaciji nije dostupna.**</span><span class="sxs-lookup"><span data-stu-id="146f2-116">**When I configure a custom VPN for iOS, the per-app VPN feature isn't made available.**</span></span>

<span data-ttu-id="146f2-117">VPN-ovi za uređaje sa sustavom iOS u programu Intune na aplikaciji trenutno su dostupni određenom popisu pružatelja usluga i partnera, koji moraju zadovoljiti preduvjete certifikata prije konfiguriranja VPN-a po aplikaciji.</span><span class="sxs-lookup"><span data-stu-id="146f2-117">Per-app VPN for iOS devices in Intune is currently available to a specific list of providers and partners, who must also meet the certificate prerequisites before configuring a per-app VPN.</span></span> <span data-ttu-id="146f2-118">Dodatne informacije potražite u članku [Postavljanje virtualne privatne mreže (VPN-a) za iOS/iPadOS uređaje u aplikaciji Intune](https://docs.microsoft.com/intune/vpn-setting-configure-per-app).</span><span class="sxs-lookup"><span data-stu-id="146f2-118">For more info, see [Set up per-app Virtual Private Network (VPN) for iOS/iPadOS devices in Intune](https://docs.microsoft.com/intune/vpn-setting-configure-per-app).</span></span> 

<span data-ttu-id="146f2-119">Dodatne informacije o svim vrstama VPN veza u programu Intune potražite u članku [Stvaranje VPN profila za povezivanje s VPN poslužiteljima u programu Intune](https://docs.microsoft.com/intune/vpn-settings-configure).</span><span class="sxs-lookup"><span data-stu-id="146f2-119">For more info about all VPN connection types in Intune, see [Create VPN profiles to connect to VPN servers in Intune](https://docs.microsoft.com/intune/vpn-settings-configure).</span></span>  

<span data-ttu-id="146f2-120">**VPN na servisu iOS na zahtjev ne pokreće se kada se pristupi konfiguriranoj domeni**</span><span class="sxs-lookup"><span data-stu-id="146f2-120">**iOS On-Demand VPN is not triggering when a configured domain is accessed**</span></span>

<span data-ttu-id="146f2-121">Da biste testirali automatske VPN postavke, postavite sljedeće vrijednosti:</span><span class="sxs-lookup"><span data-stu-id="146f2-121">To test automatic VPN settings, set the following values:</span></span>

<span data-ttu-id="146f2-122">Želim učiniti sljedeće: **procijeniti svaki pokušaj povezivanja**</span><span class="sxs-lookup"><span data-stu-id="146f2-122">I want to do the following: **Evaluate each connection attempt**</span></span> 

<span data-ttu-id="146f2-123">Odaberite želite li se povezati: **povezivanje ako je potrebno**</span><span class="sxs-lookup"><span data-stu-id="146f2-123">Choose whether to connect: **Connect if needed**</span></span>

<span data-ttu-id="146f2-124">Kada korisnici pristupe ovim domenama: **Odredišni** *naziv domene*</span><span class="sxs-lookup"><span data-stu-id="146f2-124">When users access these domains: **target** *domain name*</span></span>

<span data-ttu-id="146f2-125">Ako gore navedena konfiguracija nije uspješna, dodajte sljedeći element:</span><span class="sxs-lookup"><span data-stu-id="146f2-125">If the above configuration is not successful, add the following element:</span></span>

<span data-ttu-id="146f2-126">Kada taj URL nije dostupan, silom povežite VPN: **Badurl**</span><span class="sxs-lookup"><span data-stu-id="146f2-126">When this URL is unreachable, force connect the VPN: **BADURL**</span></span>