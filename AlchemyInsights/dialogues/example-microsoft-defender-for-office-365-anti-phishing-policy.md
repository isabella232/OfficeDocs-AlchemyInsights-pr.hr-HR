---
title: Primjer Microsoft Defender za Office 365 anti-phishing pravilnik
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: eabff70c22b641627d3ab6c0b2f8846a0be2f49e
ms.sourcegitcommit: 60c504f3ac187eaf1141b3ba701d9e0633bdd968
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/08/2021
ms.locfileid: "50692795"
---
# <a name="example-microsoft-defender-for-office-365-anti-phishing-policy"></a><span data-ttu-id="1f783-102">Primjer Microsoft Defender za Office 365 anti-phishing pravilnik</span><span class="sxs-lookup"><span data-stu-id="1f783-102">Example Microsoft Defender for Office 365 anti-phishing policy</span></span>

<span data-ttu-id="1f783-103">Ove postavke omogućuju politiku zvanu *domena i izvršni direktor*.</span><span class="sxs-lookup"><span data-stu-id="1f783-103">These settings enable a policy called *Domain and CEO*.</span></span> <span data-ttu-id="1f783-104">Ovo pravilo omogućuje oponašanje korisnika i domene, a zatim pravilnik primjenjuje na sve e-poštu primljene od korisnika unutar domene.</span><span class="sxs-lookup"><span data-stu-id="1f783-104">This policy provides both user and domain protection from impersonation and then applies the policy to all email received by users within the domain.</span></span> <span data-ttu-id="1f783-105">Najprije dodajte sljedeće podatke da biste stvorili pravilo:</span><span class="sxs-lookup"><span data-stu-id="1f783-105">First, add the following information to create the policy:</span></span>

- <span data-ttu-id="1f783-106">**Naziv**: domena i ceo **Opis**: osigurava da se izvršni direktor i vaša domena ne oponašate.</span><span class="sxs-lookup"><span data-stu-id="1f783-106">**Name**: Domain and CEO **Description**: Ensures that the CEO and your domain are not being impersonated.</span></span>
  <span data-ttu-id="1f783-107">**Primijenjena na**: odaberite **domenu primatelja**.</span><span class="sxs-lookup"><span data-stu-id="1f783-107">**Applied to**: Select **The recipient domain is**.</span></span> <span data-ttu-id="1f783-108">U odjeljku **bilo koji od ovih** mogućnosti odaberite **Odaberi**, a zatim odaberite domenu.</span><span class="sxs-lookup"><span data-stu-id="1f783-108">Under **Any of these**, select **Choose**, and then select a domain.</span></span> <span data-ttu-id="1f783-109">Odaberite **+ Dodaj**.</span><span class="sxs-lookup"><span data-stu-id="1f783-109">Select **+ Add**.</span></span> <span data-ttu-id="1f783-110">Potvrdite okvir pokraj naziva domene na popisu (na primjer, *contoso.com*), a zatim odaberite **Dodaj**.</span><span class="sxs-lookup"><span data-stu-id="1f783-110">Select the check box next to the name of the domain in the list (for example, *contoso.com*), and then select **Add**.</span></span> <span data-ttu-id="1f783-111">Odaberite **gotovo**.</span><span class="sxs-lookup"><span data-stu-id="1f783-111">Select **Done**.</span></span>
- <span data-ttu-id="1f783-112">Nakon stvaranja pravilnika možete precizno podesiti pravilo pomoću sljedećih mogućnosti:</span><span class="sxs-lookup"><span data-stu-id="1f783-112">After the policy is created, you can fine-tune the policy by using the following options:</span></span>
  - <span data-ttu-id="1f783-113">**Dodavanje korisnika u zaštitu:** U ovom primjeru na minimum dodajte adresu e-pošte glavnog direktora.</span><span class="sxs-lookup"><span data-stu-id="1f783-113">**Add users to protect:** For this example, add the CEO's email address, at a minimum.</span></span>
  - <span data-ttu-id="1f783-114">**Dodajte domene koje treba štititi**: Dodajte organizacijsku domenu koja obuhvaća ured izvršnog direktora.</span><span class="sxs-lookup"><span data-stu-id="1f783-114">**Add domains to protect**: Add the organizational domain that includes the office of the CEO.</span></span>
  - <span data-ttu-id="1f783-115">**Odaberite akcije**: **Ako je e-pošta poslao imitirani korisnik**, odaberite **Preusmjeri poruku na drugu adresu e-pošte**, a zatim unesite adresu e-pošte sigurnosnog administratora (na primjer, *securityadmin@contoso.com*).</span><span class="sxs-lookup"><span data-stu-id="1f783-115">**Choose actions**: For **If email is sent by an impersonated user**, select **Redirect message to another email address**, and then enter the email address of the security administrator (for example, *securityadmin@contoso.com*).</span></span> <span data-ttu-id="1f783-116">**Ako je e-pošta poslala imitirana domena**, odaberite **karantensku poruku**.</span><span class="sxs-lookup"><span data-stu-id="1f783-116">For **If email is sent by an impersonated domain**, select **Quarantine the message**.</span></span>
  - <span data-ttu-id="1f783-117">**Inteligencija poštanskog sandučića**: po zadanom je odabrana ta mogućnost prilikom stvaranja novog pravilnika o krađi identiteta.</span><span class="sxs-lookup"><span data-stu-id="1f783-117">**Mailbox intelligence**: By default, this option is selected when you create a new anti-phishing policy.</span></span> <span data-ttu-id="1f783-118">Ovu **postavku ostavite radi najboljih** rezultata.</span><span class="sxs-lookup"><span data-stu-id="1f783-118">Leave this setting **On** for best results.</span></span>
  - <span data-ttu-id="1f783-119">**Dodavanje pouzdanih pošiljatelja i domena:** U ovom primjeru nemojte definirati prekoračenja.</span><span class="sxs-lookup"><span data-stu-id="1f783-119">**Add trusted senders and domains:** For this example, don't define any overrides.</span></span>
- <span data-ttu-id="1f783-120">Kada pregledate postavke, odaberite **Stvori ovo pravilo** ili **Spremi**, po potrebi.</span><span class="sxs-lookup"><span data-stu-id="1f783-120">Once you've reviewed your settings, select **Create this policy** or **Save**, as appropriate.</span></span>

<span data-ttu-id="1f783-121">Dodatne informacije potražite u članku [politika suzbijanja krađe identiteta u programu Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2092235).</span><span class="sxs-lookup"><span data-stu-id="1f783-121">To learn more, see [Anti-phishing policies in Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2092235).</span></span>
