---
title: Problemi povezani s VPN-om
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
- "1545"
- "9000076"
ms.openlocfilehash: 134d78f30216dfd268c5999a5032b7d7ad1d7dd8
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 07/28/2020
ms.locfileid: "46554773"
---
# <a name="vpn-related-issues"></a><span data-ttu-id="497c4-102">Problemi povezani s VPN-om</span><span class="sxs-lookup"><span data-stu-id="497c4-102">VPN related issues</span></span>

<span data-ttu-id="497c4-103">Uspješna implementacija VPN veze za MDM klijente ovisi o implementiranom profilu koji ispravno odražava zahtjeve VPN infrastrukture.</span><span class="sxs-lookup"><span data-stu-id="497c4-103">Successful implementation of VPN connectivity for MDM clients depends on a deployed profile that correctly reflects the requirements of the VPN infrastructure.</span></span> <span data-ttu-id="497c4-104">Za odgovarajuće postavke za klijentske platforme koje istražujete potražite u članku:</span><span class="sxs-lookup"><span data-stu-id="497c4-104">For the appropriate settings for the client platforms you are investigating, see:</span></span> 

[<span data-ttu-id="497c4-105">Postavke uređaja Windows 10 i Windows Holografski za dodavanje VPN veza pomoću aplikacije Intune</span><span class="sxs-lookup"><span data-stu-id="497c4-105">Windows 10 and Windows Holographic device settings to add VPN connections using Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-windows-10)  
[<span data-ttu-id="497c4-106">Dodavanje VPN postavki na iOS i iPadOS uređajima u programu Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="497c4-106">Add VPN settings on iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-ios)  
[<span data-ttu-id="497c4-107">Postavke Android uređaja za konfiguriranje VPN-a u intune</span><span class="sxs-lookup"><span data-stu-id="497c4-107">Android device settings to configure VPN in Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-android)  
[<span data-ttu-id="497c4-108">Dodavanje VPN postavki na macOS uređajima u programu Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="497c4-108">Add VPN settings on macOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/mem/intune/configuration/vpn-settings-macos)

<span data-ttu-id="497c4-109">Ako vaš VPN profil koristi provjeru autentičnosti na temelju certifikata, provjerite jesu li korijenski certifikat i profili certifikata za provjeru autentičnosti klijenta povezani s VPN profilom uspješno uvedeni.</span><span class="sxs-lookup"><span data-stu-id="497c4-109">If your VPN profile uses certificate based authentication, make sure that the root certificate and client authentication certificate profiles linked to the VPN profile are deployed successfully.</span></span>

<span data-ttu-id="497c4-110">**Uobičajena pitanja**</span><span class="sxs-lookup"><span data-stu-id="497c4-110">**Common Issues**</span></span>

<span data-ttu-id="497c4-111">**Implementirao sam VPN profil na uređaj. Intune pokazuje da je bio uspješan, ali uređaj se ne povezuje s VPN-om.**</span><span class="sxs-lookup"><span data-stu-id="497c4-111">**I deployed a VPN profile to a device. Intune is showing that it was successful, but the device is not connecting to the VPN.**</span></span>

<span data-ttu-id="497c4-112">Uspješan status znači da je Intune uspješno uveo profil kao konfiguriran.</span><span class="sxs-lookup"><span data-stu-id="497c4-112">A successful status means that Intune has successfully deployed the profile as configured.</span></span> <span data-ttu-id="497c4-113">Međutim, te konfiguracije možda ne odgovaraju vašim zahtjevima mreže i/ili provjere autentičnosti.</span><span class="sxs-lookup"><span data-stu-id="497c4-113">However, these configurations might not match your network and/or authentication requirements.</span></span> <span data-ttu-id="497c4-114">Pregledajte zapisnike u infrastrukturi i servisu za provjeru autentičnosti (na VPN poslužitelju i NPS/Radius poslužitelju) za više pojedinosti o pokušaju povezivanja.</span><span class="sxs-lookup"><span data-stu-id="497c4-114">Review logs in the infrastructure and authentication service (on the VPN server and NPS/Radius server) for more details about the attempted connection.</span></span> <span data-ttu-id="497c4-115">Možda ćete morati surađivati s timom za mrežnu infrastrukturu ili dobavljačem VPN-a treće strane da biste prikupili i pregledali zapisnike.</span><span class="sxs-lookup"><span data-stu-id="497c4-115">You might need to work with your network infrastructure team, or the third-party VPN vendor, to gather and review logs.</span></span>

<span data-ttu-id="497c4-116">**Kada konfiguriram prilagođeni VPN za iOS, vpn značajka po aplikaciji nije dostupna.**</span><span class="sxs-lookup"><span data-stu-id="497c4-116">**When I configure a custom VPN for iOS, the per-app VPN feature isn't made available.**</span></span>

<span data-ttu-id="497c4-117">VPN po aplikaciji za iOS uređaje u aplikaciji Intune trenutno je dostupan na određenom popisu davatelja i partnera, koji također moraju ispuniti preduvjete certifikata prije konfiguriranja VPN-a po aplikaciji.</span><span class="sxs-lookup"><span data-stu-id="497c4-117">Per-app VPN for iOS devices in Intune is currently available to a specific list of providers and partners, who must also meet the certificate prerequisites before configuring a per-app VPN.</span></span> <span data-ttu-id="497c4-118">Dodatne informacije [potražite u odjeljku Postavljanje virtualne privatne mreže (VPN) po aplikaciji za iOS/iPadOS uređaje u aplikaciji Intune](https://docs.microsoft.com/intune/vpn-setting-configure-per-app).</span><span class="sxs-lookup"><span data-stu-id="497c4-118">For more info, see [Set up per-app Virtual Private Network (VPN) for iOS/iPadOS devices in Intune](https://docs.microsoft.com/intune/vpn-setting-configure-per-app).</span></span> 

<span data-ttu-id="497c4-119">Dodatne informacije o svim vrstama VPN veza u intune potražite u [odjeljku Stvaranje VPN profila za povezivanje s VPN poslužiteljima u intune](https://docs.microsoft.com/intune/vpn-settings-configure).</span><span class="sxs-lookup"><span data-stu-id="497c4-119">For more info about all VPN connection types in Intune, see [Create VPN profiles to connect to VPN servers in Intune](https://docs.microsoft.com/intune/vpn-settings-configure).</span></span>  

<span data-ttu-id="497c4-120">**IOS on-Demand VPN ne pokreće kada se pristupa konfiguriranoj domeni**</span><span class="sxs-lookup"><span data-stu-id="497c4-120">**iOS On-Demand VPN is not triggering when a configured domain is accessed**</span></span>

<span data-ttu-id="497c4-121">Da biste testirali automatske POSTAVKE VPN-a, postavite sljedeće vrijednosti:</span><span class="sxs-lookup"><span data-stu-id="497c4-121">To test automatic VPN settings, set the following values:</span></span>

<span data-ttu-id="497c4-122">Želim učiniti sljedeće: **Procijenite svaki pokušaj povezivanja**</span><span class="sxs-lookup"><span data-stu-id="497c4-122">I want to do the following: **Evaluate each connection attempt**</span></span> 

<span data-ttu-id="497c4-123">Odaberite želite li se povezati: **Povežite se ako je potrebno**</span><span class="sxs-lookup"><span data-stu-id="497c4-123">Choose whether to connect: **Connect if needed**</span></span>

<span data-ttu-id="497c4-124">Kada korisnici pristupaju tim domenama: **ciljni** *naziv domene*</span><span class="sxs-lookup"><span data-stu-id="497c4-124">When users access these domains: **target** *domain name*</span></span>

<span data-ttu-id="497c4-125">Ako gore navedena konfiguracija nije uspješna, dodajte sljedeći element:</span><span class="sxs-lookup"><span data-stu-id="497c4-125">If the above configuration is not successful, add the following element:</span></span>

<span data-ttu-id="497c4-126">Kada je ovaj URL nedostupan, prisilno povežite VPN: **BADURL**</span><span class="sxs-lookup"><span data-stu-id="497c4-126">When this URL is unreachable, force connect the VPN: **BADURL**</span></span>