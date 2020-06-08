---
title: Omogući vraćanje lozinkom u servisu Azure AD Connect
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002933"
- "5615"
ms.openlocfilehash: ab4b8692799d08363e1d726f72a3b80dcb598797
ms.sourcegitcommit: 0cf8d133d6feade6df8b1082444ce73faa91e145
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 05/13/2020
ms.locfileid: "44204617"
---
# <a name="enable-password-writeback-in-azure-ad-connect"></a><span data-ttu-id="44ddc-102">Omogući vraćanje lozinkom u servisu Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="44ddc-102">Enable password writeback in Azure AD Connect</span></span>

<span data-ttu-id="44ddc-103">Da biste omogućili ponovno pisanje samoposlužne lozinke, najprije omogućite mogućnost vraćanja na otpis u usluzi Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="44ddc-103">To enable self-service password reset writeback, first enable the writeback option in Azure AD Connect.</span></span> <span data-ttu-id="44ddc-104">Na poslužitelju Azure AD Connect učinite sljedeće:</span><span class="sxs-lookup"><span data-stu-id="44ddc-104">From your Azure AD Connect server, complete the following steps:</span></span>

1. <span data-ttu-id="44ddc-105">Prijavite se na poslužitelj Azure AD Connect i pokrenite čarobnjak za konfiguraciju **usluge Azure AD Connect.**</span><span class="sxs-lookup"><span data-stu-id="44ddc-105">Sign in to your Azure AD Connect server and start the **Azure AD Connect** configuration wizard.</span></span>
2. <span data-ttu-id="44ddc-106">Na stranici **Dobrodošlice** kliknite **Konfiguriraj**.</span><span class="sxs-lookup"><span data-stu-id="44ddc-106">On the **Welcome** page, click **Configure**.</span></span>
3. <span data-ttu-id="44ddc-107">Na stranici **Dodatni zadaci** odaberite Prilagodi **mogućnosti sinkronizacije**, a zatim kliknite **Dalje**.</span><span class="sxs-lookup"><span data-stu-id="44ddc-107">On the **Additional tasks** page, select **Customize synchronization options**, and then click **Next**.</span></span>
4. <span data-ttu-id="44ddc-108">Na **stranici Povezivanje s Azure AD** unesite vjerodajnice globalnog administratora za klijenta azure, a zatim kliknite Dalje.</span><span class="sxs-lookup"><span data-stu-id="44ddc-108">On the **Connect to Azure AD** page, enter a global administrator credential for your Azure tenant, and then click Next.</span></span>
5. <span data-ttu-id="44ddc-109">Na stranicama **povezivanje direktorija** i **domena/OU** filtriranja kliknite **Dalje**.</span><span class="sxs-lookup"><span data-stu-id="44ddc-109">On the **Connect directories** and **Domain/OU** filtering pages, click **Next**.</span></span>
6. <span data-ttu-id="44ddc-110">Na stranici **Neobavezne značajke** potvrdite okvir pokraj stavke **Povratni zapis lozinke** i kliknite **Dalje**.</span><span class="sxs-lookup"><span data-stu-id="44ddc-110">On the **Optional features** page, select the box next to **Password writeback** and click **Next**.</span></span>
7. <span data-ttu-id="44ddc-111">Na **stranici Spremno za konfiguriranje** kliknite **Konfiguriraj** i pričekajte da se postupak završi.</span><span class="sxs-lookup"><span data-stu-id="44ddc-111">On the **Ready to configure** page, click **Configure** and wait for the process to finish.</span></span>
8. <span data-ttu-id="44ddc-112">Kada vidite da je konfiguracija dovršena, kliknite **Izlaz**.</span><span class="sxs-lookup"><span data-stu-id="44ddc-112">When you see the configuration finish, click **Exit**.</span></span>

<span data-ttu-id="44ddc-113">Uz omogućen povratni unos lozinke u servisu Azure AD Connect, sada konfigurirajte Azure AD SSPR za povratni zapis.</span><span class="sxs-lookup"><span data-stu-id="44ddc-113">With password writeback enabled in Azure AD Connect, now configure Azure AD SSPR for writeback.</span></span>  <span data-ttu-id="44ddc-114">Da biste omogućili vraćanje lozinke u SSPR-u, poduzmite sljedeće korake:</span><span class="sxs-lookup"><span data-stu-id="44ddc-114">To enable password writeback in SSPR, complete the following steps:</span></span>

1. <span data-ttu-id="44ddc-115">Prijavite se na portal Azure pomoću globalnog administratorskog računa.</span><span class="sxs-lookup"><span data-stu-id="44ddc-115">Sign in to the Azure portal using a global administrator account.</span></span>
2. <span data-ttu-id="44ddc-116">Potražite i odaberite **Azure Active Directory**, kliknite Ponovno postavljanje **lozinke**, a zatim odaberite **Lokalna integracija**.</span><span class="sxs-lookup"><span data-stu-id="44ddc-116">Search for and select **Azure Active Directory**, click **Password reset**, then choose **On-premises integration**.</span></span>
3. <span data-ttu-id="44ddc-117">Postavite opciju za **Vraćanje lozinki u lokalni direktorij?** **Yes**</span><span class="sxs-lookup"><span data-stu-id="44ddc-117">Set the option for **Write back passwords to your on-premises directory?** to **Yes**.</span></span>
4. <span data-ttu-id="44ddc-118">Postavite opciju za **Dopusti korisnicima otključavanje računa bez ponovnog postavljanja lozinke?** **Yes**</span><span class="sxs-lookup"><span data-stu-id="44ddc-118">Set the option for **Allow users to unlock accounts without resetting their password?** to **Yes**.</span></span>
5. <span data-ttu-id="44ddc-119">Kada ste spremni, kliknite **Spremi**.</span><span class="sxs-lookup"><span data-stu-id="44ddc-119">When ready, click **Save**.</span></span>

<span data-ttu-id="44ddc-120">Dodatne informacije [potražite u odjeljku Omogućivanje ponovnog vraćanja ponovnog postavljanja samoposlužne lozinke servisa Azure Active Directory u lokalno okruženje](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).</span><span class="sxs-lookup"><span data-stu-id="44ddc-120">For more information, see [Enable Azure Active Directory self-service password reset writeback to an on-premises environment](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).</span></span>
