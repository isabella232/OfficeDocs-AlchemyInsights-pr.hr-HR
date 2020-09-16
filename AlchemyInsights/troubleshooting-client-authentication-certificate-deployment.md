---
title: Otklanjanje poteškoća s implementacijom certifikata provjere autentičnosti klijenta
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
- "1546"
- "9000076"
ms.openlocfilehash: cecbd091447e63f2d5012ceaf96e050c92a171e6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658978"
---
# <a name="troubleshooting-client-authentication-certificate-deployment"></a><span data-ttu-id="41f0a-102">Otklanjanje poteškoća s implementacijom certifikata provjere autentičnosti klijenta</span><span class="sxs-lookup"><span data-stu-id="41f0a-102">Troubleshooting Client Authentication certificate deployment</span></span>

<span data-ttu-id="41f0a-103">U kombinaciji s drugim vrstama profila, kao što su WiFi, VPN i e-pošte, profili za klijentske certifikate i PKCS/PFX korisnici obično se koriste u vezi s drugim oblicima na servisu Wi</span><span class="sxs-lookup"><span data-stu-id="41f0a-103">Intune NDES/SCEP and PKCS/PFX Client certificates profiles are commonly used in conjunction with other profiles types such as Wifi, VPN, and email to allow users to authenticate to corporate resources.</span></span> <span data-ttu-id="41f0a-104">Kada su te vrste profila povezane s profilom klijentskog certifikata, ovise o uspješnoj implementaciji tog profila.</span><span class="sxs-lookup"><span data-stu-id="41f0a-104">When those profile types are linked to a client certificate profile are dependant on the successful deployment of that profile.</span></span>

<span data-ttu-id="41f0a-105">Početno postavljanje infrastrukture i povezana konfiguracija profila klijentskog certifikata često je potrebno otklanjanje poteškoća.</span><span class="sxs-lookup"><span data-stu-id="41f0a-105">Initial infrastructure setup and associated configuration of the Client Certificate profile often require troubleshooting.</span></span> <span data-ttu-id="41f0a-106">Detaljne upute za uspješan postavljanje programa NDES Connector i uputa za otklanjanje poteškoća radi izoliranje problema s implementacijom certifikata potražite u članku:</span><span class="sxs-lookup"><span data-stu-id="41f0a-106">For a step-by-step guide to successful setup of the NDES connector and troubleshooting guidance to isolate issues with certificate deployment, see:</span></span> 

- [<span data-ttu-id="41f0a-107">Konfiguriranje infrastrukture radi podrške za SCEP uz Intune</span><span class="sxs-lookup"><span data-stu-id="41f0a-107">Configure infrastructure to support SCEP with Intune</span></span>](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [<span data-ttu-id="41f0a-108">Pregled radi otklanjanja poteškoća s profilima certifikata u programu Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="41f0a-108">Overview for troubleshooting SCEP certificate profiles with Microsoft Intune</span></span>](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

<span data-ttu-id="41f0a-109">Pomoću referentne skripte za PowerShell možete provjeriti konfiguraciju.</span><span class="sxs-lookup"><span data-stu-id="41f0a-109">Use the referenced powershell scripts to help verify your configuration.</span></span> <span data-ttu-id="41f0a-110">Dodatne informacije potražite u članku umetanje [skripti za provjeru povezivanja certifikata](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).</span><span class="sxs-lookup"><span data-stu-id="41f0a-110">For more info, see [Intune Certificate connector verification scripts](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).</span></span>

  
<span data-ttu-id="41f0a-111">**Ostali česti problemi**</span><span class="sxs-lookup"><span data-stu-id="41f0a-111">**Other common issues**</span></span>

<span data-ttu-id="41f0a-112">**Kada pokušam instalirati konektor certifikata na poslužitelj NDES Connector, dobivam poruku: "lozinka u zahtjevu za certifikatom nije moguće provjeriti. Možda je već korišten. Nabavite novu lozinku koju ćete poslati ovim zahtjevom. "**</span><span class="sxs-lookup"><span data-stu-id="41f0a-112">**When I try to install the Intune certificate connector on the NDES connector server, I get the message, "The password in the certificate request cannot be verified. It may have been used already. Obtain a new password to submit with this request."**</span></span>  

<span data-ttu-id="41f0a-113">Ova poruka znači da morate pokrenuti instalaciju poveznika certifikata kao administratora.</span><span class="sxs-lookup"><span data-stu-id="41f0a-113">This message means that you need to run the certificate connector installation as an Administrator.</span></span>

<span data-ttu-id="41f0a-114">U nekim okruženjima poslužitelji na kojima se izvršava dodatak certifikata moraju koristiti proxy poslužitelj da bi se povezali s Intune, pa povezivanje s certifikatom mora koristiti proxy.</span><span class="sxs-lookup"><span data-stu-id="41f0a-114">In some environments, the servers where the Intune Certificate runs must use a proxy server to connect to Intune, and so the Certificate Connector must use a proxy.</span></span> <span data-ttu-id="41f0a-115">U nekim okolnostima NDES konektor ignorira konfigurirane postavke proxyja i možda će biti potrebno konfigurirati postavke proxyja tijekom izvođenja u sigurnosnom kontekstu LocalSystem.</span><span class="sxs-lookup"><span data-stu-id="41f0a-115">In some circumstances, the NDES Connector ignores the configured proxy settings, and it might be necessary to configure the proxy settings while running in the security context of LocalSystem.</span></span> 
 
<span data-ttu-id="41f0a-116">Rješenje je pokretanje preglednika Internet Explorer kao sustava i konfiguriranje proxyja u programu IE.</span><span class="sxs-lookup"><span data-stu-id="41f0a-116">The solution is to run Internet Explorer as SYSTEM and configure a proxy in IE.</span></span> <span data-ttu-id="41f0a-117">Nakon ponovnog pokretanja servisa Intune Connector, NDES konektor povezuje se s Intune.</span><span class="sxs-lookup"><span data-stu-id="41f0a-117">After a restart of the Intune Connector Service, the NDES Connector connects to Intune.</span></span>

<span data-ttu-id="41f0a-118">**Korisnički uređaji više ne dobivaju certifikate za SCEP iz NDES-a.**</span><span class="sxs-lookup"><span data-stu-id="41f0a-118">**User devices are no longer receiving SCEP certificates from NDES.**</span></span>

<span data-ttu-id="41f0a-119">Moguće je da je certifikat za provjeru autentičnosti klijenta izdan na poslužitelju NDES, a naveden tijekom instalacije NDES konektora istekao ili nedostaje.</span><span class="sxs-lookup"><span data-stu-id="41f0a-119">It is possible that the Client Authentication certificate issued to the NDES server, and specified during the NDES connector installation, has expired or is missing.</span></span> <span data-ttu-id="41f0a-120">Da biste riješili sljedeće:</span><span class="sxs-lookup"><span data-stu-id="41f0a-120">To resolve:</span></span> 
 
1. <span data-ttu-id="41f0a-121">Deinstalirajte NDES konektor.</span><span class="sxs-lookup"><span data-stu-id="41f0a-121">Uninstall the NDES connector.</span></span>  
2. <span data-ttu-id="41f0a-122">Koristite ove pojedinosti da biste zatražili novu provjeru autentičnosti klijenta ili certifikat za provjeru autentičnosti poslužitelja:</span><span class="sxs-lookup"><span data-stu-id="41f0a-122">Use these details to request a new client authentication or server authentication certificate:</span></span> 
 
    - <span data-ttu-id="41f0a-123">Naziv predmeta: CN = vanjski FQDN</span><span class="sxs-lookup"><span data-stu-id="41f0a-123">Subject name: CN=external fqdn</span></span>  
    - <span data-ttu-id="41f0a-124">Zamjenski naziv predmeta (oba su obavezna): DNS = vanjski FQDN, DNS = Internal FQDN</span><span class="sxs-lookup"><span data-stu-id="41f0a-124">Subject alternative name (both are required): DNS=external fqdn, DNS=internal fqdn</span></span> 
 
3. <span data-ttu-id="41f0a-125">Ponovno instalirajte NDES konektor s novim certifikatom.</span><span class="sxs-lookup"><span data-stu-id="41f0a-125">Reinstall the NDES connector with the new certificate.</span></span>