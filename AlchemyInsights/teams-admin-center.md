---
title: Centar za administratore aplikacije Teams
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002890"
- "5542"
ms.openlocfilehash: bb0d757aab05132ff7169ce75009d7012b9a836c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670356"
---
# <a name="teams-admin-center"></a><span data-ttu-id="48732-102">Centar za administratore aplikacije Teams</span><span class="sxs-lookup"><span data-stu-id="48732-102">Teams Admin Center</span></span>

<span data-ttu-id="48732-103">Saznajte više o upravljanju aplikacijom Teams pomoću [centra za administratore aplikacije Teams](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).</span><span class="sxs-lookup"><span data-stu-id="48732-103">Learn about managing Teams with the [Teams Admin Center](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).</span></span>

<span data-ttu-id="48732-104">Ako ne možete pristupiti centru za administratore aplikacije Teams, provjerite sljedeće stavke:</span><span class="sxs-lookup"><span data-stu-id="48732-104">If you are unable to access the Teams Admin Center, please check the following items:</span></span>

- <span data-ttu-id="48732-105">Provjerite jeste li dopustili odgovarajuće [IP adrese i URL-ove sustava Office 365](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) na svim uređajima na vanjskoj crti obrane (vatrozidu itd.) ili u pravilima vatrozida na lokalnom računalu.</span><span class="sxs-lookup"><span data-stu-id="48732-105">Verify that you have allowed the appropriate [Office 365 IP addresses and URL's](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) on any perimeter devices (firewall, etc.) or in the firewall rules on your local machine.</span></span>
- <span data-ttu-id="48732-106">Provjerite odgovaraju li podaci za prijavu koje koristite za pristup portalu za administratore aplikacije Teams vašem korisničkom imenu na [portalu za administratore sustava Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span><span class="sxs-lookup"><span data-stu-id="48732-106">Verify that the login you are using to access the Teams Admin Portal matches your username listed in the [Microsoft 365 Admin portal](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span></span>

<span data-ttu-id="48732-107">Ako se u centru za administratore aplikacije Teams ne prikazuju korisnici, provjerite sljedeće:</span><span class="sxs-lookup"><span data-stu-id="48732-107">If users are not appearing in the Teams Admin Center, please check the following:</span></span>

- <span data-ttu-id="48732-108">Jeste li tijekom zadnja 24 sata stvarali korisnike ili dodjeljivali licence?</span><span class="sxs-lookup"><span data-stu-id="48732-108">Have you created users or assigned licenses in the last 24 hours?</span></span> <span data-ttu-id="48732-109">Pričekajte barem 24 sata prije nego što prijavite problem službi za podršku.</span><span class="sxs-lookup"><span data-stu-id="48732-109">Please make sure you wait at least 24 hours before opening a support ticket.</span></span>
- <span data-ttu-id="48732-110">Provjerite jeste li dodijelili odgovarajuće licence?</span><span class="sxs-lookup"><span data-stu-id="48732-110">Verify you have assigned appropriate licenses?</span></span>
- <span data-ttu-id="48732-111">Ako imate postojeći internetski direktorij, provjerite je li [vrijednost servisa msRTCSIP-PrimaryUserAddress ili SIP adresa u polju Proxyadrese u lokalnom aktivnom direktoriju jedinstvena, a oblikovanje odgovara](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) SIP-u:**korisničko ime** korisnika iz [centra za administratore sustava Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span><span class="sxs-lookup"><span data-stu-id="48732-111">If you have an on-premise Active Directory, verify that [the value of msRTCSIP-PrimaryUserAddress or the SIP address in the ProxyAddresses field in your local Active Directory is unique and the format matches](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) sip:**Username** of the user from the [Microsoft 365 admin center](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span></span>
- <span data-ttu-id="48732-112">Ako namjeravate zadržati implementaciju servisa Skype za tvrtke, a korisnici se nalaze na lokalnoj kartici i na internetu: slijedite gumb **"postavljanje hibridnih timova i Skypea za tvrtke online"** na upravljačkoj ploči servisa Skype za tvrtke i premještanje korisnika na internetu.</span><span class="sxs-lookup"><span data-stu-id="48732-112">If you intend to keep a Skype for Business Server deployment and have users homed on-premises and Online: follow the **"Set up hybrid with Teams and Skype for Business Online"** in your Skype for Business Server Control Panel and move users Online.</span></span>
