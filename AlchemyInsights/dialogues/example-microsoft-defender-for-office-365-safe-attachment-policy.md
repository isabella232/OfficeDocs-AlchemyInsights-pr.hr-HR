---
title: Primjeri pravilnika o privitku programa Microsoft Defender za Office 365
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
ms.openlocfilehash: 077762dd37a2974b4e519c1f242fa753623cb49a
ms.sourcegitcommit: 4883f1f89d4c6ca23161e9a43ff206ad21d4f09b
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/08/2021
ms.locfileid: "50692760"
---
# <a name="example-microsoft-defender-for-office-365-safe-attachment-policy"></a><span data-ttu-id="7e956-102">Primjeri pravilnika o privitku programa Microsoft Defender za Office 365</span><span class="sxs-lookup"><span data-stu-id="7e956-102">Example Microsoft Defender for Office 365 Safe Attachment policy</span></span>

<span data-ttu-id="7e956-103">Ove postavke omogućuju pravilo koje se zove *nema kašnjenja* koje odmah dostavljaju poruke, a zatim ponovno prilaže privitke nakon skeniranja:</span><span class="sxs-lookup"><span data-stu-id="7e956-103">These settings enable a policy called *No delays* that delivers messages immediately and then reattaches attachments after they're scanned:</span></span>

- <span data-ttu-id="7e956-104">**Naziv**: nema kašnjenja</span><span class="sxs-lookup"><span data-stu-id="7e956-104">**Name**: No delays</span></span>
- <span data-ttu-id="7e956-105">**Opis**: odmah dostavlja poruke i ponovno prilaže privitke nakon skeniranja.</span><span class="sxs-lookup"><span data-stu-id="7e956-105">**Description**: Delivers messages immediately and reattaches attachments after scanning.</span></span>
- <span data-ttu-id="7e956-106">**Odgovor**: odaberite mogućnost **dinamičke isporuke** .</span><span class="sxs-lookup"><span data-stu-id="7e956-106">**Response**: Select the **Dynamic Delivery** option.</span></span> <span data-ttu-id="7e956-107">Dodatne informacije potražite u članku [dinamička isporuka u pravilima sigurnog privitaka](https://go.microsoft.com/fwlink/?linkid=2092328).</span><span class="sxs-lookup"><span data-stu-id="7e956-107">For more information, see [Dynamic Delivery in Safe Attachments policies](https://go.microsoft.com/fwlink/?linkid=2092328).</span></span>
- <span data-ttu-id="7e956-108">Odjeljak **preusmjeravanje privitaka** : odaberite mogućnost **Omogućivanje preusmjeravanja**, a zatim unesite adresu e-pošte sustava Microsoft 365 Global administrator, administrator sigurnosti ili sigurnosni analitičar koji će istraživati zlonamjerne privitke.</span><span class="sxs-lookup"><span data-stu-id="7e956-108">**Redirect attachment** section: Select the option to **Enable redirect**, and then enter the email address of your Microsoft 365 global administrator, security administrator, or security analyst who will investigate malicious attachments.</span></span>
- <span data-ttu-id="7e956-109">**Primijenjena na** sekciju: odaberite **domenu primatelja**, a zatim odaberite svoju domenu.</span><span class="sxs-lookup"><span data-stu-id="7e956-109">**Applied To** section: Select **The recipient domain is**, and then select your domain.</span></span> <span data-ttu-id="7e956-110">Odaberite **Dodaj**, a zatim odaberite **u redu**.</span><span class="sxs-lookup"><span data-stu-id="7e956-110">Select **add**, and then select **OK**.</span></span> <span data-ttu-id="7e956-111">Kada završite, odaberite **Spremi**.</span><span class="sxs-lookup"><span data-stu-id="7e956-111">Once you're finished, select **Save**.</span></span>

<span data-ttu-id="7e956-112">Dodatne informacije potražite u članku [sigurni privici u programu Microsoft Defender za Office 365](https://go.microsoft.com/fwlink/?linkid=2092213).</span><span class="sxs-lookup"><span data-stu-id="7e956-112">To learn more, see [Safe Attachments in Microsoft Defender for Office 365](https://go.microsoft.com/fwlink/?linkid=2092213).</span></span>
