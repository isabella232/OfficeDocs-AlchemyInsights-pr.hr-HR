---
title: Sinkronizacija lozinki
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "8619"
ms.openlocfilehash: 601649f6e5212ca03df5fcc32cd1d02c133e9170
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481144"
---
# <a name="password-synchronization"></a><span data-ttu-id="c0624-102">Sinkronizacija lozinki</span><span class="sxs-lookup"><span data-stu-id="c0624-102">Password synchronization</span></span>

<span data-ttu-id="c0624-103">**Sinkronizacija zaporke za lozinke ne funkcionira uopće**</span><span class="sxs-lookup"><span data-stu-id="c0624-103">**Password Hash Synchronization does not work at all**</span></span>

<span data-ttu-id="c0624-104">Neki Česti problemi s kojima se korisnici susreću kada sinkronizacija lozinke ne funkcionira:</span><span class="sxs-lookup"><span data-stu-id="c0624-104">Some common issues customers encounter when Password Hash Synchronization does not work are:</span></span>

- <span data-ttu-id="c0624-105">Račun za Active Directory koji koristi Azure AD Connect da bi komunicirala s lokalnim aktivnim imenikom nije odobreno **repliciranje promjena direktorija** i **Replicacijski direktorij mijenja sve** dozvole, koje su potrebne za sinkronizaciju lozinki – morate to riješiti tako da dodijelite ove dozvole za račun servisa Active Directory.</span><span class="sxs-lookup"><span data-stu-id="c0624-105">The Active Directory account used by Azure AD Connect to communicate with on-premises Active Directory is not granted **Replicate Directory Changes** and **Replicate Directory Changes All** permissions, which are required for password synchronization - You need to fix this by granting these permissions to the Active Directory account.</span></span>
- <span data-ttu-id="c0624-106">Sinkronizacija zaporke za lozinke onemogućena je nakon što je administrator izmijenio način korištenja korisničke Sign-In iz **sinkronizacije lozinki** u neku drugu mogućnost, kao što je **Federacija sa programom AD FS** u čarobnjaku za Azure ad Connect – to možete riješiti ponovnim omogućivanjem značajke **sinkronizacije zaporke za lozinke** u čarobnjaku za Azure ad Connect.</span><span class="sxs-lookup"><span data-stu-id="c0624-106">Password hash synchronization is disabled after an administrator changed the User Sign-In method from **Password Synchronization** to another option such as **Federation with AD FS** in the Azure AD Connect wizard - You can fix this by re-enabling the **password hash synchronization** feature in the Azure AD Connect wizard.</span></span>
- <span data-ttu-id="c0624-107">Problem s povezivanjem s lokalnim aktivnim imenikom.</span><span class="sxs-lookup"><span data-stu-id="c0624-107">Connectivity issue with on-premises Active Directory.</span></span> <span data-ttu-id="c0624-108">Primjerice, nekim kontrolorima domena nije moguće pristupiti pomoću servisa Azure AD Connect ili je vatrozid [potreban](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports) da biste ga blokirali, morate to riješiti tako da veza između poslužitelja Azure ad Connect i lokalnog servisa Active Directory funkcionira ispravno.</span><span class="sxs-lookup"><span data-stu-id="c0624-108">For example, some domain controllers are not accessible by Azure AD Connect, or the [ports required](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports) are blocked by Firewall - You need to fix this by ensuring that the connectivity between the Azure AD Connect server and the on-premises Active Directory works correctly.</span></span>
- <span data-ttu-id="c0624-109">Poslužitelj za Azure AD Connect trenutno se nalazi u načinu rada za uključivanje u modu, što će prouzročiti da poslužitelj ne može otkloniti lozinku – da biste otklonili problem, slijedite korake opisane u odjeljku [Otklanjanje poteškoća s sinkronizacijom lozinke pomoću servisa Azure ad Connect sync – ne sinkroniziraju se lozinke](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span><span class="sxs-lookup"><span data-stu-id="c0624-109">Azure AD Connect server currently being in staging mode, which will result the server not being able to the password hashes - To troubleshoot the issue, follow the steps described in section [Troubleshoot password synchronization with Azure AD Connect sync - No passwords are synchronized](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>

<span data-ttu-id="c0624-110">**Sinkronizacija lozinki za lozinke ne funkcionira za neke korisnike**</span><span class="sxs-lookup"><span data-stu-id="c0624-110">**Password Hash Synchronization does not work for some of my users**</span></span>

1. <span data-ttu-id="c0624-111">Ako ste primijetili da se dodatak za lozinke ne sinkronizira za korisnika, upotrijebite zadatak **otklanjanja poteškoća** u programu Azure ad Connect da biste istražili i riješili problem.</span><span class="sxs-lookup"><span data-stu-id="c0624-111">If you noticed that password hash is not syncing for a user, use the **troubleshoot** task in the Azure AD Connect to investigate and resolve the issue.</span></span> <span data-ttu-id="c0624-112">Izvedite sljedeće zadatke:</span><span class="sxs-lookup"><span data-stu-id="c0624-112">Perform the following tasks:</span></span>

    <span data-ttu-id="c0624-113">je.</span><span class="sxs-lookup"><span data-stu-id="c0624-113">a.</span></span> [<span data-ttu-id="c0624-114">Pokretanje zadatka otklanjanja poteškoća u čarobnjaku</span><span class="sxs-lookup"><span data-stu-id="c0624-114">Run the troubleshooting task in the wizard</span></span>](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-objectsync)

    <span data-ttu-id="c0624-115">b.</span><span class="sxs-lookup"><span data-stu-id="c0624-115">b.</span></span> [<span data-ttu-id="c0624-116">Korištenje cmdleta za otklanjanje poteškoća radi istraživanja problema s sinkronizacijom lozinke za određeno korištenje</span><span class="sxs-lookup"><span data-stu-id="c0624-116">Use the troubleshooting cmdlet to investigate the password hash syncing issue for a specific use</span></span>](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)

2. <span data-ttu-id="c0624-117">Korisnički objekt lokalnog imenika Active Directory omogućen je za **korisnika mora promijeniti lozinku pri sljedećoj mogućnosti prijave** .</span><span class="sxs-lookup"><span data-stu-id="c0624-117">The on-premises Active Directory User object is enabled for **User must change password at next logon** option.</span></span> <span data-ttu-id="c0624-118">Kada je ta mogućnost omogućena, korisniku se dodjeljuje privremena lozinka i od vas će se zatražiti da promijenite lozinku na sljedećoj prijavi.</span><span class="sxs-lookup"><span data-stu-id="c0624-118">When this option is enabled, the user is assigned a temporary password and will be prompted to change the password on the next logon.</span></span> <span data-ttu-id="c0624-119">Azure AD Connect ne sinkronizira privremene lozinke za Azure AD.</span><span class="sxs-lookup"><span data-stu-id="c0624-119">Azure AD Connect does not synchronize temporary passwords to Azure AD.</span></span>

<span data-ttu-id="c0624-120">Da biste riješili gore navedeni problem, izvedite neki od sljedećih zadataka:</span><span class="sxs-lookup"><span data-stu-id="c0624-120">To resolve the above issue, perform either of the following tasks:</span></span>

- <span data-ttu-id="c0624-121">Zatražite od korisnika da se prijavi u lokalnu aplikaciju (primjerice, stolna računala sa sustavom Windows) i promijenite lozinku.</span><span class="sxs-lookup"><span data-stu-id="c0624-121">Ask the user to sign in to on-premises application (for example, Windows Desktop) and change the password.</span></span> <span data-ttu-id="c0624-122">Nova lozinka sinkronizirat će se sa servisom Azure AD.</span><span class="sxs-lookup"><span data-stu-id="c0624-122">The new password will be synchronized to Azure AD.</span></span>
- <span data-ttu-id="c0624-123">Administrator će ažurirati korisničku lozinku bez omogućivanja mogućnosti da **korisnik mora promijeniti lozinku pri sljedećoj prijavi** i zajednički koristiti novu lozinku s korisnikom.</span><span class="sxs-lookup"><span data-stu-id="c0624-123">Have an administrator update the user's password without enabling the option **User must change password at next logon**, and share the new password with the user.</span></span>

3. <span data-ttu-id="c0624-124">Lokalni objekt servisa Active Directory **nije pravilno konfiguriran** za sinkronizaciju objekata ili sinkronizaciju lozinki.</span><span class="sxs-lookup"><span data-stu-id="c0624-124">The on-premises Active Directory User object is **not correctly configured** for object synchronization or password synchronization.</span></span> <span data-ttu-id="c0624-125">Da biste riješili taj problem, slijedite korake opisane u [članku Otklanjanje poteškoća sa sinkroniziranjem lozinke uz sinkronizaciju servisa Azure ad Connect](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span><span class="sxs-lookup"><span data-stu-id="c0624-125">To troubleshoot this issue, follow the steps described in the [Troubleshoot password hash synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>







