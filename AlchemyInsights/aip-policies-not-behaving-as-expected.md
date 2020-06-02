---
title: 'AIP: Pravila se ne ponašaju prema očekivanjima'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4780"
ms.openlocfilehash: 527556fcb02525eb88ea992c38a2ddfcba6f9453
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: HT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506550"
---
# <a name="aip-policies-not-behaving-as-expected"></a><span data-ttu-id="6bd7f-102">AIP: Pravila se ne ponašaju prema očekivanjima</span><span class="sxs-lookup"><span data-stu-id="6bd7f-102">AIP: Policies not behaving as expected</span></span>

<span data-ttu-id="6bd7f-103">Azure Information Protection: Pravila se ne ponašaju prema očekivanjima, pogledajte sljedeće za preporučene smjernice za različite probleme s pravilima:</span><span class="sxs-lookup"><span data-stu-id="6bd7f-103">Azure Information Protection: Policies not behaving as expected, see the following for recommended guidelines for various policy issues:</span></span>

1. <span data-ttu-id="6bd7f-104">Ako imate problema s vizualnim oznakama, pregledajte [Kada se primjenjuju vizualne oznake](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span><span class="sxs-lookup"><span data-stu-id="6bd7f-104">If you are having issues with visual markings, please review [When visual markings are applied](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span></span>
2. <span data-ttu-id="6bd7f-105">Ako imate problema s automatskim označavanjem, pregledajte [Kako konfigurirati uvjete za automatsku i preporučenu klasifikaciju za Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) i Što traže vrste [osjetljivih informacija](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span><span class="sxs-lookup"><span data-stu-id="6bd7f-105">If you are having issues with automatic labeling, please review [How to configure conditions for automatic and recommended classification for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) and [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>
3. <span data-ttu-id="6bd7f-106">Ako imate problema s zaštitom nativnog/pfile, pregledajte [konfiguraciju API-ja datoteka](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span><span class="sxs-lookup"><span data-stu-id="6bd7f-106">If you are having issues with Native/Pfile protection, please review [File API configuration](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span></span>
4. <span data-ttu-id="6bd7f-107">Provjerite koristite li pravila s opsegom koja nisu ispravno konfigurirana: [Konfiguriranje pravila zaštite podataka za Azure za određene korisnike pomoću pravila s opsegom](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span><span class="sxs-lookup"><span data-stu-id="6bd7f-107">Check if you are using scoped policies that aren't configured properly: [How to configure the Azure Information Protection policy for specific users by using scoped policies](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span></span>
5. <span data-ttu-id="6bd7f-108">Ako automatsko označavanje ne funkcionira za Outlook prilikom prilaganja označenog dokumenta, provjerite nije li DRMEncryptProperty definiran kao što je ovdje opisano: [Postavke registra IRM-a za sigurnost](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span><span class="sxs-lookup"><span data-stu-id="6bd7f-108">If automatic labeling isn't working for Outlook when attaching a labeled document, verify that DRMEncryptProperty isn't defined as described here: [IRM registry settings for security](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span></span>

<span data-ttu-id="6bd7f-109">Ako i dalje imate problema, prikupite zapisnike klijenata za zaštitu podataka usluge Azure i priložite izvezene zapisnike ovoj karti.</span><span class="sxs-lookup"><span data-stu-id="6bd7f-109">If you still are experiencing issues, please collect Azure Information Protection client logs and attach the exported logs to this ticket.</span></span>

1. <span data-ttu-id="6bd7f-110">Otvorite dokument sustava Office ili stvorite novu e-poštu u programu Outlook.</span><span class="sxs-lookup"><span data-stu-id="6bd7f-110">Open an Office document or create a new email in Outlook.</span></span>
2. <span data-ttu-id="6bd7f-111">Kliknite **Zaštiti/osjetljivost**  >  **Pomoć i povratne informacije**.</span><span class="sxs-lookup"><span data-stu-id="6bd7f-111">Click **Protect/Sensitivity** > **Help and feedback**.</span></span>
3. <span data-ttu-id="6bd7f-112">Kliknite **Izvoz zapisnika**.</span><span class="sxs-lookup"><span data-stu-id="6bd7f-112">Click **Export Logs**.</span></span>
4. <span data-ttu-id="6bd7f-113">Spremite zapisnike na svoj izbor lokacije i priložite ih ovom zahtjevu za uslugom.</span><span class="sxs-lookup"><span data-stu-id="6bd7f-113">Save the logs to your choice of location, and attach them to this service request.</span></span>

<span data-ttu-id="6bd7f-114">Dodatni resursi:</span><span class="sxs-lookup"><span data-stu-id="6bd7f-114">Additional resources:</span></span>

- [<span data-ttu-id="6bd7f-115">Konfiguriranje oznake za vizualne oznake za zaštitu informacija za Azure</span><span class="sxs-lookup"><span data-stu-id="6bd7f-115">How to configure a label for visual markings for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [<span data-ttu-id="6bd7f-116">Pregled dokumentacije o zaštiti podataka za Azure</span><span class="sxs-lookup"><span data-stu-id="6bd7f-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="6bd7f-117">Korištenje oznaka osjetljivosti u aplikacijama sustava Office</span><span class="sxs-lookup"><span data-stu-id="6bd7f-117">Use sensitivity labels in Office apps</span></span>](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

