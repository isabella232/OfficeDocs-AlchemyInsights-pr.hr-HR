---
title: Nije se moguće prijaviti u aplikaciju Teams zbog pogreške autologon.microsoftazuread-sso.com:443
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "9001686"
- "3750"
ms.openlocfilehash: 77049153939989d1c63789adfec0b494d047a6e4
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931831"
---
# <a name="unable-to-log-into-teams-due-to-error-autologonmicrosoftazuread-sso-dot-com443"></a><span data-ttu-id="9d262-102">Nije se moguće prijaviti u aplikaciju Teams zbog pogreške autologon.microsoftazuread-sso dot com:443</span><span class="sxs-lookup"><span data-stu-id="9d262-102">Unable to log into Teams due to error autologon.microsoftazuread-sso dot com:443</span></span>

<span data-ttu-id="9d262-103">Ako je kao provjera autentičnosti O365 omogućen besprijekorni SSO, možda će se na intranetska web-mjesta morati dodati URL "autologon.microsoftazuread-sso.com".</span><span class="sxs-lookup"><span data-stu-id="9d262-103">If Seamless SSO is enabled as the O365 authentication, the URL "autologon.microsoftazuread-sso.com" may need to be added to Intranet Sites.</span></span>  <span data-ttu-id="9d262-104">Ako je prethodno dodan na pouzdana web-mjesta, a u programu se koristi besprijekorni SSO, mora se ukloniti s pouzdanih web-mjesta.</span><span class="sxs-lookup"><span data-stu-id="9d262-104">If it has previously been added to Trusted Sites  and Seamless SSO is in use, it should be removed from Trusted Sites.</span></span>

<span data-ttu-id="9d262-105">Pregledajte [kontrolni popis za otklanjanje poteškoća s besprijekornim SSO](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso#troubleshooting-checklist).</span><span class="sxs-lookup"><span data-stu-id="9d262-105">Please review the [Seamless SSO Troubleshooting Checklist](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso#troubleshooting-checklist).</span></span>

<span data-ttu-id="9d262-106">Slijedite korake u nastavku da biste dodali URL na popis intranetskih web-mjesta:</span><span class="sxs-lookup"><span data-stu-id="9d262-106">Follow these steps to add a URL to Intranet Sites list:</span></span>

1. <span data-ttu-id="9d262-107">Otvorite Internet Explorer tako da kliknete gumb **početak**.</span><span class="sxs-lookup"><span data-stu-id="9d262-107">Open Internet Explorer by clicking the **Start** button.</span></span> <span data-ttu-id="9d262-108">U okvir za pretraživanje unesite Internet Explorer, a zatim na popisu rezultata kliknite **Internet Explorer**.</span><span class="sxs-lookup"><span data-stu-id="9d262-108">In the search box, type Internet Explorer, and then, in the list of results, click **Internet Explorer**.</span></span>
2. <span data-ttu-id="9d262-109">Kliknite **Alati** pa odaberite **Internetske mogućnosti**.</span><span class="sxs-lookup"><span data-stu-id="9d262-109">Click **Tools**, and then click **Internet options**.</span></span>
3. <span data-ttu-id="9d262-110">Kliknite karticu **Sigurnost**.</span><span class="sxs-lookup"><span data-stu-id="9d262-110">Click the **Security** tab.</span></span>
4. <span data-ttu-id="9d262-111">Sada kliknite na **lokalna intranetska web-mjesta** a zatim kliknite gumb **web-mjesta**, te **gumb Napredno**.</span><span class="sxs-lookup"><span data-stu-id="9d262-111">Now click on **Local Intranet sites** and then click on the **sites** button and then **Advanced** button.</span></span>
5. <span data-ttu-id="9d262-112">Unesite URL web-mjesta, a zatim kliknite **dodajte**.</span><span class="sxs-lookup"><span data-stu-id="9d262-112">Enter the Website URL and click **Add**.</span></span>
6. <span data-ttu-id="9d262-113">Kada završite, kliknite **Zatvori**.</span><span class="sxs-lookup"><span data-stu-id="9d262-113">When you are finished, click **Close**.</span></span>

<span data-ttu-id="9d262-114">Dodatne informacije potražite u članku [Dokumentacija za implementaciju besprijekornih SSO-a za O365](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start) (uključuje proces utemeljen na pravilniku da biste URL dodali na intranetska web-mjesta u koraku 3).</span><span class="sxs-lookup"><span data-stu-id="9d262-114">For more information, see [Documentation for deploying Seamless SSO for O365](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start) (includes Policy-based process to add a URL to Intranet Sites in Step 3).</span></span>
