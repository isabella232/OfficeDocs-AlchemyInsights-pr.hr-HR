---
title: 'AIP: pravila se ne ponašaju kao što je očekivano'
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
- "9002266"
- "4780"
ms.openlocfilehash: 0dfaae776ec551fe12919e8a8e69f2e7a58d67d0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663181"
---
# <a name="aip-policies-not-behaving-as-expected"></a><span data-ttu-id="59a47-102">AIP: pravila se ne ponašaju kao što je očekivano</span><span class="sxs-lookup"><span data-stu-id="59a47-102">AIP: Policies not behaving as expected</span></span>

<span data-ttu-id="59a47-103">Zaštita informacija o Azure: pravila se ne ponašaju kao što je očekivano, pročitajte sljedeće za preporučene smjernice za razne probleme s politikom:</span><span class="sxs-lookup"><span data-stu-id="59a47-103">Azure Information Protection: Policies not behaving as expected, see the following for recommended guidelines for various policy issues:</span></span>

1. <span data-ttu-id="59a47-104">Ako nailazite na probleme s vizualnim oznakama, pregledajte [kada se primjenjuju vizualne oznake](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span><span class="sxs-lookup"><span data-stu-id="59a47-104">If you are having issues with visual markings, please review [When visual markings are applied](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span></span>
2. <span data-ttu-id="59a47-105">Ako imate problema s automatskim označavanju, pregledajte [način konfiguriranja uvjeta za automatsku i preporučenu klasifikaciju za zaštitu informacija za Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) te [koje vrste osjetljivih podataka traže](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span><span class="sxs-lookup"><span data-stu-id="59a47-105">If you are having issues with automatic labeling, please review [How to configure conditions for automatic and recommended classification for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) and [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>
3. <span data-ttu-id="59a47-106">Ako imate problema s zaštitom izvornih/Pdatoteka, pročitajte [konfiguraciju datoteka API](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration)-ja.</span><span class="sxs-lookup"><span data-stu-id="59a47-106">If you are having issues with Native/Pfile protection, please review [File API configuration](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span></span>
4. <span data-ttu-id="59a47-107">Provjerite koristite li pravila koja nisu ispravno konfigurirana: [kako konfigurirati pravilnik o zaštiti podataka za Azure za određene korisnike pomoću pravilnika u opsegu](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span><span class="sxs-lookup"><span data-stu-id="59a47-107">Check if you are using scoped policies that aren't configured properly: [How to configure the Azure Information Protection policy for specific users by using scoped policies](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span></span>
5. <span data-ttu-id="59a47-108">Ako automatsko označavanje ne funkcionira u programu Outlook prilikom prilaganja označenom dokumentu, provjerite ne definira li se funkcija DRMEncryptProperty kao što je opisano ovdje: [postavke registra IRM-a za sigurnost](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span><span class="sxs-lookup"><span data-stu-id="59a47-108">If automatic labeling isn't working for Outlook when attaching a labeled document, verify that DRMEncryptProperty isn't defined as described here: [IRM registry settings for security](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span></span>

<span data-ttu-id="59a47-109">Ako i dalje nailazite na probleme, prikupite zapisnike o zaštiti podataka za Azure i priložite izvezene zapisnike na ovu ulaznicu.</span><span class="sxs-lookup"><span data-stu-id="59a47-109">If you still are experiencing issues, please collect Azure Information Protection client logs and attach the exported logs to this ticket.</span></span>

1. <span data-ttu-id="59a47-110">Otvaranje dokumenta sustava Office ili stvaranje nove poruke e-pošte u programu Outlook.</span><span class="sxs-lookup"><span data-stu-id="59a47-110">Open an Office document or create a new email in Outlook.</span></span>
2. <span data-ttu-id="59a47-111">Kliknite **zaštiti/osjetljivosti**  >  **pomoći i povratnih informacija**.</span><span class="sxs-lookup"><span data-stu-id="59a47-111">Click **Protect/Sensitivity** > **Help and feedback**.</span></span>
3. <span data-ttu-id="59a47-112">Kliknite **Izvezi zapisnike**.</span><span class="sxs-lookup"><span data-stu-id="59a47-112">Click **Export Logs**.</span></span>
4. <span data-ttu-id="59a47-113">Spremite zapisnike na odabir mjesta i priložite ih na ovaj zahtjev za servis.</span><span class="sxs-lookup"><span data-stu-id="59a47-113">Save the logs to your choice of location, and attach them to this service request.</span></span>

<span data-ttu-id="59a47-114">Dodatni resursi:</span><span class="sxs-lookup"><span data-stu-id="59a47-114">Additional resources:</span></span>

- [<span data-ttu-id="59a47-115">Konfiguriranje natpisa za vizualne oznake za zaštitu informacija za Azure</span><span class="sxs-lookup"><span data-stu-id="59a47-115">How to configure a label for visual markings for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [<span data-ttu-id="59a47-116">Pregledajte dokumentaciju o zaštiti informacija za Azure</span><span class="sxs-lookup"><span data-stu-id="59a47-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="59a47-117">Korištenje naljepnica s osjetljivosti u aplikacijama Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="59a47-117">Use sensitivity labels in Microsoft 365 apps</span></span>](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

