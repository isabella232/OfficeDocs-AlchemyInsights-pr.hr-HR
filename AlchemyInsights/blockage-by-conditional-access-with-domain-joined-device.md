---
title: Blokira mi se uvjetni pristup pomoću uređaja za priključene domene
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/20/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9834"
- "9003257"
ms.openlocfilehash: 052311ffe71bcb65de2b5c2a964932b1fb99c373
ms.sourcegitcommit: c34ba92e19419dcb2d251b8a1afe4d180a939617
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/20/2021
ms.locfileid: "51035233"
---
# <a name="im-getting-blocked-by-conditional-access-with-domain-joined-device"></a><span data-ttu-id="7e14c-102">Blokira mi se uvjetni pristup pomoću uređaja za priključene domene</span><span class="sxs-lookup"><span data-stu-id="7e14c-102">I’m getting blocked by Conditional Access with domain joined device</span></span>

<span data-ttu-id="7e14c-103">**Visoko preporučeni Alati**</span><span class="sxs-lookup"><span data-stu-id="7e14c-103">**Highly Recommended Tools**</span></span>

<span data-ttu-id="7e14c-104">[Alat za otklanjanje poteškoća s registracijom uređaja](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) – alat koji olakšava otklanjanje poteškoća s najčešćih problema s registracijom uređaja.</span><span class="sxs-lookup"><span data-stu-id="7e14c-104">[Device Registration Troubleshooter Tool](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) - The tool that helps in troubleshooting the most common device registration issues.</span></span>

<span data-ttu-id="7e14c-105">[Testna skripta za povezivanje s uređajem za registraciju](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) – skripta koja omogućuje pristup krajnjim točkama registracije uređaja u odjeljku sistemski račun.</span><span class="sxs-lookup"><span data-stu-id="7e14c-105">[Test Device Registration Connectivity script](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) - The script that helps ensuring that a device can access Device Registration endpoints under the system account.</span></span>

<span data-ttu-id="7e14c-106">[Skripta za čišćenje servisa Azure ad](https://github.com/mzmaili/AzureADDeviceCleanup) -skripta koja omogućuje traženje i upravljanje ustajalim uređajima u vašem okruženju.</span><span class="sxs-lookup"><span data-stu-id="7e14c-106">[Azure AD Device Cleanup Script](https://github.com/mzmaili/AzureADDeviceCleanup) - The script that enables you to seek and manage stale devices in your environment.</span></span>

<span data-ttu-id="7e14c-107">Evo nekoliko običnih razloga zbog kojih uvjetni pristup možda ne uspijeva na uređaju koji se pridružio domeni (Hybrid Azure AD).</span><span class="sxs-lookup"><span data-stu-id="7e14c-107">Here are some common reasons why conditional access may be failing a device that has joined a domain (Hybrid Azure AD).</span></span>

1. <span data-ttu-id="7e14c-108">**Na uređaju nema servisa Azure ad PRT** , morate osigurati da uređaj ima token za primarni osvježavanje za Azure AD (prt).</span><span class="sxs-lookup"><span data-stu-id="7e14c-108">**There’s no Azure AD PRT on the device** - You need to ensure that the device has Azure AD Primary Refresh Token (PRT).</span></span> <span data-ttu-id="7e14c-109">Dodatne informacije o PRT-u potražite u ovom [dokumentu](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).</span><span class="sxs-lookup"><span data-stu-id="7e14c-109">For more information about PRT, see this [document](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).</span></span>

<span data-ttu-id="7e14c-110">Da biste provjerili imate li Azure AD PRT, možete pokrenuti `dsregcmd/status` naredbu na uređaju i provjeriti je li "AzureAdPrt" jednako "da".</span><span class="sxs-lookup"><span data-stu-id="7e14c-110">To verify if you have Azure AD PRT, you can run `dsregcmd/status` command on the device and verify if “AzureAdPrt” equals “YES”.</span></span>

<span data-ttu-id="7e14c-111">Ako je "AzureAdPrt" "ne", provjerite sljedeće:</span><span class="sxs-lookup"><span data-stu-id="7e14c-111">If "AzureAdPrt" is "NO", check the following:</span></span>

- <span data-ttu-id="7e14c-112">Bez obzira na to imate li **udruženu okolinu sa programom AD FS, a nedostupna je iz kućnih mreža vaših korisnika**: u ovom slučaju provjerite jesu li krajnje točke "usernazivno" podijeljene u programu extranet dostupne.</span><span class="sxs-lookup"><span data-stu-id="7e14c-112">**Whether you have a federated environment with AD FS, and it’s unreachable from your users’ home networks**: In this case, ensure that your "usernamemixed" endpoints are accessible from the extranet.</span></span> <span data-ttu-id="7e14c-113">Ako je vaš AD FS iza VPN-a, pobrinite se da se korisnici povezuju s VPN-om i ponovno se prijave na uređaj.</span><span class="sxs-lookup"><span data-stu-id="7e14c-113">If your AD FS is behind a VPN, ensure that the users connect to the VPN and re-login to the device.</span></span> <span data-ttu-id="7e14c-114">Dodatne informacije potražite u ovom [dokumentu](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains).</span><span class="sxs-lookup"><span data-stu-id="7e14c-114">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains).</span></span>

- <span data-ttu-id="7e14c-115">**Bez obzira na to je li TPM neispravan i time ne može potvrditi autentičnost uređaja**: Potvrdite "TPM. msc" da biste provjerili je li stanje TPM-a "spremno".</span><span class="sxs-lookup"><span data-stu-id="7e14c-115">**Whether the device’s TPM is faulty and thus cannot authenticate the device**: Check "tpm.msc" to see if the state of TPM is "Ready".</span></span> <span data-ttu-id="7e14c-116">Ako ne, pokrenite `dsregcmd/leave` i pustite da se uređaj ponovno pridruži Azure ad-u.</span><span class="sxs-lookup"><span data-stu-id="7e14c-116">If not, run `dsregcmd/leave` and let the device re-join to Azure AD.</span></span> <span data-ttu-id="7e14c-117">Zatim pokušajte ponovno.</span><span class="sxs-lookup"><span data-stu-id="7e14c-117">Then, try again.</span></span> <span data-ttu-id="7e14c-118">Dodatne informacije potražite u ovom [dokumentu](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).</span><span class="sxs-lookup"><span data-stu-id="7e14c-118">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).</span></span>

- <span data-ttu-id="7e14c-119">**Koristite davatelja usluge trećih strana, koji ne podržava WS-Trust Protocol**.</span><span class="sxs-lookup"><span data-stu-id="7e14c-119">**You’re using a 3rd party identity provider, which does not support WS-Trust protocol**.</span></span> <span data-ttu-id="7e14c-120">Kao što je opisano u našim dokumentima, Hybrid Azure AD-pridruženi uređaji ne mogu raditi u ovom slučaju.</span><span class="sxs-lookup"><span data-stu-id="7e14c-120">As described in our docs, hybrid Azure AD-joined devices cannot work in this case.</span></span> <span data-ttu-id="7e14c-121">Suradite s pružateljem identiteta radi podrške.</span><span class="sxs-lookup"><span data-stu-id="7e14c-121">Please work with your Identity provider for support.</span></span>

2. <span data-ttu-id="7e14c-122">**Korisnici koriste preglednik Chrome bez računa sustava Windows 10** ili **ekstenzije sustava Office Chrome ne koristi automatski prt na AAD-u ili HIBRIDNU-AAD-kompatibilnim uređajima**: to dovodi do neuspjeha bilo koje pravilnike o uvjetnom pristupu utemeljenoj na uređaju, s prikazanim porukama o pogrešci "neregistrirani uređaj".</span><span class="sxs-lookup"><span data-stu-id="7e14c-122">**Users are using Chrome browser without the Windows 10 Accounts** or **Office extension Chrome does not automatically use the PRT on AAD-joined or hybrid-AAD-joined devices**: This leads to failure of any device-based Conditional Access policies, with “Unregistered device” error message displayed.</span></span> <span data-ttu-id="7e14c-123">Da biste ispravno koristili preglednik Chrome, morate instalirati "računi u sustavu Windows 10" ili "ekstenziju sustava Office u pregledniku Chrome" Via SCCM ili Intune.</span><span class="sxs-lookup"><span data-stu-id="7e14c-123">To use Chrome browser correctly, you must install the “Windows 10 Accounts” or "Office extension to the users’ Chrome browser" via SCCM or Intune.</span></span> <span data-ttu-id="7e14c-124">Dodatne informacije potražite u ovom [dokumentu](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support).</span><span class="sxs-lookup"><span data-stu-id="7e14c-124">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support).</span></span>

<span data-ttu-id="7e14c-125">Ako nije moguće pritisnuti daljinsko proširenje, obavijestite korisnike da ručno instaliraju neku od navedenih proširenja da bi pristupili aplikacijama iza uvjetnog pristupa utemeljenog na uređaju.</span><span class="sxs-lookup"><span data-stu-id="7e14c-125">If it’s not possible to push the extension remotely, notify users to manually install one of the above extensions to access applications behind device-based Conditional Access.</span></span> <span data-ttu-id="7e14c-126">Dodatne informacije potražite u ovom [dokumentu](https://docs.microsoft.com/azure/active-directory/conditional-access/require-managed-devices#prerequisites).</span><span class="sxs-lookup"><span data-stu-id="7e14c-126">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/conditional-access/require-managed-devices#prerequisites).</span></span>

3. <span data-ttu-id="7e14c-127">**Uređaj je ispravno spojen hibridni Azure AD, ali je nehotice izbrisano ili onemogućeno, bilo zbog sinkronizacije promjena u servisu Azure ad Connect ili s portala Azure**: ako se to dogodi, objekt Device više nije prepoznat kao potpuno spojeni uređaj, iako se status "Azureadconnector" i "prt" prikazuje kao valjano na uređaju.</span><span class="sxs-lookup"><span data-stu-id="7e14c-127">**The device was correctly hybrid Azure AD joined, but it was inadvertently deleted or disabled, either due to sync changes in Azure AD Connect or from the Azure portal**: If this happens, the device object is no longer recognized as a fully joined device even though the "AzureAdJoined" and "PRT" status show up as valid on the device.</span></span>

<span data-ttu-id="7e14c-128">Da biste riješili taj problem, pokrenite se `dsregcmd/leave` na pogođenim uređajima i pustite ih da se vrate u Azure AD.</span><span class="sxs-lookup"><span data-stu-id="7e14c-128">To fix this issue, run `dsregcmd/leave` on the affected devices and let them rejoin Azure AD.</span></span> <span data-ttu-id="7e14c-129">Dodatne informacije potražite u ovom [dokumentu](https://docs.microsoft.com/azure/active-directory/devices/faq#q-why-do-my-users-see-an-error-message-saying-your-organization-has-deleted-the-device-or-your-organization-has-disabled-the-device-on-their-windows-10-devices).</span><span class="sxs-lookup"><span data-stu-id="7e14c-129">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/faq#q-why-do-my-users-see-an-error-message-saying-your-organization-has-deleted-the-device-or-your-organization-has-disabled-the-device-on-their-windows-10-devices).</span></span>

> [!NOTE]
> <span data-ttu-id="7e14c-130">Ako su vaši uređaji u sustavu Windows 10, 1809 Update, uz VPN/Cloud proxy i pogledajte probleme s stanjem "AzureAdPrt" ili bilo kojom aplikacijom sa sustavom SSO (Outlook ne povezuje se s poštanskim sandučićem iako ste imali PRT), provjerite imate li tu zakrpu [KB4554354](https://support.microsoft.com/topic/march-30-2020-kb4554354-os-build-17763-1132-deaba49b-4b29-55b9-caee-3e2d87dd75a2) ili Travanj Kumulativno ažuriranje [KB4549949](https://support.microsoft.com/topic/april-14-2020-kb4549949-os-build-17763-1158-76d9a3af-b20b-8996-bd4d-7b50c505fda6) da biste spriječili pogreške prt-a na tim uređajima.</span><span class="sxs-lookup"><span data-stu-id="7e14c-130">If your devices are on Windows 10, 1809 update, with VPN/Cloud Proxy and see issues with "AzureAdPrt" state or any app with SSO problem (outlook not connecting to mailbox even though you had PRT), ensure you have this patch [KB4554354](https://support.microsoft.com/topic/march-30-2020-kb4554354-os-build-17763-1132-deaba49b-4b29-55b9-caee-3e2d87dd75a2) or April cumulative update [KB4549949](https://support.microsoft.com/topic/april-14-2020-kb4549949-os-build-17763-1158-76d9a3af-b20b-8996-bd4d-7b50c505fda6) to prevent PRT failures on those machines.</span></span>

















