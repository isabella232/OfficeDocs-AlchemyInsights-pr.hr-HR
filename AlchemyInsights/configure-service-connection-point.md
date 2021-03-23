---
title: Konfiguriranje točke povezivanja servisa (SCP)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9732"
- "9003244"
ms.openlocfilehash: 9d733a1a0a3b8d92bdd5477a8978b6fbeede9653
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035097"
---
# <a name="configure-service-connection-point-scp"></a><span data-ttu-id="49e12-102">Konfiguriranje točke povezivanja servisa (SCP)</span><span class="sxs-lookup"><span data-stu-id="49e12-102">Configure Service connection Point (SCP)</span></span>

<span data-ttu-id="49e12-103">**DSREG_AUTOJOIN_ADCONFIG_READ_FAILED (0x801c001d/-2145648611)**</span><span class="sxs-lookup"><span data-stu-id="49e12-103">**DSREG_AUTOJOIN_ADCONFIG_READ_FAILED (0x801c001d/-2145648611)**</span></span>

- <span data-ttu-id="49e12-104">**Razlog**: nije moguće pročitati objekt SCP i nabaviti informacije o klijentu za Azure ad</span><span class="sxs-lookup"><span data-stu-id="49e12-104">**Reason**: Unable to read the SCP object and get the Azure AD tenant information</span></span>
- <span data-ttu-id="49e12-105">**Rezolucija**: Pogledajte odjeljak [Konfiguriranje točke povezivanja servisa](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains#configure-hybrid-azure-ad-join)</span><span class="sxs-lookup"><span data-stu-id="49e12-105">**Resolution**: Refer to the section [Configure a Service Connection Point](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains#configure-hybrid-azure-ad-join)</span></span>


<span data-ttu-id="49e12-106">**Akcijski plan**</span><span class="sxs-lookup"><span data-stu-id="49e12-106">**Action plan**</span></span>

- <span data-ttu-id="49e12-107">Provjerite je li uređaj primio GPO za kontroliranu provjeru valjanosti.</span><span class="sxs-lookup"><span data-stu-id="49e12-107">Check whether the device has received the GPO for the controlled validation.</span></span>
- <span data-ttu-id="49e12-108">Provjerite je li GPO stvorio ključeve registra.</span><span class="sxs-lookup"><span data-stu-id="49e12-108">Ensure that the GPO has created the registry keys.</span></span>
- <span data-ttu-id="49e12-109">Provjerite imate li dva ključa stvorena pomoću ID-a direktorija i domene u sustavu Microsoft.</span><span class="sxs-lookup"><span data-stu-id="49e12-109">Ensure that you have 2 keys created with your Directory ID and onmicrosoft domain.</span></span>

<span data-ttu-id="49e12-110">**Konfiguriranje postavke registra na klijentskoj strani za SCP**</span><span class="sxs-lookup"><span data-stu-id="49e12-110">**Configure client-side registry setting for SCP**</span></span>

<span data-ttu-id="49e12-111">Pomoću sljedećeg primjera stvorite objekt pravilnika grupe (GPO) da biste implementirali postavku registra koja u registru uređaja konfigurira unos u SCP-u.</span><span class="sxs-lookup"><span data-stu-id="49e12-111">Use the following example to create a Group Policy Object (GPO) to deploy a registry setting that configures an SCP entry in the registry of your devices.</span></span>

1. <span data-ttu-id="49e12-112">Otvorite konzolu za upravljanje pravilima grupe i stvorite novi GPO u svojoj domeni.</span><span class="sxs-lookup"><span data-stu-id="49e12-112">Open a Group Policy Management console and create a new GPO in your domain.</span></span>
     - <span data-ttu-id="49e12-113">Navedite novostvoreni GPO naziv (primjerice, ClientSideSCP)</span><span class="sxs-lookup"><span data-stu-id="49e12-113">Provide your newly created GPO a name (for example, ClientSideSCP)</span></span>

2. <span data-ttu-id="49e12-114">Uredite GPO i pronađite sljedeći put: postavke **računalne > postavke > Windows > Registry**.</span><span class="sxs-lookup"><span data-stu-id="49e12-114">Edit the GPO and locate the following path: **Computer Configuration > Preferences > Windows Settings > Registry**.</span></span>

3. <span data-ttu-id="49e12-115">Desnom tipkom miša kliknite **Registry** , a zatim odaberite **Nova > stavka registra**.</span><span class="sxs-lookup"><span data-stu-id="49e12-115">Right-click on **Registry** and select **New > Registry Item**.</span></span>

4. <span data-ttu-id="49e12-116">Na kartici **Općenito** konfigurirajte sljedeće:</span><span class="sxs-lookup"><span data-stu-id="49e12-116">On the **General** tab, configure the following:</span></span>
  
- <span data-ttu-id="49e12-117">**Akcija**: Ažuriranje</span><span class="sxs-lookup"><span data-stu-id="49e12-117">**Action**: Update</span></span>
    
- <span data-ttu-id="49e12-118">**Košnica**: HKEY_LOCAL_MACHINE</span><span class="sxs-lookup"><span data-stu-id="49e12-118">**Hive**: HKEY_LOCAL_MACHINE</span></span>
    
- <span data-ttu-id="49e12-119">**Ključ puta**: Software\microsoft\windows\currentversion\cdj\aad</span><span class="sxs-lookup"><span data-stu-id="49e12-119">**Key Path**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span></span>
    
- <span data-ttu-id="49e12-120">**Naziv vrijednosti**: tenantid</span><span class="sxs-lookup"><span data-stu-id="49e12-120">**Value name**: TenantId</span></span>
    
- <span data-ttu-id="49e12-121">**Vrsta vrijednosti**: REG_SZ</span><span class="sxs-lookup"><span data-stu-id="49e12-121">**Value type**: REG_SZ</span></span>
    
- <span data-ttu-id="49e12-122">**Podaci o vrijednosti**: ID GUID-a ili direktorij vaše instance Azure AD (ta se vrijednost može pronaći u **portalu Azure > azure Active directory > svojstva > ID direktorija**)</span><span class="sxs-lookup"><span data-stu-id="49e12-122">**Value data**: The GUID or Directory ID of your Azure AD instance (This value can be found in **Azure portal > Azure Active Directory > Properties > Directory ID**)</span></span>
 
- <span data-ttu-id="49e12-123">Kliknite **U redu**.</span><span class="sxs-lookup"><span data-stu-id="49e12-123">Click **OK**.</span></span>
 
5. <span data-ttu-id="49e12-124">Desnom tipkom miša kliknite **Registry** , a zatim odaberite **Nova > stavka registra**.</span><span class="sxs-lookup"><span data-stu-id="49e12-124">Right-click on **Registry** and select **New > Registry Item**.</span></span>

6. <span data-ttu-id="49e12-125">Na kartici **Općenito** konfigurirajte sljedeće:</span><span class="sxs-lookup"><span data-stu-id="49e12-125">On the **General** tab, configure the following:</span></span>
  
- <span data-ttu-id="49e12-126">**Akcija**: Ažuriranje</span><span class="sxs-lookup"><span data-stu-id="49e12-126">**Action**: Update</span></span>
    
- <span data-ttu-id="49e12-127">**Košnica**: HKEY_LOCAL_MACHINE</span><span class="sxs-lookup"><span data-stu-id="49e12-127">**Hive**: HKEY_LOCAL_MACHINE</span></span>
    
- <span data-ttu-id="49e12-128">**Ključ puta**: Software\microsoft\windows\currentversion\cdj\aad</span><span class="sxs-lookup"><span data-stu-id="49e12-128">**Key Path**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span></span>
    
- <span data-ttu-id="49e12-129">**Naziv vrijednosti**: tenantname</span><span class="sxs-lookup"><span data-stu-id="49e12-129">**Value name**: TenantName</span></span>
    
- <span data-ttu-id="49e12-130">**Vrsta vrijednosti**: REG_SZ</span><span class="sxs-lookup"><span data-stu-id="49e12-130">**Value type**: REG_SZ</span></span>
    
- <span data-ttu-id="49e12-131">**Podaci o vrijednosti**: potvrđeni naziv domene ako koristite Sjedinjenih okruženja kao što je AD FS.</span><span class="sxs-lookup"><span data-stu-id="49e12-131">**Value data**: Your verified domain name if you are using federated environment such as AD FS.</span></span> <span data-ttu-id="49e12-132">Potvrđeni naziv domene ili naziv domene onmicrosoft.com (primjerice contoso. inmicrosoft). com ako koristite upravljano okruženje</span><span class="sxs-lookup"><span data-stu-id="49e12-132">Your verified domain name or your onmicrosoft.com domain name (for example, contoso.onmicrosoft).com if you are using managed environment</span></span>

- <span data-ttu-id="49e12-133">Kliknite **U redu**.</span><span class="sxs-lookup"><span data-stu-id="49e12-133">Click **OK**.</span></span>

7. <span data-ttu-id="49e12-134">Zatvaranje uređivača za novostvorenog GPO-a.</span><span class="sxs-lookup"><span data-stu-id="49e12-134">Close the editor for the newly created GPO.</span></span>

8. <span data-ttu-id="49e12-135">Povežite novostvorenu GPO u željenu domenu koja sadrži računala koja pripadaju vašoj kontroliranoj populaciji.</span><span class="sxs-lookup"><span data-stu-id="49e12-135">Link the newly created GPO to the desired OU containing domain-joined computers that belong to your controlled rollout population.</span></span>

<span data-ttu-id="49e12-136">Dodatne informacije potražite u članku [kontrolirana provjera valjanosti hibridne Azure ad Join-Azure ad | Microsoft docs](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control) i  [Otklanjanje poteškoća s hibridom Azure Active Directory pridruženi uređaji | Microsoftovi dokumenti](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current).</span><span class="sxs-lookup"><span data-stu-id="49e12-136">For more information, see [Controlled validation of hybrid Azure AD join - Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control) and  [Troubleshooting hybrid Azure Active Directory joined devices | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current).</span></span>









