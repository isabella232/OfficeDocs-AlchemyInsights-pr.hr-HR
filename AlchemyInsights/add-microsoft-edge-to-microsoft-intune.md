---
title: Dodavanje programa Microsoft Edge u Microsoft Intune
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/10/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8240"
- "9004604"
ms.openlocfilehash: d56c65910d1c2170d3e0ce9676e913663701db96
ms.sourcegitcommit: 03378c78eadac5d950802dcbacc328bca3314032
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 02/10/2021
ms.locfileid: "50194460"
---
# <a name="add-microsoft-edge-to-microsoft-intune"></a><span data-ttu-id="d35ca-102">Dodavanje programa Microsoft Edge u Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="d35ca-102">Add Microsoft Edge to Microsoft Intune</span></span>

<span data-ttu-id="d35ca-103">Da biste mogli implementirati, konfigurirati, nadzirati i štititi Microsoft Edge za Windows 10, najprije ga morate dodati u Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="d35ca-103">To be able to deploy, configure, monitor, and protect Microsoft Edge for Windows 10, you must first add it to Microsoft Intune.</span></span>

> [!IMPORTANT]
- <span data-ttu-id="d35ca-104">Intune podržava Microsoft Edge 77 i novije verzije.</span><span class="sxs-lookup"><span data-stu-id="d35ca-104">Intune supports Microsoft Edge 77 and later versions.</span></span>
- <span data-ttu-id="d35ca-105">Intune će otkrivati bilo koje postojeće instalacije sustava Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="d35ca-105">Intune will detect any pre-existing installations of Microsoft Edge.</span></span>
- <span data-ttu-id="d35ca-106">Ako je Microsoft Edge instaliran u kontekstu korisničkog konteksta, instalacija sustava prebrisat će instalaciju u kontekstu korisničkog konteksta.</span><span class="sxs-lookup"><span data-stu-id="d35ca-106">If Microsoft Edge is installed in user context, a system installation will overwrite the installation in user context.</span></span>
- <span data-ttu-id="d35ca-107">Ako je Microsoft Edge instaliran u kontekstu sustava, prikazat će se uspješan instalacijski program.</span><span class="sxs-lookup"><span data-stu-id="d35ca-107">If Microsoft Edge is installed in system context, the installation success will be reported.</span></span>
- <span data-ttu-id="d35ca-108">Unaprijed instalirani Microsoft Edge 77 i novije verzije, za sve kanale u kontekstu korisnika, prebrisat će se uz Microsoft Edge instaliran u kontekstu sustava.</span><span class="sxs-lookup"><span data-stu-id="d35ca-108">Pre-installed Microsoft Edge 77 and later versions, for all channels in user context, will be overwritten with Microsoft Edge installed in system context.</span></span>

<span data-ttu-id="d35ca-109">**Preduvjet**</span><span class="sxs-lookup"><span data-stu-id="d35ca-109">**Prerequisite**</span></span>

<span data-ttu-id="d35ca-110">Windows 10 verzija 1709 ili novija verzija</span><span class="sxs-lookup"><span data-stu-id="d35ca-110">Windows 10 version 1709 or later versions</span></span>

<span data-ttu-id="d35ca-111">**Koraci za dodavanje ruba u Intune**</span><span class="sxs-lookup"><span data-stu-id="d35ca-111">**Steps to add Edge to Intune**</span></span>

1. <span data-ttu-id="d35ca-112">[Konfigurirajte aplikaciju u programu Intune](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span><span class="sxs-lookup"><span data-stu-id="d35ca-112">[Configure the app in Intune](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
2. <span data-ttu-id="d35ca-113">[Konfigurirajte informacije o aplikaciji](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span><span class="sxs-lookup"><span data-stu-id="d35ca-113">[Configure the app information](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
3. <span data-ttu-id="d35ca-114">[Konfigurirajte postavke aplikacije](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span><span class="sxs-lookup"><span data-stu-id="d35ca-114">[Configure the app settings](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
4. <span data-ttu-id="d35ca-115">[Odaberite oznake dosega (neobavezno)](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span><span class="sxs-lookup"><span data-stu-id="d35ca-115">[Select the scope tags (optional)](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
5. <span data-ttu-id="d35ca-116">[Dodajte aplikaciju](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span><span class="sxs-lookup"><span data-stu-id="d35ca-116">[Add the app](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>

<span data-ttu-id="d35ca-117">Dodatnu pomoć potražite u članku [Otklanjanje poteškoća](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span><span class="sxs-lookup"><span data-stu-id="d35ca-117">For more help, see [Troubleshooting](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>




