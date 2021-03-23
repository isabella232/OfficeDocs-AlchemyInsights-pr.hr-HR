---
title: Uvoz i izvoz iz servisa Yammer
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9735"
- "9003224"
ms.openlocfilehash: dcdf569f96e51a62899761589ef6f9f317517c3a
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035092"
---
# <a name="import-and-export-from-yammer"></a><span data-ttu-id="1fea2-102">Uvoz i izvoz iz servisa Yammer</span><span class="sxs-lookup"><span data-stu-id="1fea2-102">Import and export from Yammer</span></span>

<span data-ttu-id="1fea2-103">**Uvoz**</span><span class="sxs-lookup"><span data-stu-id="1fea2-103">**Import**</span></span>

<span data-ttu-id="1fea2-104">Mogućnosti uvoza korisnika razlikuju se ovisno o tome je li mreža servisa Yammer u [izvornom načinu rada za Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/overview-native-mode)ili ne.</span><span class="sxs-lookup"><span data-stu-id="1fea2-104">User-import options vary depending on whether your Yammer network is in [Native Mode for Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/overview-native-mode), or not.</span></span>

- <span data-ttu-id="1fea2-105">**Način koji nije urođenik**: korisnici se mogu uvesti u grupe pomoću značajke [Dodaj iz adresara](https://support.microsoft.com/office/manage-yammer-community-members-75253554-d0f3-4148-b835-e6a9a8a0c294) (ograničenje na 100 korisnika) unutar postavki grupe ili na mrežu pomoću [skupnog ažuriranja](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users) unutar administratora mreže.</span><span class="sxs-lookup"><span data-stu-id="1fea2-105">**Non-Native Mode**: Users can be imported to groups using [Add from Address Book](https://support.microsoft.com/office/manage-yammer-community-members-75253554-d0f3-4148-b835-e6a9a8a0c294) (limit to 100 users) within group settings, or to the network using [Bulk Update](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users) within Network Admin.</span></span>
- <span data-ttu-id="1fea2-106">**Izvorni način rada**: članstvo u grupama i mreža za članstvo moraju se izvoditi na servisu [Microsoft 365 admin portal](https://docs.microsoft.com/microsoft-365/admin/add-users), [Azure ad portal](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)ili pomoću druge mogućnosti Azure AD.</span><span class="sxs-lookup"><span data-stu-id="1fea2-106">**Native Mode**: Group membership and network membership operations should be performed from the [Microsoft 365 admin portal](https://docs.microsoft.com/microsoft-365/admin/add-users), [Azure AD portal](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory), or using another Azure AD option.</span></span> <span data-ttu-id="1fea2-107">Mreže u izvornom načinu više ne sadrže pristup masovnim ažuriranjem i drugim naslijeđenim značajkama.</span><span class="sxs-lookup"><span data-stu-id="1fea2-107">Networks in Native Mode no longer have access to Bulk Update and other legacy features.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="1fea2-108">Yammer nikada nije podržao Uvoz sadržaja iz mrežnog administratora čak ni kada je značajka izvoza podataka korištena u drugoj mreži.</span><span class="sxs-lookup"><span data-stu-id="1fea2-108">Yammer never supported importing content from within Network Admin even when the Data Export feature was used in another network.</span></span> <span data-ttu-id="1fea2-109">Sadržaj se može ponovno knjižiti putem partnerskih rješenja ili API-ja za odmor u servisu Yammer.</span><span class="sxs-lookup"><span data-stu-id="1fea2-109">Content can be re-posted by partner solutions or the Yammer REST APIs.</span></span>

<span data-ttu-id="1fea2-110">**Izvoz**</span><span class="sxs-lookup"><span data-stu-id="1fea2-110">**Export**</span></span>

<span data-ttu-id="1fea2-111">[Izvoz mrežnih podataka unutar mrežnog administratora](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data) dopušta izvoz sadržaja iz mreža servisa Yammer, uključujući poruke i datoteke.</span><span class="sxs-lookup"><span data-stu-id="1fea2-111">[Export Network Data within Network Admin](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data) permits the export of content from Yammer networks, including messages and files.</span></span> <span data-ttu-id="1fea2-112">Privici mogu biti izuzetno veliki i prouzroci da će izvoz poduzeti značajno vrijeme za dovršetak.</span><span class="sxs-lookup"><span data-stu-id="1fea2-112">Attachments can be extremely large and will cause exports to take significant time to complete.</span></span> <span data-ttu-id="1fea2-113">Preporučujemo da se aktivne mreže izvoze pomoću API-ja za [Izvoz podataka](https://developer.yammer.com/docs/data-export-api) u komadima za dan ili tjedan.</span><span class="sxs-lookup"><span data-stu-id="1fea2-113">We recommend that active networks are exported using the [Data Export API](https://developer.yammer.com/docs/data-export-api) in chunks by day or week.</span></span> <span data-ttu-id="1fea2-114">Microsoftova podrška ne nudi prilagođene skripte za tu svrhu.</span><span class="sxs-lookup"><span data-stu-id="1fea2-114">Microsoft Support does not provide custom scripts for this purpose.</span></span>

<span data-ttu-id="1fea2-115">Za izvoz sadržaja za pojedinačnog korisnika postoji zasebni [Izvoz u Gdpr](https://docs.microsoft.com/yammer/manage-security-and-compliance/gdpr-requests-in-yammer-enterprise) -u.</span><span class="sxs-lookup"><span data-stu-id="1fea2-115">A separate [GDPR export](https://docs.microsoft.com/yammer/manage-security-and-compliance/gdpr-requests-in-yammer-enterprise) exists to export content for an individual user.</span></span>