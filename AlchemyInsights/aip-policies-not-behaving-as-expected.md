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
ms.openlocfilehash: 7926ff9ebbd54969fb5b3ae5d909baffe96a4292
ms.sourcegitcommit: 2afad0b107d03cd8c4de0b85b5bee38a13a7960d
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 05/26/2020
ms.locfileid: "44492954"
---
# <a name="aip-policies-not-behaving-as-expected"></a><span data-ttu-id="5d638-102">AIP: Pravila se ne ponašaju prema očekivanjima</span><span class="sxs-lookup"><span data-stu-id="5d638-102">AIP: Policies not behaving as expected</span></span>

<span data-ttu-id="5d638-103">Azure Information Protection: Pravila se ne ponašaju prema očekivanjima, pogledajte sljedeće za preporučene smjernice za različite probleme s pravilima:</span><span class="sxs-lookup"><span data-stu-id="5d638-103">Azure Information Protection: Policies not behaving as expected, see the following for recommended guidelines for various policy issues:</span></span>

1. <span data-ttu-id="5d638-104">Ako imate problema s vizualnim oznakama, pregledajte [Kada se primjenjuju vizualne oznake](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span><span class="sxs-lookup"><span data-stu-id="5d638-104">If you are having issues with visual markings, please review [When visual markings are applied](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span></span>
2. <span data-ttu-id="5d638-105">Ako imate problema s automatskim označavanjem, pregledajte [Kako konfigurirati uvjete za automatsku i preporučenu klasifikaciju za Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) i Što traže vrste [osjetljivih informacija](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span><span class="sxs-lookup"><span data-stu-id="5d638-105">If you are having issues with automatic labeling, please review [How to configure conditions for automatic and recommended classification for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) and [What the sensitive information types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>
3. <span data-ttu-id="5d638-106">Ako imate problema s zaštitom nativnog/pfile, pregledajte [konfiguraciju API-ja datoteka](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span><span class="sxs-lookup"><span data-stu-id="5d638-106">If you are having issues with Native/Pfile protection, please review [File API configuration](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span></span>
4. <span data-ttu-id="5d638-107">Provjerite koristite li pravila s opsegom koja nisu ispravno konfigurirana: [Konfiguriranje pravila zaštite podataka za Azure za određene korisnike pomoću pravila s opsegom](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span><span class="sxs-lookup"><span data-stu-id="5d638-107">Check if you are using scoped policies that aren't configured properly: [How to configure the Azure Information Protection policy for specific users by using scoped policies](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span></span>
5. <span data-ttu-id="5d638-108">Ako automatsko označavanje ne funkcionira za Outlook prilikom prilaganja označenog dokumenta, provjerite nije li DRMEncryptProperty definiran kao što je ovdje opisano: [Postavke registra IRM-a za sigurnost](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span><span class="sxs-lookup"><span data-stu-id="5d638-108">If automatic labeling isn't working for Outlook when attaching a labeled document, verify that DRMEncryptProperty isn't defined as described here: [IRM registry settings for security](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span></span>

<span data-ttu-id="5d638-109">Ako i dalje imate problema, prikupite zapisnike klijenata za zaštitu podataka usluge Azure i priložite izvezene zapisnike ovoj karti.</span><span class="sxs-lookup"><span data-stu-id="5d638-109">If you still are experiencing issues, please collect Azure Information Protection client logs and attach the exported logs to this ticket.</span></span>

1. <span data-ttu-id="5d638-110">Otvorite dokument sustava Office ili stvorite novu e-poštu u programu Outlook.</span><span class="sxs-lookup"><span data-stu-id="5d638-110">Open an Office document or create a new email in Outlook.</span></span>
2. <span data-ttu-id="5d638-111">Kliknite **Zaštiti/osjetljivost**  >  **Pomoć i povratne informacije**.</span><span class="sxs-lookup"><span data-stu-id="5d638-111">Click **Protect/Sensitivity** > **Help and feedback**.</span></span>
3. <span data-ttu-id="5d638-112">Kliknite **Izvoz zapisnika**.</span><span class="sxs-lookup"><span data-stu-id="5d638-112">Click **Export Logs**.</span></span>
4. <span data-ttu-id="5d638-113">Spremite zapisnike na svoj izbor lokacije i priložite ih ovom zahtjevu za uslugom.</span><span class="sxs-lookup"><span data-stu-id="5d638-113">Save the logs to your choice of location, and attach them to this service request.</span></span>

<span data-ttu-id="5d638-114">Dodatni resursi:</span><span class="sxs-lookup"><span data-stu-id="5d638-114">Additional resources:</span></span>

- [<span data-ttu-id="5d638-115">Konfiguriranje oznake za vizualne oznake za zaštitu informacija za Azure</span><span class="sxs-lookup"><span data-stu-id="5d638-115">How to configure a label for visual markings for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [<span data-ttu-id="5d638-116">Pregled dokumentacije o zaštiti podataka za Azure</span><span class="sxs-lookup"><span data-stu-id="5d638-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="5d638-117">Korištenje oznaka osjetljivosti u aplikacijama sustava Office</span><span class="sxs-lookup"><span data-stu-id="5d638-117">Use sensitivity labels in Office apps</span></span>](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

