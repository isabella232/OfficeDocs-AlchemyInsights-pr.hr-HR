---
title: Rješavanje običnih problema s oblikovanjem zapisa DKIM
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/23/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: 0a59ca1c93121cb4681c0d44b85a9b756c07895b
ms.sourcegitcommit: 78fe9f33438cb0c19f0dab31253b5853b73f4f47
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50523401"
---
# <a name="fix-common-problems-with-dkim-record-formatting"></a><span data-ttu-id="74085-102">Rješavanje običnih problema s oblikovanjem zapisa DKIM</span><span class="sxs-lookup"><span data-stu-id="74085-102">Fix common problems with DKIM record formatting</span></span>

<span data-ttu-id="74085-103">Većina problema s postavkom d-a odnosi se na pogrešne DNS zapise.</span><span class="sxs-lookup"><span data-stu-id="74085-103">Most DKIM set-up issues are related to incorrect DNS records.</span></span>

<span data-ttu-id="74085-104">Da biste riješili probleme s postavkom za d-up, provjerite je li u zapisu programa d (**ne** TXT zapis) pravilno oblikovan.</span><span class="sxs-lookup"><span data-stu-id="74085-104">To fix the DKIM set-up issues, verify that the DKIM CNAME record (**not** a TXT record) is formatted correctly.</span></span> <span data-ttu-id="74085-105">Dodatne informacije potražite u članku [što je potrebno učiniti da biste ručno postavili dukič u sustavu Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email).</span><span class="sxs-lookup"><span data-stu-id="74085-105">For more information, see [What you need to do to manually set up DKIM in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email).</span></span>

<span data-ttu-id="74085-106">Ako vam je potrebna pomoć za općenito DNS zapise, pročitajte članak [Stvaranje DNS zapisa na bilo kojem davatelju usluga HOSTIRANJA DNS-a za Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).</span><span class="sxs-lookup"><span data-stu-id="74085-106">If you need help with DNS records in general, see [Create DNS records at any DNS hosting provider for Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).</span></span>

> [!NOTE]
> <span data-ttu-id="74085-107">Kada stvorite ili ažurirate svoj DNS zapise u servisu DNS na web-mjestu hosting za domenu, morat ćete čekati da se DNS zapisi propagiraju.</span><span class="sxs-lookup"><span data-stu-id="74085-107">After you create or update your DKIM DNS records at the DNS hosting service for your domain, you'll need to wait for the DNS records to propagate.</span></span>
