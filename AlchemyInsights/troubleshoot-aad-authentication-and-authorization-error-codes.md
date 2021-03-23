---
title: Otklanjanje poteškoća s kodom pogreške Azure AD i autorizacija (AADSTS)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9800"
- "9005744"
ms.openlocfilehash: 14555dfcb1406fd3a3977012393714a713ff80dc
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035197"
---
# <a name="troubleshoot-azure-ad-authentication-and-authorization-aadsts-error-codes"></a><span data-ttu-id="a146f-102">Otklanjanje poteškoća s kodom pogreške Azure AD i autorizacija (AADSTS)</span><span class="sxs-lookup"><span data-stu-id="a146f-102">Troubleshoot Azure AD Authentication and Authorization (AADSTS) error codes</span></span>

<span data-ttu-id="a146f-103">Da biste riješili provjeru autentičnosti AAD i šifre pogrešaka autorizacije (AADSTS), izvedite sljedeće preporučene korake:</span><span class="sxs-lookup"><span data-stu-id="a146f-103">To resolve AAD authentication and authorization error codes (AADSTS), perform the following recommended steps:</span></span>

1. <span data-ttu-id="a146f-104">**Rješavanje kodova pogrešaka u aplikaciji**</span><span class="sxs-lookup"><span data-stu-id="a146f-104">**Handling error codes in your application**</span></span>

- <span data-ttu-id="a146f-105">**Spec. OAuth 2.0**, https://tools.ietf.org/html/rfc6749#section-5.2 nudi smjernice o tome kako obraditi pogreške tijekom provjere autentičnosti pomoću dijela pogreške u odgovoru na pogrešku.</span><span class="sxs-lookup"><span data-stu-id="a146f-105">The **OAuth2.0 spec**, https://tools.ietf.org/html/rfc6749#section-5.2, provides guidance on how to handle errors during authentication using the error portion of the error response.</span></span>

    - <span data-ttu-id="a146f-106">**pogreška**: niz kod pogreške koji se može koristiti za klasificiranje vrsta pogrešaka koje se javljaju i moraju se koristiti za reakcije na pogreške.</span><span class="sxs-lookup"><span data-stu-id="a146f-106">**error**: An error code string that can be used to classify types of errors that occur, and should be used to react to errors.</span></span>
    - <span data-ttu-id="a146f-107">Polje **pogreške** sadrži nekoliko mogućih vrijednosti – pregledajte veze s dokumentacijom protokola i specifikacije OAuth 2,0 da biste saznali više o određenim pogreškama i kako reagirati na njih.</span><span class="sxs-lookup"><span data-stu-id="a146f-107">The **error** field has several possible values - review the protocol documentation links and OAuth 2.0 specs for more information about specific errors and how to react to them.</span></span>

- <span data-ttu-id="a146f-108">Ovdje je ogledni odgovor o pogrešci:</span><span class="sxs-lookup"><span data-stu-id="a146f-108">Here is a sample error response:</span></span>
```
{
  "error": "invalid_scope",
  "error_description": "AADSTS70011: The provided value for the input parameter 'scope' is not 
valid. The scope https://example.contoso.com/activity.read is not valid.\r\nTrace ID: 255d1aef- 8c98-452f-ac51-23d051240864\r\nCorrelation ID: fb3d2015-bc17-4bb9-bb85-30c5cf1aaaa7\r\nTimestamp: 2016-01-09 02:02:12Z",
  "error_codes": [
    70011
  ],
  "timestamp": "2016-01-09 02:02:12Z",
  "trace_id": "255d1aef-8c98-452f-ac51-23d051240864",
  "correlation_id": "fb3d2015-bc17-4bb9-bb85-30c5cf1aaaa7", 
  "error_uri":"https://login.microsoftonline.com/error?code=70011"
}
```
2. <span data-ttu-id="a146f-109">**Podaci o postojećem kodu pogreške**</span><span class="sxs-lookup"><span data-stu-id="a146f-109">**Lookup current error code information**</span></span>

- <span data-ttu-id="a146f-110">Kodovi pogrešaka i poruke podložni su promjeni.</span><span class="sxs-lookup"><span data-stu-id="a146f-110">Error codes and messages are subject to change.</span></span> <span data-ttu-id="a146f-111">Najnovije informacije potražite u članku https://login.microsoftonline.com/error Pronalaženje AADSTS opisa pogrešaka, popravaka i nekih predloženih zaobilaznih rješenja.</span><span class="sxs-lookup"><span data-stu-id="a146f-111">For the most current information, see the https://login.microsoftonline.com/error page to find AADSTS error descriptions, fixes, and some suggested workarounds.</span></span>
- <span data-ttu-id="a146f-112">Možete potražiti i otkloniti [šifre pogrešaka Aadsts](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#aadsts-error-codes) navedenih u odjeljku članak [Provjera autentičnosti oglasa i pogreške autorizacije](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#handling-error-codes-in-your-application).</span><span class="sxs-lookup"><span data-stu-id="a146f-112">You can also search for and troubleshoot [AADSTS error codes](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#aadsts-error-codes) listed in the article [Azure AD Authentication and authorization error codes](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#handling-error-codes-in-your-application).</span></span>

3. <span data-ttu-id="a146f-113">**Pomoć**</span><span class="sxs-lookup"><span data-stu-id="a146f-113">**Get Help**</span></span>

- <span data-ttu-id="a146f-114">[Mogućnosti podrške i pomoći za razvojne inženjere](https://docs.microsoft.com/azure/active-directory/develop/developer-support-help-options) – ako vam je potreban odgovor na pitanje ili pomoć u rješavanju problema koji nije pokriven našom dokumentacijom, možda je vrijeme da se obratite stručnjacima za pomoć.</span><span class="sxs-lookup"><span data-stu-id="a146f-114">[Support and help options for developers](https://docs.microsoft.com/azure/active-directory/develop/developer-support-help-options) - If you need an answer to a question or help in solving a problem not covered in our documentation, it might be time to reach out to experts for help.</span></span> <span data-ttu-id="a146f-115">U ovom se članku nudi nekoliko prijedloga za dobivanje odgovora na pitanja prilikom razvoja aplikacija koje se integriraju u Microsoftovu platformu identiteta.</span><span class="sxs-lookup"><span data-stu-id="a146f-115">This article provides several suggestions for getting answers to your questions as you develop apps that integrate with the Microsoft identity platform.</span></span>








