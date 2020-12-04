---
title: Otklanjanje poteškoća s izdankom PRT
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/01/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000076"
- "7317"
ms.openlocfilehash: 8e654a38d720aa51daf21bf5c3fb0da8b9c3d8e7
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573380"
---
# <a name="troubleshoot-prt-issue"></a><span data-ttu-id="87114-102">Otklanjanje poteškoća s izdankom PRT</span><span class="sxs-lookup"><span data-stu-id="87114-102">Troubleshoot PRT issue</span></span>

<span data-ttu-id="87114-103">Da bi bilo koji uređaj trebao biti autentičan, mora biti u potpunosti registriran i u dobroj državi i može steći primarni token osvježavanja (PRT).</span><span class="sxs-lookup"><span data-stu-id="87114-103">For any device to complete getting authenticated, it must be fully registered and in good state and able to acquire a Primary Refresh Token (PRT).</span></span>

<span data-ttu-id="87114-104">Postupak registracije za hibridnu verziju Azure AD Join zahtijeva da uređaji budu na korporacijskom mreži.</span><span class="sxs-lookup"><span data-stu-id="87114-104">The hybrid Azure AD join registration process requires devices to be on a corporate network.</span></span> <span data-ttu-id="87114-105">Internet isto tako utvrde na VPN, ali ima neki opomena to taj.</span><span class="sxs-lookup"><span data-stu-id="87114-105">It also works over VPN but there are some caveats to that.</span></span> <span data-ttu-id="87114-106">Čuli smo da kupci trebaju pomoć pri otklanjanju poteškoća s postupkom registracije hibridne Azure AD Join u odjeljku uvjeti daljinskog rada.</span><span class="sxs-lookup"><span data-stu-id="87114-106">We’ve heard customers needing assistance with troubleshooting the hybrid Azure AD join registration process under remote-work circumstances.</span></span> <span data-ttu-id="87114-107">Ovdje se nalazi slom događaja "Under The Hood" tijekom postupka registracije.</span><span class="sxs-lookup"><span data-stu-id="87114-107">Here’s a breakdown of what’s happening ‘under the hood’ during the registration process.</span></span>

<span data-ttu-id="87114-108">**Okruženje za provjeru autentičnosti u oblaku (korištenje značajke korištenja lozinke za Azure AD i provjera autentičnosti)**</span><span class="sxs-lookup"><span data-stu-id="87114-108">**Cloud authentication environment (using Azure AD password hash sync or pass-through authentication)**</span></span>

<span data-ttu-id="87114-109">Ovaj tijek registracije poznat je i kao "Sinkronizacija pridruživanja".</span><span class="sxs-lookup"><span data-stu-id="87114-109">This registration flow is also known as “Sync Join”.</span></span>

1. <span data-ttu-id="87114-110">Windows 10 otkriva zapis o SCP-u na korisniku koji se prijavljuje na uređaj.</span><span class="sxs-lookup"><span data-stu-id="87114-110">Windows 10 discovers an SCP record upon user logging on to the device.</span></span>
    1. <span data-ttu-id="87114-111">Uređaj najprije pokuša dohvatiti informacije o klijentu s klijentskog SCP-a u registru [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span><span class="sxs-lookup"><span data-stu-id="87114-111">The device first tries to retrieve tenant information from client-side SCP in registry [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span></span> <span data-ttu-id="87114-112">Dodatne informacije potražite u ovom [dokumentu](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).</span><span class="sxs-lookup"><span data-stu-id="87114-112">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).</span></span>
    2. <span data-ttu-id="87114-113">Ako ne uspije, uređaj komunicira s lokalnim servisom Active Directory (AD) da bi dobio informacije o klijentu iz točke veze za servis (SCP).</span><span class="sxs-lookup"><span data-stu-id="87114-113">If it fails, the device communicates with on-premises Active Directory (AD) to get tenant information from Service Connection Point (SCP).</span></span> <span data-ttu-id="87114-114">Da biste potvrdili SCP, pogledajte ovaj [dokument](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span><span class="sxs-lookup"><span data-stu-id="87114-114">To verify SCP, please refer to this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span></span> 

> [!NOTE]
> <span data-ttu-id="87114-115">Preporučujemo vam da u OGLASU omogućite SCP, a za početnu provjeru valjanosti koristite samo SKP na strani klijenta.</span><span class="sxs-lookup"><span data-stu-id="87114-115">We recommend enabling SCP in the AD and only using client-side SCP for initial validation.</span></span>

2. <span data-ttu-id="87114-116">Windows 10 pokušava razgovarati s Azure AD u odjeljku sistemski kontekst radi provjere autentičnosti za Azure AD.</span><span class="sxs-lookup"><span data-stu-id="87114-116">Windows 10 tries to communicate with Azure AD under the system context to authenticate itself against Azure AD.</span></span> <span data-ttu-id="87114-117">Možete potvrditi može li uređaj pristupati Microsoftovim resursima u odjeljku sistemski račun pomoću skripte za povezivanje s registriranjem testnog uređaja.</span><span class="sxs-lookup"><span data-stu-id="87114-117">You can verify if the device can access Microsoft resources under the system account by using the Test Device Registration Connectivity script.</span></span>

3. <span data-ttu-id="87114-118">Windows 10 generira samopotpisani certifikat i pohranjuje ga ispod objekta računala u lokalnom AD-u.</span><span class="sxs-lookup"><span data-stu-id="87114-118">Windows 10 generates a self-signed certificate and stores it under the computer object in on-premises AD.</span></span> <span data-ttu-id="87114-119">Za to je potreban kontrolor domene.</span><span class="sxs-lookup"><span data-stu-id="87114-119">This requires line-of-sight to Domain Controller.</span></span>

4. <span data-ttu-id="87114-120">Objekt uređaja s certifikatom može se sinkronizirati s programom Azure AD putem servisa Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="87114-120">A device object that has a certificate gets synchronized to Azure AD via Azure AD Connect.</span></span> <span data-ttu-id="87114-121">Ciklus sinkronizacije svaki je 30 minuta po zadanom, ali ovisi o konfiguraciji servisa Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="87114-121">Sync cycle is every 30 minutes by default, but it depends on configuration of Azure AD Connect.</span></span> <span data-ttu-id="87114-122">Dodatne informacije potražite u ovom [dokumentu](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).</span><span class="sxs-lookup"><span data-stu-id="87114-122">For more information, please refer to this [document](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).</span></span>

5. <span data-ttu-id="87114-123">U ovoj će fazi biti moguće vidjeti predmet uređaja u odjeljku "u tijeku" u odjeljku sprava Blade of Azure portal.</span><span class="sxs-lookup"><span data-stu-id="87114-123">At this stage, you should be able to see the subject device in “Pending” state under Device blade of Azure Portal.</span></span>

6. <span data-ttu-id="87114-124">Kada se sljedeći korisnik prijavi na Windows 10, registracija će biti dovršena.</span><span class="sxs-lookup"><span data-stu-id="87114-124">At the next user login to Windows 10, the registration will be completed.</span></span> 

> [!NOTE]
> <span data-ttu-id="87114-125">Ako ste na VPN-u, a ako je postupak prijave neograničen, možete ručno pokrenuti registraciju:</span><span class="sxs-lookup"><span data-stu-id="87114-125">If you're on VPN and a logoff-login process terminates the domain connectivity, you can trigger registration manually:</span></span>
 1. <span data-ttu-id="87114-126">Izdanje dsregcmd/pridružite se lokalno na administratorskom upitu ili na daljinu putem Psexez-a na PC.</span><span class="sxs-lookup"><span data-stu-id="87114-126">Issue a dsregcmd /join locally on admin prompt or remotely via PSExec to your PC.</span></span> <span data-ttu-id="87114-127">Na primjer, Psexez-s \\ win10client01 cmd, dsregcmd/Join</span><span class="sxs-lookup"><span data-stu-id="87114-127">For example, PsExec -s \\win10client01 cmd, dsregcmd /join</span></span>

 2. <span data-ttu-id="87114-128">Dodatne informacije o hibridnim pitanjima pridruživanja potražite u članku [Otklanjanje poteškoća s uređajima](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344).</span><span class="sxs-lookup"><span data-stu-id="87114-128">For more details on Hybrid Join issues, see [Troubleshoot devices Issue](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344).</span></span>
