---
title: Rješavanje 0x8004de40 pogreške na servisu OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 0edb3e19b5dea240c9f2846dc503e65d92113cb7
ms.sourcegitcommit: 477cce131dc4a3c212ab18a8763a50b2f3bb20b1
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/09/2021
ms.locfileid: "51649740"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="b0e9e-102">Rješavanje 0x8004de40 pogreške na servisu OneDrive</span><span class="sxs-lookup"><span data-stu-id="b0e9e-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="b0e9e-103">Ako koristite Windows 7 i primite tu pogrešku, ažuriranje da biste [omogućili TLS 1.1 i TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)kao zadane sigurne protokole u sustavu WinHTTP u sustavu Windows .</span><span class="sxs-lookup"><span data-stu-id="b0e9e-103">If you're running Windows 7 and receive this error, [Update to enable TLS 1.1 and TLS 1.2 as default secure protocols in WinHTTP in Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392).</span></span>

<span data-ttu-id="b0e9e-104">Ako koristite Windows 10 i prikazuje vam se pogreška 0x8004de40 onedrive:</span><span class="sxs-lookup"><span data-stu-id="b0e9e-104">If you're running Windows 10, and you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="b0e9e-105">Ponovno pokrenite zahvaćeno računalo dok ste povezani s domenom Acitve Directory.</span><span class="sxs-lookup"><span data-stu-id="b0e9e-105">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="b0e9e-106">Ako se problem ne riješi ponovnim pokretanjem, ponovno se pridružite uređaju pomoću servisa Azure AD.</span><span class="sxs-lookup"><span data-stu-id="b0e9e-106">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="b0e9e-107">**Napomena:** tijekom izvođenja ovih koraka trebali biste biti na mreži tvrtke.</span><span class="sxs-lookup"><span data-stu-id="b0e9e-107">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="b0e9e-108">Nemojte izvoditi ove korake kada niste povezani s korporativnom infrastrukturom (primjerice, tijekom putovanja).</span><span class="sxs-lookup"><span data-stu-id="b0e9e-108">Don't perform these steps when you aren't connected to your corporate infrastructure (for example, while traveling).</span></span> 

1. <span data-ttu-id="b0e9e-109">Otvorite povišen naredbeni redak tako da odaberete **Start**, desnom tipkom miša kliknite **Naredbeni redak**, a zatim **odaberite Pokreni kao administrator**.</span><span class="sxs-lookup"><span data-stu-id="b0e9e-109">Open an elevated command prompt by selecting **Start**, right-click **Command Prompt**, and then select **Run as administrator**.</span></span>

1. <span data-ttu-id="b0e9e-110">Upišite *dsregcmd /leave pa* pritisnite **Enter**.</span><span class="sxs-lookup"><span data-stu-id="b0e9e-110">Type *dsregcmd /leave* and press **Enter**.</span></span>

1. <span data-ttu-id="b0e9e-111">Kada završite, upišite *dsregcmd /join i* pritisnite **Enter**.</span><span class="sxs-lookup"><span data-stu-id="b0e9e-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>

1. <span data-ttu-id="b0e9e-112">Kada završite, zatvorite naredbeni redak.</span><span class="sxs-lookup"><span data-stu-id="b0e9e-112">When complete, close the command prompt.</span></span>

1. <span data-ttu-id="b0e9e-113">Ponovno pokrenite računalo i prijavite se na OneDrive.</span><span class="sxs-lookup"><span data-stu-id="b0e9e-113">Reboot the computer, and log into OneDrive.</span></span>