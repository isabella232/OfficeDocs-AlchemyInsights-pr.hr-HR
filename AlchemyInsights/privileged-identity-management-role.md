---
title: Povlaštena uloga upravljanja identitetom
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
- "9003230"
- "6825"
ms.openlocfilehash: 726511d016462f56c48a4272b57abc3e9f0cbc3d
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 11/17/2020
ms.locfileid: "49088569"
---
# <a name="privileged-identity-managementpim-role"></a><span data-ttu-id="0c492-102">Povlaštene uloge za upravljanje identitetom (PIM)</span><span class="sxs-lookup"><span data-stu-id="0c492-102">Privileged Identity Management(PIM) role</span></span>

<span data-ttu-id="0c492-103">**Dozvole se ne dodjeljuju nakon aktiviranja uloge**</span><span class="sxs-lookup"><span data-stu-id="0c492-103">**Permissions are not granted after activating a role**</span></span>

<span data-ttu-id="0c492-104">Kada aktivirate ulogu u povlaštenom upravljanju identitetom servisa Azure AD (PIM), aktivacija se možda neće odmah proširiti na sve portale koje zahtijevaju privilegiranu ulogu.</span><span class="sxs-lookup"><span data-stu-id="0c492-104">When you activate a role in Azure AD Privileged Identity Management (PIM), the activation may not instantly propagate to all portals that require the privileged role.</span></span> <span data-ttu-id="0c492-105">Ponekad se, čak i ako se promjena proširi, web-predmemoriranje na portalu može rezultirati promjenom netrenutačne efekte.</span><span class="sxs-lookup"><span data-stu-id="0c492-105">Sometimes, even if the change is propagated, web caching in a portal may result in the change not taking effect immediately.</span></span>

<span data-ttu-id="0c492-106">Ako aktivacija kasni, slijedite ove korake:</span><span class="sxs-lookup"><span data-stu-id="0c492-106">If your activation is delayed, follow these steps:</span></span>

1. <span data-ttu-id="0c492-107">Odjavite se s portala Azure, a zatim se ponovno prijavite.</span><span class="sxs-lookup"><span data-stu-id="0c492-107">Sign out of the Azure portal and then sign back in.</span></span> <span data-ttu-id="0c492-108">Kada aktivirate ulogu Azure AD ili ulogu resursa Azure, prikazat će vam se faze aktivacije.</span><span class="sxs-lookup"><span data-stu-id="0c492-108">When you activate an Azure AD role or an Azure resource role, you will see the stages of your activation.</span></span> <span data-ttu-id="0c492-109">Kada završite sa svim fazama, prikazat će se veza za odjavu.</span><span class="sxs-lookup"><span data-stu-id="0c492-109">Once all the stages are complete, you will see a 'Sign out' link.</span></span> <span data-ttu-id="0c492-110">Ovu vezu možete koristiti za odjavu. To će riješiti većinu slučajeva za kašnjenje aktivacije.</span><span class="sxs-lookup"><span data-stu-id="0c492-110">You can use this link to sign out. This will solve most cases for activation delay.</span></span>
2. <span data-ttu-id="0c492-111">U servisu PIM provjerite jeste li navedeni kao član uloge.</span><span class="sxs-lookup"><span data-stu-id="0c492-111">In PIM, verify that you are listed as the member of the role.</span></span>
3. <span data-ttu-id="0c492-112">Ako aktivirate ulogu administratora sustava Exchange, provjerite jeste li se odjavili i ponovno prijavili.</span><span class="sxs-lookup"><span data-stu-id="0c492-112">If you are activating the Exchange Administrator role, make sure you sign out and sign back in.</span></span> <span data-ttu-id="0c492-113">Ako se problem ne riješi, otvorite karticu za podršku i Podignimo ovo kao problem.</span><span class="sxs-lookup"><span data-stu-id="0c492-113">If the problem persists, open a support ticket and raise this as an issue.</span></span> <span data-ttu-id="0c492-114">Ako koristite ulogu administratora sustava Exchange za pristup centru za sigurnost i usklađenost, pročitajte sljedeći korak.</span><span class="sxs-lookup"><span data-stu-id="0c492-114">If you are using your Exchange Administrator role to access the Security and Compliance Center, see the next step.</span></span>
4. <span data-ttu-id="0c492-115">Ako aktivirate ulogu za pristup centru za sigurnost i usklađenost ili ako aktivirate ulogu administratora sustava SharePoint, za nekoliko minuta doživjet ćete odgodu aktivacije do nekoliko sati.</span><span class="sxs-lookup"><span data-stu-id="0c492-115">If you are activating a role to access the Security and Compliance Center or if you are activating the SharePoint Administrator role, you will experience some activation delay from a few minutes up to a few hours.</span></span> <span data-ttu-id="0c492-116">To je poznat problem i aktivno radimo s tim timovima radi rješavanja tog problema što je prije moguće.</span><span class="sxs-lookup"><span data-stu-id="0c492-116">This is a known issue and we are actively working with these teams to resolve this issue as soon as possible.</span></span>

<span data-ttu-id="0c492-117">Dodatne informacije potražite u članku:</span><span class="sxs-lookup"><span data-stu-id="0c492-117">For more information, see:</span></span>

- [<span data-ttu-id="0c492-118">Aktiviranje uloga Azure oglasa u servisu PIM</span><span class="sxs-lookup"><span data-stu-id="0c492-118">Activate my Azure AD roles in PIM</span></span>](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?wt.mc_id=portal-microsoft_azure_support")
- [<span data-ttu-id="0c492-119">Aktivacija uloga resursa za Azure u servisu PIM</span><span class="sxs-lookup"><span data-stu-id="0c492-119">Activate my Azure resource roles in PIM</span></span>](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?wt.mc_id=portal-microsoft_azure_support")

<span data-ttu-id="0c492-120">**Dozvole se ne uklanjaju Nakon deaktivacije uloge ili isteka aktivacije uloge**</span><span class="sxs-lookup"><span data-stu-id="0c492-120">**Permissions are not removed after deactivating a role or the role activation expires**</span></span>

<span data-ttu-id="0c492-121">Kada deaktivirate ulogu u povlaštenom upravljanju identitetu ili kada istekne razdoblje aktivacije uloga, možda će biti odgoda gdje ćete i dalje imati pristup.</span><span class="sxs-lookup"><span data-stu-id="0c492-121">When you deactivate a role in Azure AD Privileged Identity Management or when a role activation period expires, there might be a delay where you continue to have access.</span></span>

<span data-ttu-id="0c492-122">Ako vaša deaktivacija kasni, slijedite ove korake:</span><span class="sxs-lookup"><span data-stu-id="0c492-122">If your deactivation is delayed, follow these steps:</span></span>

1. <span data-ttu-id="0c492-123">Ako deaktivirate ulogu administratora sustava Exchange ili razdoblje aktivacije uloga, a primjetite značajno kašnjenje prije uklanjanja dozvola, otvorite karticu za podršku i obavijestite inženjera za podršku da vam pomogne podnijeti prijavu karte pomoću tima za upravljanje povlaštenim pristupom (PAM) u sustavu Office u vezi s tim problemom.</span><span class="sxs-lookup"><span data-stu-id="0c492-123">If you are deactivating the Exchange Administrator role or the role activation period expires, and you notice a significant delay before the permissions are removed, open a support ticket and tell your support engineer to help you file a ticket with the Privileged Access Management (PAM) team inside Office about this issue.</span></span>
2. <span data-ttu-id="0c492-124">Ako je razdoblje aktivacije isteklo, ali i dalje imate otvorenu sesiju preglednika, zatvori preglednik.</span><span class="sxs-lookup"><span data-stu-id="0c492-124">If the activation period has expired, but you still have the browser session open, close your browser.</span></span> <span data-ttu-id="0c492-125">Ulogu možete nastaviti koristiti sve dok ne zatvoriš tu sesiju.</span><span class="sxs-lookup"><span data-stu-id="0c492-125">You can continue to use the role until you close that session.</span></span> <span data-ttu-id="0c492-126">To je poznat problem i tražimo potencijalno rješenje za aktivno ukidanje svake sesije kada je aktivacija istekla.</span><span class="sxs-lookup"><span data-stu-id="0c492-126">This is a known issue and we are looking at a potential fix to actively revoke each session once activation has expired.</span></span>

<span data-ttu-id="0c492-127">Ako vam se kašnjenje razlikuje od ovih dvaju scenarija, otvorite karticu za podršku.</span><span class="sxs-lookup"><span data-stu-id="0c492-127">If your delay is different than these two scenarios, please open a support ticket.</span></span>
