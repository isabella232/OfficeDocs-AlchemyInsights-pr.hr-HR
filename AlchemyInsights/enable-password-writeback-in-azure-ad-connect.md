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
ms.openlocfilehash: 0eecd89b2558359702935379d7ffbd8b7508f4cd
ms.sourcegitcommit: 62a83a1c6bd9779a1a11b749490bd11670d4b063
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 12/02/2020
ms.locfileid: "49560432"
---
# <a name="enable-password-writeback-in-azure-ad-connect"></a><span data-ttu-id="291eb-102">Omogućivanje lozinke za nepotvrđenim u servisu Azure ad Connect</span><span class="sxs-lookup"><span data-stu-id="291eb-102">Enable password writeback in Azure AD Connect</span></span>

<span data-ttu-id="291eb-103">Da biste omogućili samoposlužnu lozinku za vraćanje izvornih postavki, najprije omogućite mogućnost nepotvrđenim u servisu Azure ad Connect.</span><span class="sxs-lookup"><span data-stu-id="291eb-103">To enable self-service password reset writeback, first enable the writeback option in Azure AD Connect.</span></span> <span data-ttu-id="291eb-104">Na servisu Azure AD Connect Server dovršite sljedeće korake:</span><span class="sxs-lookup"><span data-stu-id="291eb-104">From your Azure AD Connect server, complete the following steps:</span></span>

1. <span data-ttu-id="291eb-105">Prijavite se na poslužitelj za Azure AD Connect i pokrenite čarobnjak za konfiguraciju **Azure ad Connect** .</span><span class="sxs-lookup"><span data-stu-id="291eb-105">Sign in to your Azure AD Connect server and start the **Azure AD Connect** configuration wizard.</span></span>
2. <span data-ttu-id="291eb-106">Na stranici **dobrodošlice** kliknite **Konfiguriraj**.</span><span class="sxs-lookup"><span data-stu-id="291eb-106">On the **Welcome** page, click **Configure**.</span></span>
3. <span data-ttu-id="291eb-107">Na stranici **dodatni zadaci** odaberite **Prilagodi mogućnosti sinkronizacije**, a zatim kliknite **dalje**.</span><span class="sxs-lookup"><span data-stu-id="291eb-107">On the **Additional tasks** page, select **Customize synchronization options**, and then click **Next**.</span></span>
4. <span data-ttu-id="291eb-108">Na stranici **Povezivanje sa servisom Azure** Unesite korisničku vjerodajnicu za Azure, a zatim kliknite **dalje**.</span><span class="sxs-lookup"><span data-stu-id="291eb-108">On the **Connect to Azure AD** page, enter a global administrator credential for your Azure tenant, and then click **Next**.</span></span>
5. <span data-ttu-id="291eb-109">Na stranicama **Connect direktorije** i **domene/ou** filtriranje kliknite **dalje**.</span><span class="sxs-lookup"><span data-stu-id="291eb-109">On the **Connect directories** and **Domain/OU** filtering pages, click **Next**.</span></span>
6. <span data-ttu-id="291eb-110">Na stranici **neobavezne značajke** odaberite okvir pokraj stavke **Lozinka nepotvrđenim** i kliknite **dalje**.</span><span class="sxs-lookup"><span data-stu-id="291eb-110">On the **Optional features** page, select the box next to **Password writeback** and click **Next**.</span></span>
7. <span data-ttu-id="291eb-111">Na stranici **spremni za konfiguriranje** kliknite **Konfiguriraj** i pričekajte da se postupak završi.</span><span class="sxs-lookup"><span data-stu-id="291eb-111">On the **Ready to configure** page, click **Configure** and wait for the process to finish.</span></span>
8. <span data-ttu-id="291eb-112">Kada se prikaže kraj konfiguracije, kliknite **izlaz**.</span><span class="sxs-lookup"><span data-stu-id="291eb-112">When you see the configuration finish, click **Exit**.</span></span>

<span data-ttu-id="291eb-113">Ako je u servisu Azure ad Connect omogućeno lozinka nepotvrđenim, konfigurirajte Azure ad sspr za nepotvrđenim.</span><span class="sxs-lookup"><span data-stu-id="291eb-113">With password writeback enabled in Azure AD Connect, configure Azure AD SSPR for writeback.</span></span>  <span data-ttu-id="291eb-114">Da biste omogućili lozinku nepotvrđenim u sspr-u, dovršite sljedeće korake:</span><span class="sxs-lookup"><span data-stu-id="291eb-114">To enable password writeback in SSPR, complete the following steps:</span></span>

1. <span data-ttu-id="291eb-115">Prijavite se na portal Azure pomoću globalnog administratorskog računa.</span><span class="sxs-lookup"><span data-stu-id="291eb-115">Sign in to the Azure portal using a global administrator account.</span></span>
2. <span data-ttu-id="291eb-116">Potražite i odaberite **Azure Active Directory**, kliknite **ponovno postavljanje lozinke**, a zatim **lokalne integracije**.</span><span class="sxs-lookup"><span data-stu-id="291eb-116">Search for and select **Azure Active Directory**, click **Password reset**, then click **On-premises integration**.</span></span>
3. <span data-ttu-id="291eb-117">Postavite mogućnost za **unos lozinki za vraćanje u lokalni direktorij?** **u da**.</span><span class="sxs-lookup"><span data-stu-id="291eb-117">Set the option for **Write back passwords to your on-premises directory?** to **Yes**.</span></span>
4. <span data-ttu-id="291eb-118">Postavite mogućnost **Dopusti korisnicima da otključaju račune bez ponovnog postavljanja lozinke?** u **da**.</span><span class="sxs-lookup"><span data-stu-id="291eb-118">Set the option for **Allow users to unlock accounts without resetting their password?** to **Yes**.</span></span>
5. <span data-ttu-id="291eb-119">Kada ste spremni, kliknite **Spremi**.</span><span class="sxs-lookup"><span data-stu-id="291eb-119">When ready, click **Save**.</span></span>

<span data-ttu-id="291eb-120">Dodatne informacije potražite u članku [Omogućivanje izvorne lozinke za samoposluživanje u servisu Azure Active Directory ponovno postavljanje programa nepotvrđenim u lokalno okruženje](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).</span><span class="sxs-lookup"><span data-stu-id="291eb-120">For more information, see [Enable Azure Active Directory self-service password reset writeback to an on-premises environment](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).</span></span>

> [!NOTE]
>  <span data-ttu-id="291eb-121">Ako administrator ponovno postavi korisnikovu lozinku na portalu Azure, ako je taj korisnik sinkroniziran ili je postavljen za lozinku, lozinka će biti napisana natrag na lokalno.</span><span class="sxs-lookup"><span data-stu-id="291eb-121">When an administrator resets a user's password in the Azure Portal, if that user is federated or password hash synchronized, the password is written back to on-premises.</span></span> <span data-ttu-id="291eb-122">Ova funkcionalnost trenutno nije podržana na portalu za administratore sustava Office.</span><span class="sxs-lookup"><span data-stu-id="291eb-122">This functionality is currently not supported in the Office Admin portal.</span></span>