---
title: Problem s atributom atribut i skoping
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8470"
- "9004687"
ms.openlocfilehash: 78df24c0d8a670d678e26879cf81476f1ae9b92d
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50480969"
---
# <a name="problem-with-attribute-and-scoping-filter"></a><span data-ttu-id="9b949-102">Problem s atributom atribut i skoping</span><span class="sxs-lookup"><span data-stu-id="9b949-102">Problem with attribute and scoping filter</span></span>

<span data-ttu-id="9b949-103">**Problem s suprotnih vrijednosti UPN-a**</span><span class="sxs-lookup"><span data-stu-id="9b949-103">**Issue with conflicting UPN values**</span></span>

<span data-ttu-id="9b949-104">WORKDAY za oglase za dodjelu korisničkih radnih dana u servisu AD za korisnike prikazuje poruku o pogrešci **Hybridsinkronizationactivedirectoryuserprincipalnamenotunique**.</span><span class="sxs-lookup"><span data-stu-id="9b949-104">The Workday to AD User Provisioning Workday to AD User Provisioning shows error message **HybridSynchronizationActiveDirectoryUserPrincipalNameNotUnique**.</span></span> <span data-ttu-id="9b949-105">Operacija nije uspjela jer vrijednost UPN koja je navedena za dodavanje/izmjena nije jedinstvena u širokom nivou šuma.</span><span class="sxs-lookup"><span data-stu-id="9b949-105">The operation failed because UPN value provided for addition/modification is not unique forest-wide.</span></span> <span data-ttu-id="9b949-106">Pojedinosti o pogrešci: **CONSTRAINT_ATT_TYPE-userPrincipalName**.</span><span class="sxs-lookup"><span data-stu-id="9b949-106">Error Details: **CONSTRAINT_ATT_TYPE - userPrincipalName**.</span></span>

<span data-ttu-id="9b949-107">Vrijednost **UserPrincipalName** koja WORKDAY konektor pokušava postaviti prilikom stvaranja korisničkog računa za oglas već postoji u ciljnoj domeni oglasa.</span><span class="sxs-lookup"><span data-stu-id="9b949-107">The **userPrincipalName** value that Workday connector is trying to set when creating the AD user account already exists in the target AD domain.</span></span> <span data-ttu-id="9b949-108">To implicira da bilo (1) korisnik već postoji, a provjera podudaranja ID-a nije uspjela za korisnika ili (2) pravilo stvaranja različite vrijednosti.</span><span class="sxs-lookup"><span data-stu-id="9b949-108">This implies that either (1) the user already exists and the matching ID check failed for the user or (2) the UPN generation rule generated a conflicting value.</span></span>

<span data-ttu-id="9b949-109">Evo predloženih koraka sanacije:</span><span class="sxs-lookup"><span data-stu-id="9b949-109">Here are the suggested resolution steps:</span></span>

<span data-ttu-id="9b949-110">Ako korisnik već postoji, a provjera podudaranja ID-a nije uspjela povezati račun WORKDAY s računom servisa Active Directory, provjerite je li atribut podudaranja ID-a (obično **IDZaposlenika**) u radnom danu i oglasu točno podudaran.</span><span class="sxs-lookup"><span data-stu-id="9b949-110">If the user already exists and the matching ID check failed to link the Workday account to Active Directory account, then check if the matching ID attribute (typically **employeeID**) in both Workday and AD have an exact match.</span></span> <span data-ttu-id="9b949-111">Ako nemaju podudaranje, to je problem s podacima koji je potreban za popravak.</span><span class="sxs-lookup"><span data-stu-id="9b949-111">If they don't have a match, it is a data issue that needs to be fixed.</span></span> <span data-ttu-id="9b949-112">Ako je, primjerice, IDZaposlenika u radnim danom 001052, a u aplikaciji AD to je 1052, motor za dodjelu resursa neće uspjeti spojiti dva računa i pokušat će stvoriti korisnika koji već postoji.</span><span class="sxs-lookup"><span data-stu-id="9b949-112">For example, if the EmployeeID in Workday is 001052 and in AD it is 1052, then the provisioning engine will fail to link the two accounts and will try to create a user that already exists.</span></span> <span data-ttu-id="9b949-113">Rješenje u ovom slučaju jest promjena vrijednosti **zaposlenika** u aplikaciji ad da biste uključili početne nule da bi bilo 001052.</span><span class="sxs-lookup"><span data-stu-id="9b949-113">The solution in this case is to change the **EmployeeID** value in AD to include the leading zeros to make it 001052.</span></span>
<span data-ttu-id="9b949-114">Ako izraz UPN-generiranje ne generira jedinstvenu vrijednost, razmotrite korištenje funkcije de-dupliciranje **Selectuniquevalue** da bi se svaki put generirao jedinstvena vrijednost.</span><span class="sxs-lookup"><span data-stu-id="9b949-114">If the UPN-generating expression is not generating a unique value, consider using the de-duplication function **SelectUniqueValue** to generate a unique value each time.</span></span>

<span data-ttu-id="9b949-115">**Radni dan za dodjelu resursa korisniku oglasa ne postavlja vrijednost atributa upravitelja za korisnički račun za oglas**</span><span class="sxs-lookup"><span data-stu-id="9b949-115">**Workday to AD User Provisioning does not set manager attribute value for AD user account**</span></span>

<span data-ttu-id="9b949-116">Radni dan za dodjelu resursa korisniku oglasa ne postavlja vrijednost atributa **upravitelja** za KORISNIČKE račune oglasa.</span><span class="sxs-lookup"><span data-stu-id="9b949-116">The Workday to AD User Provisioning job is not setting the **manager** attribute value for AD user accounts.</span></span> <span data-ttu-id="9b949-117">Postoje dva moguća scenarija kada se to ponašanje vidi:</span><span class="sxs-lookup"><span data-stu-id="9b949-117">There are two possible scenarios when this behavior is seen:</span></span>

1. <span data-ttu-id="9b949-118">Upravitelj u radnim danom ne može se razriješiti na odgovarajući korisnički račun za oglas jer upravitelj nije u opsegu.</span><span class="sxs-lookup"><span data-stu-id="9b949-118">The manager in Workday cannot be resolved to a corresponding AD User account because the manager is not in scope.</span></span>
2. <span data-ttu-id="9b949-119">U scenariju **višestrukih domena oglasa** upravitelj u radnom danu nije prisutan u istoj domeni kao i korisnik.</span><span class="sxs-lookup"><span data-stu-id="9b949-119">In a **multiple AD domains** scenario, the manager in Workday is not present in the same domain as the user.</span></span>

<span data-ttu-id="9b949-120">Da biste riješili problem, isprobajte sljedeće korake:</span><span class="sxs-lookup"><span data-stu-id="9b949-120">Try these steps to resolve the issue:</span></span>

1. <span data-ttu-id="9b949-121">Ako ste definirali filtre za filtriranje, najprije provjerite je li upravitelj u opsegu i zadovoljava li uvjet skoping.</span><span class="sxs-lookup"><span data-stu-id="9b949-121">If you have defined scoping filters, first check if the manager is in scope and that it satisfies the scoping clause.</span></span> <span data-ttu-id="9b949-122">Ako upravitelj ne zadovolji filtar, promijenite filtar tako da je i upravitelj u opsegu postupka dodjele resursa.</span><span class="sxs-lookup"><span data-stu-id="9b949-122">If the manager does not satisfy the scoping filter, change the filter so that the manager is also in scope of the provisioning operation.</span></span>
2. <span data-ttu-id="9b949-123">Ako imate više domena oglasa, poveznik sadrži poznato ograničenje nemogućnosti rješavanja referenci upravitelja unakrsnih domena.</span><span class="sxs-lookup"><span data-stu-id="9b949-123">If you have multiple AD domains, then the connector has a known limitation of inability to resolve cross-domain manager references.</span></span>

<span data-ttu-id="9b949-124">Dodatne informacije o konfiguriranju radnog dana za automatiziranu dodjelu resursa potražite u članku [Udžbenik: Konfiguriranje radnog dana za automatsku dodjelu korisnika](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span><span class="sxs-lookup"><span data-stu-id="9b949-124">For more details on configuring workday for automated provisioning, see [Tutorial: Configure Workday for automatic user provisioning](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>













