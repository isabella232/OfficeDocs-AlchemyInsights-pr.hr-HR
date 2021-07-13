---
title: Odlazni relej
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/08/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "12315"
ms.openlocfilehash: b723566a29e0be581b7fdc30332166d5cddbd38f
ms.sourcegitcommit: 270a1ca9c35b50b8be6b06f432c9c90e4090fb57
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 07/08/2021
ms.locfileid: "53381595"
---
# <a name="outbound-relay-pool"></a><span data-ttu-id="1f93c-102">Odlazni relej</span><span class="sxs-lookup"><span data-stu-id="1f93c-102">Outbound relay pool</span></span>

<span data-ttu-id="1f93c-103">Microsoft mijenja konfiguraciju za prijenos ili prosljeđivanje e-pošte putem Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="1f93c-103">Microsoft is making some changes to the configuration for relaying or forwarding email through Microsoft 365.</span></span> <span data-ttu-id="1f93c-104">Poruke u određenim scenarijima prosljeđuju se ili prenose putem Microsoft 365 pomoću posebnog releja.</span><span class="sxs-lookup"><span data-stu-id="1f93c-104">Messages in certain scenarios are forwarded or relayed through Microsoft 365 using a special relay pool.</span></span> <span data-ttu-id="1f93c-105">Poruke poslane pomoću releja mogu završiti u mapi bezvrijedne pošte primatelja.</span><span class="sxs-lookup"><span data-stu-id="1f93c-105">Messages sent by using the relay pool could end up in recipient's junk mail folder.</span></span> <span data-ttu-id="1f93c-106">Dodatne informacije potražite u članku Grupe [izlazne isporuke](/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages#relay-pool)</span><span class="sxs-lookup"><span data-stu-id="1f93c-106">For more information, see [Outbound delivery pools](/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages#relay-pool)</span></span>

<span data-ttu-id="1f93c-107">Da biste izbjegli scenarij pomoću releja, provjerite zadovoljavaju li proslijeđene/proslijeđene poruke jedan od sljedećih kriterija:</span><span class="sxs-lookup"><span data-stu-id="1f93c-107">To avoid a scenario using the relay pool, make sure that forwarded/relayed messages meet one of the following criteria:</span></span>

- <span data-ttu-id="1f93c-108">Odlazni pošiljatelj prihvaćena je domena klijenta.</span><span class="sxs-lookup"><span data-stu-id="1f93c-108">The outbound sender is an accepted domain of the tenant.</span></span>
- <span data-ttu-id="1f93c-109">SPF (Sender Policy Framework) prosljeđuje se kada se poruka Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="1f93c-109">Sender Policy Framework (SPF) passes when the message comes to Microsoft 365.</span></span>
- <span data-ttu-id="1f93c-110">DomainKeys Identified Mail (DKIM) on the P2 sender domain passes when the message comes to Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="1f93c-110">DomainKeys Identified Mail (DKIM) on the P2 sender domain passes when the message comes to Microsoft 365.</span></span>
 
<span data-ttu-id="1f93c-111">Poruke koje zadovoljavaju gore navedene kriterije ne prenose se putem releja.</span><span class="sxs-lookup"><span data-stu-id="1f93c-111">Messages that meet the above criteria are not relayed through the relay pool.</span></span>

<span data-ttu-id="1f93c-112">Ako se MX zapis za vašu domenu usmjeri na poslužitelj drugih proizvođača ili lokalnog poslužitelja, pomoću poboljšanog filtriranja provjerite je li SPF provjera valjanosti točna za ulaznu e-poštu i da biste izbjegli slanje e-pošte putem releja.</span><span class="sxs-lookup"><span data-stu-id="1f93c-112">If the MX record for your domain is pointed to a third-party or on-premises server, use enhanced filtering to make sure the SPF validation is correct for inbound email and to avoid sending email through the relay pool.</span></span>

<span data-ttu-id="1f93c-113">**Kako možemo znati utječe li na nas relej?**</span><span class="sxs-lookup"><span data-stu-id="1f93c-113">**How can we tell if we're impacted by the relay pool?**</span></span>

<span data-ttu-id="1f93c-114">Ako proslijeđene ili proslijeđene poruke e-pošte koriste jedan od gore navedenih kriterija, poruke se neće prenijeti putem releja.</span><span class="sxs-lookup"><span data-stu-id="1f93c-114">If your forwarded or relayed emails use one of the above criteria, messages won't be relayed through the relay pool.</span></span> <span data-ttu-id="1f93c-115">No ako se poruka pošalje putem releja, IP odlaznog poslužitelja nalazi se u rasponu 40.95.0.0/16, a naziv izlaznog poslužitelja **sadrži rly** u naziv.</span><span class="sxs-lookup"><span data-stu-id="1f93c-115">However, if a message is sent through a relay pool, the outbound server IP is in the 40.95.0.0/16 range and the outbound server name includes **rly** in the name.</span></span>

