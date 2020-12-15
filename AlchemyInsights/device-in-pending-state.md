---
title: Uređaj u stanju na čekanju
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003244"
- "7319"
ms.openlocfilehash: f70b43a8b914b0d2dda9db61606b8ae24523f869
ms.sourcegitcommit: 097a8cabe0d2280af489159789988a0ab532dabb
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 12/11/2020
ms.locfileid: "49677137"
---
# <a name="device-in-pending-state"></a><span data-ttu-id="4aa0d-102">Uređaj u stanju na čekanju</span><span class="sxs-lookup"><span data-stu-id="4aa0d-102">Device in pending state</span></span>

<span data-ttu-id="4aa0d-103">**Preduvjeti**</span><span class="sxs-lookup"><span data-stu-id="4aa0d-103">**Prerequisites:**</span></span>

1. <span data-ttu-id="4aa0d-104">Ako prvi put postavljate registracije uređaja, provjerite jeste li pregledali [Uvod u upravljanje uređajima u servisu Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) koji će vas voditi na način na koji možete nabaviti uređaje u odjeljku kontrola Azure AD.</span><span class="sxs-lookup"><span data-stu-id="4aa0d-104">If you are setting up device registrations for the first time, please ensure that you have reviewed [Introduction to device management in Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) that will guide you on how to get devices under the control of Azure AD.</span></span>
2. <span data-ttu-id="4aa0d-105">Ako izravno registrirate uređaje u Azure AD i postavite ih u Intune, morat ćete se pobrinuti da ste [konfigurirali Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) i da prvo imate [licenciranje](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) .</span><span class="sxs-lookup"><span data-stu-id="4aa0d-105">If you are registering devices into Azure AD directly and enrolling them into Intune, you will need to ensure that you have [configured Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) and have the [licensing](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) in place first.</span></span>
3. <span data-ttu-id="4aa0d-106">Provjerite jeste li ovlašteni za izvršavanje operacija u Azure AD i lokalnom AD-u.</span><span class="sxs-lookup"><span data-stu-id="4aa0d-106">Ensure you are authorized to perform operations in Azure AD and on-premises AD.</span></span> <span data-ttu-id="4aa0d-107">Samo globalni administrator u servisu Azure AD može upravljati postavkama za registraciju uređaja.</span><span class="sxs-lookup"><span data-stu-id="4aa0d-107">Only a global administrator in Azure AD can manage settings for device registrations.</span></span> <span data-ttu-id="4aa0d-108">Osim toga, ako postavljate automatske registracije u lokalnom servisu Active Directory, morat ćete biti administrator servisa Active Directory i AD FS (ako je primjenjivo).</span><span class="sxs-lookup"><span data-stu-id="4aa0d-108">In addition, if you are setting up automatic registrations in your on-premises Active Directory, you will need to be an administrator of Active Directory and AD FS (if applicable).</span></span>

<span data-ttu-id="4aa0d-109">Postupak registracije za hibridnu verziju Azure AD Join zahtijeva uređaje za korporacijsku mrežu.</span><span class="sxs-lookup"><span data-stu-id="4aa0d-109">The hybrid Azure AD join registration process requires devices to be on corporate network.</span></span> <span data-ttu-id="4aa0d-110">Internet isto tako utvrde na VPN, ali ima neki opomena to taj.</span><span class="sxs-lookup"><span data-stu-id="4aa0d-110">It also works over VPN but there are some caveats to that.</span></span> <span data-ttu-id="4aa0d-111">Čuli smo da kupci trebaju pomoć pri otklanjanju poteškoća s postupkom registracije hibridne Azure AD Join u odjeljku udaljeni uvjeti rada.</span><span class="sxs-lookup"><span data-stu-id="4aa0d-111">We have heard customers needing assistance with troubleshooting the hybrid Azure AD join registration process under remote work circumstances.</span></span>

<span data-ttu-id="4aa0d-112">**Okruženje za provjeru autentičnosti u oblaku (korištenje značajke korištenja lozinke za Azure AD i provjera autentičnosti)**</span><span class="sxs-lookup"><span data-stu-id="4aa0d-112">**Cloud authentication environment (using Azure AD password hash sync or pass-through authentication)**</span></span>

<span data-ttu-id="4aa0d-113">Ovaj tijek registracije poznat je i kao "Sinkronizacija pridruživanja".</span><span class="sxs-lookup"><span data-stu-id="4aa0d-113">This registration flow is also known as “Sync Join”.</span></span>

<span data-ttu-id="4aa0d-114">Ovdje se nalazi kvar u tijeku postupka registracije:</span><span class="sxs-lookup"><span data-stu-id="4aa0d-114">Here is a breakdown of what happens during the registration process:</span></span>

1. <span data-ttu-id="4aa0d-115">Windows 10 otkriva točku povezivanja servisa (SCP) kada se korisnik prijavljuje na uređaj.</span><span class="sxs-lookup"><span data-stu-id="4aa0d-115">Windows 10 discovers Service Connection Point (SCP) record when the user logs on to the device.</span></span>

    1. <span data-ttu-id="4aa0d-116">Uređaj najprije pokuša dohvatiti informacije o klijentu s klijentskog SCP-a u registru [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span><span class="sxs-lookup"><span data-stu-id="4aa0d-116">The device first tries to retrieve tenant information from client-side SCP in registry [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span></span> <span data-ttu-id="4aa0d-117">Dodatne informacije potražite u članku [dokument](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).</span><span class="sxs-lookup"><span data-stu-id="4aa0d-117">For more information, see [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).</span></span>
    1. <span data-ttu-id="4aa0d-118">Ako ne uspije, uređaj komunicira s lokalnim programom Active Directory radi nabavljanje informacija o klijentu iz programa SCP.</span><span class="sxs-lookup"><span data-stu-id="4aa0d-118">If it fails, the device communicates with on-premises Active Directory to get tenant information from SCP.</span></span> <span data-ttu-id="4aa0d-119">Da biste potvrdili SCP, obratite se ovom [dokumentu](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span><span class="sxs-lookup"><span data-stu-id="4aa0d-119">To verify SCP, refer this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span></span>

    > [!NOTE]
    > <span data-ttu-id="4aa0d-120">Preporučujemo da u aktivnom direktoriju omogućite SCP, a za početnu provjeru valjanosti koristite samo SKP za klijentski dio.</span><span class="sxs-lookup"><span data-stu-id="4aa0d-120">We recommend enabling SCP in the Active Directory and only using client-side SCP for initial validation.</span></span>

2. <span data-ttu-id="4aa0d-121">Windows 10 pokušava razgovarati s Azure AD u odjeljku sistemski kontekst radi provjere autentičnosti za Azure AD.</span><span class="sxs-lookup"><span data-stu-id="4aa0d-121">Windows 10 tries to communicate with Azure AD under the system context to authenticate itself against Azure AD.</span></span>

    <span data-ttu-id="4aa0d-122">Možete potvrditi može li uređaj pristupati Microsoftovim resursima u odjeljku sistemski račun pomoću skripte za povezivanje s [registriranjem testnog uređaja](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0).</span><span class="sxs-lookup"><span data-stu-id="4aa0d-122">You can verify if the device can access Microsoft resources under the system account by using the [Test Device Registration Connectivity script](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0).</span></span>

3. <span data-ttu-id="4aa0d-123">Windows 10 generira samopotpisani certifikat i pohranjuje ga u objekt računala u lokalnom servisu Active Directory.</span><span class="sxs-lookup"><span data-stu-id="4aa0d-123">Windows 10 generates self-signed certificate and stores it under the computer object in on-premises Active Directory.</span></span> <span data-ttu-id="4aa0d-124">Za to je potreban kontrolor domene.</span><span class="sxs-lookup"><span data-stu-id="4aa0d-124">This requires line-of-sight to Domain Controller.</span></span>

4. <span data-ttu-id="4aa0d-125">Objekt uređaja s certifikatom može se sinkronizirati s programom Azure AD putem servisa Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="4aa0d-125">Device object that has certificate gets synchronized to Azure AD via Azure AD Connect.</span></span> <span data-ttu-id="4aa0d-126">Ciklus sinkronizacije svaki je 30 minuta po zadanom, ali ovisi o konfiguraciji servisa Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="4aa0d-126">Sync cycle is every 30 minutes by default, but it depends on the configuration of Azure AD Connect.</span></span> <span data-ttu-id="4aa0d-127">Dodatne informacije potražite u ovom [dokumentu](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).</span><span class="sxs-lookup"><span data-stu-id="4aa0d-127">For more information, refer this [document](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).</span></span>

5. <span data-ttu-id="4aa0d-128">U ovoj će fazi biti moguće vidjeti predmet uređaja u odjeljku "u **tijeku**" u odjeljku sprava Blade of Azure portal.</span><span class="sxs-lookup"><span data-stu-id="4aa0d-128">At this stage, you should be able to see the subject device in “**Pending**” state under Device blade of Azure Portal.</span></span>

6. <span data-ttu-id="4aa0d-129">Kada se sljedeći korisnik prijavi na Windows 10, registracija će biti dovršena.</span><span class="sxs-lookup"><span data-stu-id="4aa0d-129">At the next user login to Windows 10, the registration will be completed.</span></span>

    > [!NOTE]
    > <span data-ttu-id="4aa0d-130">Ako ste na VPN-u i odjava/prijava prestaje s povezivanjem domene, registraciju možete aktivirati ručno.</span><span class="sxs-lookup"><span data-stu-id="4aa0d-130">If you are on VPN and logoff/login terminates the domain connectivity, you can trigger registration manually.</span></span> <span data-ttu-id="4aa0d-131">Da biste to učinili, učinite sljedeće:</span><span class="sxs-lookup"><span data-stu-id="4aa0d-131">To do that:</span></span>
    >
    > <span data-ttu-id="4aa0d-132">Problem `dsregcmd /join` lokalno na administratorskom upitu ili na daljinu putem Psexez-a na PC.</span><span class="sxs-lookup"><span data-stu-id="4aa0d-132">Issue a `dsregcmd /join` locally on admin prompt or remotely via PSExec to your PC.</span></span>
    >
    > <span data-ttu-id="4aa0d-133">Na primjer: `PsExec -s \\win10client01 cmd, dsregcmd /join`</span><span class="sxs-lookup"><span data-stu-id="4aa0d-133">For example: `PsExec -s \\win10client01 cmd, dsregcmd /join`</span></span>

<span data-ttu-id="4aa0d-134">Za česte probleme s registracijom uređaja Azure Active Directory, pročitajte članak [Najčešća pitanja o uređajima](https://docs.microsoft.com/azure/active-directory/devices/faq).</span><span class="sxs-lookup"><span data-stu-id="4aa0d-134">For common issues with Azure Active Directory device registration, see [Devices FAQ](https://docs.microsoft.com/azure/active-directory/devices/faq).</span></span>
