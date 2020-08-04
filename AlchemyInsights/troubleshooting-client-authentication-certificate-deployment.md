---
title: Otklanjanje poteškoća s implementacijom certifikata za provjeru autentičnosti klijenta
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
- "1546"
- "9000076"
ms.openlocfilehash: 698329d7705af320c9f679b92532b58ac84e6624
ms.sourcegitcommit: e90b918f02102cd9764881c2d8c914567c6b070e
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 07/29/2020
ms.locfileid: "46554787"
---
# <a name="troubleshooting-client-authentication-certificate-deployment"></a><span data-ttu-id="47970-102">Otklanjanje poteškoća s implementacijom certifikata za provjeru autentičnosti klijenta</span><span class="sxs-lookup"><span data-stu-id="47970-102">Troubleshooting Client Authentication certificate deployment</span></span>

<span data-ttu-id="47970-103">Intune NDES/SCEP i PKCS/PFX Klijentski certifikati profili se obično koriste u kombinaciji s drugim vrstama profila kao što su WiFi, VPN i e-pošta kako bi se korisnicima omogućilo provjeru autentičnosti korporativnih resursa.</span><span class="sxs-lookup"><span data-stu-id="47970-103">Intune NDES/SCEP and PKCS/PFX Client certificates profiles are commonly used in conjunction with other profiles types such as Wifi, VPN, and email to allow users to authenticate to corporate resources.</span></span> <span data-ttu-id="47970-104">Kada su te vrste profila povezane s profilom certifikata klijenta ovise o uspješnoj implementaciji tog profila.</span><span class="sxs-lookup"><span data-stu-id="47970-104">When those profile types are linked to a client certificate profile are dependant on the successful deployment of that profile.</span></span>

<span data-ttu-id="47970-105">Početno postavljanje infrastrukture i pridružena konfiguracija profila klijentske potvrde često zahtijevaju otklanjanje poteškoća.</span><span class="sxs-lookup"><span data-stu-id="47970-105">Initial infrastructure setup and associated configuration of the Client Certificate profile often require troubleshooting.</span></span> <span data-ttu-id="47970-106">Detaljni vodič za uspješno postavljanje NDES priključka i upute za otklanjanje poteškoća za izoliranje problema s implementacijom certifikata potražite u članku:</span><span class="sxs-lookup"><span data-stu-id="47970-106">For a step-by-step guide to successful setup of the NDES connector and troubleshooting guidance to isolate issues with certificate deployment, see:</span></span> 

- [<span data-ttu-id="47970-107">Konfiguriranje infrastrukture za podršku SKEP-a s Intuneom</span><span class="sxs-lookup"><span data-stu-id="47970-107">Configure infrastructure to support SCEP with Intune</span></span>](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [<span data-ttu-id="47970-108">Pregled otklanjanja poteškoća s profilima certifikata SCEP-a pomoću programa Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="47970-108">Overview for troubleshooting SCEP certificate profiles with Microsoft Intune</span></span>](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

<span data-ttu-id="47970-109">Pomoću referencišenih skripti ljuske powershell provjerite konfiguraciju.</span><span class="sxs-lookup"><span data-stu-id="47970-109">Use the referenced powershell scripts to help verify your configuration.</span></span> <span data-ttu-id="47970-110">Dodatne informacije [potražite u odjeljku Skripte za provjeru poveznika certifikata intune](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).</span><span class="sxs-lookup"><span data-stu-id="47970-110">For more info, see [Intune Certificate connector verification scripts](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).</span></span>

  
<span data-ttu-id="47970-111">**Ostala uobičajena pitanja**</span><span class="sxs-lookup"><span data-stu-id="47970-111">**Other common issues**</span></span>

<span data-ttu-id="47970-112">**Našto JA pokušati uvesti koga u službu Intune izdati svjedodžbu povezivanje na NDES povezivanje poslužitelj, JA dobiti poruka, " lozinka in izdati svjedodžbu molba ne moći biti verified. Možda je već korišten. Nabavite novu lozinku za slanje s ovim zahtjevom."**</span><span class="sxs-lookup"><span data-stu-id="47970-112">**When I try to install the Intune certificate connector on the NDES connector server, I get the message, "The password in the certificate request cannot be verified. It may have been used already. Obtain a new password to submit with this request."**</span></span>  

<span data-ttu-id="47970-113">Ova poruka znači da morate pokrenuti instalaciju poveznika certifikata kao administrator.</span><span class="sxs-lookup"><span data-stu-id="47970-113">This message means that you need to run the certificate connector installation as an Administrator.</span></span>

<span data-ttu-id="47970-114">U nekim okruženjima poslužitelji na kojima se izvodi Intune certifikat moraju koristiti proxy poslužitelj za povezivanje s intuneom pa poveznik certifikata mora koristiti proxy.</span><span class="sxs-lookup"><span data-stu-id="47970-114">In some environments, the servers where the Intune Certificate runs must use a proxy server to connect to Intune, and so the Certificate Connector must use a proxy.</span></span> <span data-ttu-id="47970-115">U nekim okolnostima NDES Connector zanemaruje konfigurirane postavke proxy poslužitelja i možda će biti potrebno konfigurirati postavke proxy poslužitelja tijekom pokretanja u sigurnosnom kontekstu LocalSystema.</span><span class="sxs-lookup"><span data-stu-id="47970-115">In some circumstances, the NDES Connector ignores the configured proxy settings, and it might be necessary to configure the proxy settings while running in the security context of LocalSystem.</span></span> 
 
<span data-ttu-id="47970-116">rješenje će biti trčanje Internet explorer kao SISTEM i konfiguracijski proksiji in IE.</span><span class="sxs-lookup"><span data-stu-id="47970-116">The solution is to run Internet Explorer as SYSTEM and configure a proxy in IE.</span></span> <span data-ttu-id="47970-117">Nakon ponovnog pokretanja servisa Intune Connector, NDES priključak povezuje se s intune.</span><span class="sxs-lookup"><span data-stu-id="47970-117">After a restart of the Intune Connector Service, the NDES Connector connects to Intune.</span></span>

<span data-ttu-id="47970-118">**Korisnički uređaji više ne primaju SCEP certifikate iz NDES-a.**</span><span class="sxs-lookup"><span data-stu-id="47970-118">**User devices are no longer receiving SCEP certificates from NDES.**</span></span>

<span data-ttu-id="47970-119">Moguće je da je certifikat za provjeru autentičnosti klijenta izdan ndes poslužitelju i naveden tijekom instalacije NDES priključka istekao ili nedostaje.</span><span class="sxs-lookup"><span data-stu-id="47970-119">It is possible that the Client Authentication certificate issued to the NDES server, and specified during the NDES connector installation, has expired or is missing.</span></span> <span data-ttu-id="47970-120">Da biste riješili problem:</span><span class="sxs-lookup"><span data-stu-id="47970-120">To resolve:</span></span> 
 
1. <span data-ttu-id="47970-121">Deinstalirajte NDES poveznik.</span><span class="sxs-lookup"><span data-stu-id="47970-121">Uninstall the NDES connector.</span></span>  
2. <span data-ttu-id="47970-122">Koristite ove pojedinosti da biste zatražili novu provjeru autentičnosti klijenta ili certifikat za provjeru autentičnosti poslužitelja:</span><span class="sxs-lookup"><span data-stu-id="47970-122">Use these details to request a new client authentication or server authentication certificate:</span></span> 
 
    - <span data-ttu-id="47970-123">Naziv predmeta: CN=vanjski fqdn</span><span class="sxs-lookup"><span data-stu-id="47970-123">Subject name: CN=external fqdn</span></span>  
    - <span data-ttu-id="47970-124">Alternativni naziv predmeta (oba su obavezna): DNS=vanjski fqdn, DNS=interni fqdn</span><span class="sxs-lookup"><span data-stu-id="47970-124">Subject alternative name (both are required): DNS=external fqdn, DNS=internal fqdn</span></span> 
 
3. <span data-ttu-id="47970-125">Ponovno instalirajte NDES priključak s novim certifikatom.</span><span class="sxs-lookup"><span data-stu-id="47970-125">Reinstall the NDES connector with the new certificate.</span></span>