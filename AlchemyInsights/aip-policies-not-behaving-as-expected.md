---
title: 'AIP: pravila se ne ponašaju prema očekivanom'
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4780"
ms.openlocfilehash: 7baa010cc0b18b5d2a295623639fabf2bc5f88ec
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821619"
---
# <a name="aip-policies-not-behaving-as-expected"></a><span data-ttu-id="a624c-102">AIP: pravila se ne ponašaju prema očekivanom</span><span class="sxs-lookup"><span data-stu-id="a624c-102">AIP: Policies not behaving as expected</span></span>

<span data-ttu-id="a624c-103">Azure Information Protection: pravila koja se ne ponašaju prema očekivanom, potražite u nastavku preporučene smjernice za razne probleme s pravilnikom:</span><span class="sxs-lookup"><span data-stu-id="a624c-103">Azure Information Protection: Policies not behaving as expected, see the following for recommended guidelines for various policy issues:</span></span>

1. <span data-ttu-id="a624c-104">Ako imate problema s vizualnim oznakama, pregledajte Kada se primjenjuju [vizualne oznake](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span><span class="sxs-lookup"><span data-stu-id="a624c-104">If you are having issues with visual markings, please review [When visual markings are applied](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span></span>
2. <span data-ttu-id="a624c-105">Ako imate problema s automatskim označavanjem, pročitajte upute za konfiguriranje uvjeta za automatsku i preporučenu klasifikaciju za [Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) i Što [osjetljive vrste podataka izgledaju](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span><span class="sxs-lookup"><span data-stu-id="a624c-105">If you are having issues with automatic labeling, please review [How to configure conditions for automatic and recommended classification for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) and [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>
3. <span data-ttu-id="a624c-106">Ako imate problema sa zaštitom Native/Pfile, pregledajte [konfiguraciju API-ja za datoteke.](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration)</span><span class="sxs-lookup"><span data-stu-id="a624c-106">If you are having issues with Native/Pfile protection, please review [File API configuration](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span></span>
4. <span data-ttu-id="a624c-107">Provjerite koristite li pravilnike s opsegom koji nisu pravilno konfigurirani: Konfiguriranje pravilnika o zaštiti podataka za Azure za određene korisnike [pomoću pravilnika s opsegom](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span><span class="sxs-lookup"><span data-stu-id="a624c-107">Check if you are using scoped policies that aren't configured properly: [How to configure the Azure Information Protection policy for specific users by using scoped policies](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span></span>
5. <span data-ttu-id="a624c-108">Ako automatsko označavanje ne funkcionira za Outlook prilikom prilaganja označenog dokumenta, provjerite nije li DRMEncryptProperty definiran ovdje: [postavke registra IRM za sigurnost](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span><span class="sxs-lookup"><span data-stu-id="a624c-108">If automatic labeling isn't working for Outlook when attaching a labeled document, verify that DRMEncryptProperty isn't defined as described here: [IRM registry settings for security](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span></span>

<span data-ttu-id="a624c-109">Ako i dalje nailazite na probleme, prikupite zapisnike klijenta za Azure Information Protection i priložite izvezene zapisnike na ovu kartu.</span><span class="sxs-lookup"><span data-stu-id="a624c-109">If you still are experiencing issues, please collect Azure Information Protection client logs and attach the exported logs to this ticket.</span></span>

1. <span data-ttu-id="a624c-110">Otvorite dokument sustava Office ili stvorite novu e-poštu u programu Outlook.</span><span class="sxs-lookup"><span data-stu-id="a624c-110">Open an Office document or create a new email in Outlook.</span></span>
2. <span data-ttu-id="a624c-111">Kliknite **Zaštita/osjetljivost Pomoć i**  >  **povratne informacije**.</span><span class="sxs-lookup"><span data-stu-id="a624c-111">Click **Protect/Sensitivity** > **Help and feedback**.</span></span>
3. <span data-ttu-id="a624c-112">Kliknite **Izvezi zapisnike**.</span><span class="sxs-lookup"><span data-stu-id="a624c-112">Click **Export Logs**.</span></span>
4. <span data-ttu-id="a624c-113">Spremite zapisnike na odabir mjesta i priložite ih tom zahtjevu za uslugu.</span><span class="sxs-lookup"><span data-stu-id="a624c-113">Save the logs to your choice of location, and attach them to this service request.</span></span>

<span data-ttu-id="a624c-114">Dodatni resursi:</span><span class="sxs-lookup"><span data-stu-id="a624c-114">Additional resources:</span></span>

- [<span data-ttu-id="a624c-115">Konfiguriranje oznake za vizualne oznake za Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="a624c-115">How to configure a label for visual markings for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [<span data-ttu-id="a624c-116">Pregled dokumentacije za Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="a624c-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="a624c-117">Korištenje oznaka osjetljivosti u aplikacijama microsoft 365</span><span class="sxs-lookup"><span data-stu-id="a624c-117">Use sensitivity labels in Microsoft 365 apps</span></span>](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

