---
title: Problemi s SharePoint na Windows 7 računala
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9006484"
- "11070"
ms.openlocfilehash: 787f0e713cc95b590bc494868d5098a25131ac56
ms.sourcegitcommit: d33ab8c73d8af51da782094fb8f8abf7626f4df3
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/28/2021
ms.locfileid: "52124814"
---
# <a name="issues-with-sharepoint-on-windows-7-machines"></a><span data-ttu-id="e8370-102">Problemi s SharePoint na Windows 7 računala</span><span class="sxs-lookup"><span data-stu-id="e8370-102">Issues with SharePoint on Windows 7 machines</span></span>

<span data-ttu-id="e8370-103">Ako se prilikom rada na SharePoint ili OneDrive pojavljuje pogreška na Windows 7 računala, možda su povezane s ukidanjom TLS 1.0/1.1.</span><span class="sxs-lookup"><span data-stu-id="e8370-103">If you receive errors on Windows 7 machines while working on SharePoint or OneDrive, they might be related to the deprecation of TLS 1.0/1.1.</span></span> <span data-ttu-id="e8370-104">Dodatne informacije potražite u sljedećim člancima:</span><span class="sxs-lookup"><span data-stu-id="e8370-104">For more information, see:</span></span>

- [<span data-ttu-id="e8370-105">Priprema za TLS 1.2 u Office 365 i Office 365 GCC</span><span class="sxs-lookup"><span data-stu-id="e8370-105">Preparing for TLS 1.2 in Office 365 and Office 365 GCC</span></span>](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- <span data-ttu-id="e8370-106">Windows 7 SP1/Windows 8 moraju imati omogućen TLS1.2.</span><span class="sxs-lookup"><span data-stu-id="e8370-106">Windows 7 SP1/Windows 8 clients must have TLS1.2 enabled.</span></span> <span data-ttu-id="e8370-107">Dodatne informacije potražite u članku Pogreške provjere autentičnosti kada klijent nema podršku [za TLS 1.2](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)</span><span class="sxs-lookup"><span data-stu-id="e8370-107">For more information, see [Authentication errors occur when client doesn't have TLS 1.2 support](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)</span></span>

- <span data-ttu-id="e8370-108">Instalirajte KB3140245 i stvorite vrijednost registra.</span><span class="sxs-lookup"><span data-stu-id="e8370-108">Install KB3140245 and create the registry value.</span></span> <span data-ttu-id="e8370-109">Dodatne informacije potražite u članku Ažuriranje radi omogućivanja [TLS 1.1 i TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392) kao zadanih sigurnih protokola u sustavu WinHTTP u Windows</span><span class="sxs-lookup"><span data-stu-id="e8370-109">For more information, see [Update to enable TLS 1.1 and TLS 1.2 as default secure protocols in WinHTTP in Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)</span></span>

- <span data-ttu-id="e8370-110">Windows 7 SP1/Windows 8 moraju biti instalirani najnoviji TLS paketi za šifru.</span><span class="sxs-lookup"><span data-stu-id="e8370-110">Windows 7 SP1/Windows 8 clients must ensure latest TLS cipher suites are installed.</span></span> <span data-ttu-id="e8370-111">Dodatne informacije potražite u članku [Microsoft Security Advisory 3042058](https://docs.microsoft.com/security-updates/SecurityAdvisories/2015/3042058).</span><span class="sxs-lookup"><span data-stu-id="e8370-111">For more information, see [Microsoft Security Advisory 3042058](https://docs.microsoft.com/security-updates/SecurityAdvisories/2015/3042058).</span></span> 


