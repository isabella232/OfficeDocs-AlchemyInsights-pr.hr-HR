---
title: Omogućivanje lozinke za nepotvrđenim u servisu Azure ad Connect
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
- "9002933"
- "5615"
ms.openlocfilehash: 9dbb88492a3906f6780a345cf880327d411dcc66
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709719"
---
# <a name="enable-password-writeback-in-azure-ad-connect"></a><span data-ttu-id="e548f-102">Omogućivanje lozinke za nepotvrđenim u servisu Azure ad Connect</span><span class="sxs-lookup"><span data-stu-id="e548f-102">Enable password writeback in Azure AD Connect</span></span>

<span data-ttu-id="e548f-103">Da biste omogućili samoposlužnu lozinku za vraćanje izvornih postavki, najprije omogućite mogućnost nepotvrđenim u servisu Azure ad Connect.</span><span class="sxs-lookup"><span data-stu-id="e548f-103">To enable self-service password reset writeback, first enable the writeback option in Azure AD Connect.</span></span> <span data-ttu-id="e548f-104">Na servisu Azure AD Connect Server dovršite sljedeće korake:</span><span class="sxs-lookup"><span data-stu-id="e548f-104">From your Azure AD Connect server, complete the following steps:</span></span>

1. <span data-ttu-id="e548f-105">Prijavite se na poslužitelj za Azure AD Connect i pokrenite čarobnjak za konfiguraciju **Azure ad Connect** .</span><span class="sxs-lookup"><span data-stu-id="e548f-105">Sign in to your Azure AD Connect server and start the **Azure AD Connect** configuration wizard.</span></span>
2. <span data-ttu-id="e548f-106">Na stranici **dobrodošlice** kliknite **Konfiguriraj**.</span><span class="sxs-lookup"><span data-stu-id="e548f-106">On the **Welcome** page, click **Configure**.</span></span>
3. <span data-ttu-id="e548f-107">Na stranici **dodatni zadaci** odaberite **Prilagodi mogućnosti sinkronizacije**, a zatim kliknite **dalje**.</span><span class="sxs-lookup"><span data-stu-id="e548f-107">On the **Additional tasks** page, select **Customize synchronization options**, and then click **Next**.</span></span>
4. <span data-ttu-id="e548f-108">Na stranici **Povezivanje sa servisom Azure** Unesite korisničku vjerodajnicu za Azure, a zatim kliknite dalje.</span><span class="sxs-lookup"><span data-stu-id="e548f-108">On the **Connect to Azure AD** page, enter a global administrator credential for your Azure tenant, and then click Next.</span></span>
5. <span data-ttu-id="e548f-109">Na stranicama **Connect direktorije** i **domene/ou** filtriranje kliknite **dalje**.</span><span class="sxs-lookup"><span data-stu-id="e548f-109">On the **Connect directories** and **Domain/OU** filtering pages, click **Next**.</span></span>
6. <span data-ttu-id="e548f-110">Na stranici **neobavezne značajke** odaberite okvir pokraj stavke **Lozinka nepotvrđenim** i kliknite **dalje**.</span><span class="sxs-lookup"><span data-stu-id="e548f-110">On the **Optional features** page, select the box next to **Password writeback** and click **Next**.</span></span>
7. <span data-ttu-id="e548f-111">Na stranici **spremni za konfiguriranje** kliknite **Konfiguriraj** i pričekajte da se postupak završi.</span><span class="sxs-lookup"><span data-stu-id="e548f-111">On the **Ready to configure** page, click **Configure** and wait for the process to finish.</span></span>
8. <span data-ttu-id="e548f-112">Kada se prikaže kraj konfiguracije, kliknite **izlaz**.</span><span class="sxs-lookup"><span data-stu-id="e548f-112">When you see the configuration finish, click **Exit**.</span></span>

<span data-ttu-id="e548f-113">Ako je u servisu Azure ad Connect omogućeno lozinka nepotvrđenim, sada konfigurirajte Azure ad sspr za nepotvrđenim.</span><span class="sxs-lookup"><span data-stu-id="e548f-113">With password writeback enabled in Azure AD Connect, now configure Azure AD SSPR for writeback.</span></span>  <span data-ttu-id="e548f-114">Da biste omogućili lozinku nepotvrđenim u sspr-u, dovršite sljedeće korake:</span><span class="sxs-lookup"><span data-stu-id="e548f-114">To enable password writeback in SSPR, complete the following steps:</span></span>

1. <span data-ttu-id="e548f-115">Prijavite se na portal Azure pomoću globalnog administratorskog računa.</span><span class="sxs-lookup"><span data-stu-id="e548f-115">Sign in to the Azure portal using a global administrator account.</span></span>
2. <span data-ttu-id="e548f-116">Potražite i odaberite **Azure Active Directory**, kliknite **ponovno postavljanje lozinke**, a zatim odaberite **lokalnu integraciju**.</span><span class="sxs-lookup"><span data-stu-id="e548f-116">Search for and select **Azure Active Directory**, click **Password reset**, then choose **On-premises integration**.</span></span>
3. <span data-ttu-id="e548f-117">Postavite mogućnost za **unos lozinki za vraćanje u lokalni direktorij?** **u da**.</span><span class="sxs-lookup"><span data-stu-id="e548f-117">Set the option for **Write back passwords to your on-premises directory?** to **Yes**.</span></span>
4. <span data-ttu-id="e548f-118">Postavite mogućnost **Dopusti korisnicima da otključaju račune bez ponovnog postavljanja lozinke?** u **da**.</span><span class="sxs-lookup"><span data-stu-id="e548f-118">Set the option for **Allow users to unlock accounts without resetting their password?** to **Yes**.</span></span>
5. <span data-ttu-id="e548f-119">Kada ste spremni, kliknite **Spremi**.</span><span class="sxs-lookup"><span data-stu-id="e548f-119">When ready, click **Save**.</span></span>

<span data-ttu-id="e548f-120">Dodatne informacije potražite u članku [Omogućivanje izvorne lozinke za samoposluživanje u servisu Azure Active Directory ponovno postavljanje programa nepotvrđenim u lokalno okruženje](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).</span><span class="sxs-lookup"><span data-stu-id="e548f-120">For more information, see [Enable Azure Active Directory self-service password reset writeback to an on-premises environment](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).</span></span>
