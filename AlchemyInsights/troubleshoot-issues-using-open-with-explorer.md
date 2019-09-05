---
title: Rješavanje problema Otvori pomoću programa Explorer
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 12/10/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: a9ab7dd27e4dc1bd76c93cc81260616063e638ed
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36742725"
---
# <a name="fix-problems-with-open-with-explorer"></a><span data-ttu-id="f55f3-102">Riješite probleme s Otvori pomoću programa Explorer</span><span class="sxs-lookup"><span data-stu-id="f55f3-102">Fix problems with Open with Explorer</span></span>

<span data-ttu-id="f55f3-103">Riješite uobičajene probleme s otvaranjem biblioteku dokumenata u SharePoint ili OneDrive koristeći naredbu **Otvori pomoću programa Explorer** :</span><span class="sxs-lookup"><span data-stu-id="f55f3-103">Fix common problems with opening a document library in SharePoint or OneDrive using the **Open with Explorer** command:</span></span> 
  
- <span data-ttu-id="f55f3-104">Koristite Internet Explorer 10 ili Internet Explorer 11.</span><span class="sxs-lookup"><span data-stu-id="f55f3-104">Use Internet Explorer 10 or Internet Explorer 11.</span></span> <span data-ttu-id="f55f3-105">**Otvori pomoću programa Explorer** nije kompatibilna s Microsoft Edge, vizualnog Google, Firefox i drugima.</span><span class="sxs-lookup"><span data-stu-id="f55f3-105">**Open with Explorer** isn't compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="f55f3-106">**Otvori pomoću programa Explorer** onemogućeno je u svim preglednicima osim preglednika Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="f55f3-106">**Open with Explorer** is disabled in all browsers except Internet Explorer.</span></span> 
    
- <span data-ttu-id="f55f3-107">**Otvori pomoću programa Explorer** nije dostupna u modernom iskustvo za SharePoint biblioteke.</span><span class="sxs-lookup"><span data-stu-id="f55f3-107">**Open with Explorer** is not available in the modern experience for SharePoint libraries.</span></span> <span data-ttu-id="f55f3-108">Umjesto toga koristite **Prikaz Explorer datoteka** .</span><span class="sxs-lookup"><span data-stu-id="f55f3-108">Use **View in File Explorer** instead.</span></span> <span data-ttu-id="f55f3-109">Odaberite **Mogućnosti prikaza** \> **Prikaz Explorer datoteka**.</span><span class="sxs-lookup"><span data-stu-id="f55f3-109">Select **View options** \> **View in File Explorer**.</span></span> <span data-ttu-id="f55f3-110">Prikaz u programu Explorer datoteka nije kompatibilna s Microsoft Edge, vizualnog Google, Firefox i drugima.</span><span class="sxs-lookup"><span data-stu-id="f55f3-110">View in File Explorer is not compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="f55f3-111">**Prikaz u programu Explorer datoteku** u dostupna samo u programu Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="f55f3-111">**View in File Explorer** in available only in Internet Explorer.</span></span> 
    
- <span data-ttu-id="f55f3-112">Provjerite je li pokrenut servis WebClient.</span><span class="sxs-lookup"><span data-stu-id="f55f3-112">Make sure the WebClient service is running.</span></span> <span data-ttu-id="f55f3-113">U okvir za pretraživanje Windows, vrsta pokretanja, odaberite Pokreni radne površine app, upišite services.msc i pritisnite tipku Enter.</span><span class="sxs-lookup"><span data-stu-id="f55f3-113">In the Windows search box, type run, select the Run desktop app, type services.msc, and then press Enter.</span></span> <span data-ttu-id="f55f3-114">Pomaknite WebClient servisa i provjerite je li stupac **Stanje** prikazuje "Pokrenuto".</span><span class="sxs-lookup"><span data-stu-id="f55f3-114">Scroll down to the WebClient service and make sure the **Status** column displays "Running."</span></span> <span data-ttu-id="f55f3-115">Ako ne, dvaput kliknite servis, kliknite **Start**, a zatim kliknite **u redu**.</span><span class="sxs-lookup"><span data-stu-id="f55f3-115">If it doesn't, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="f55f3-116">(Možda ćete morati omogućiti servis odabirom **ručno** ili **Automatsko** u okviru **Vrsta pokretanja** .)</span><span class="sxs-lookup"><span data-stu-id="f55f3-116">(You might need to first enable the service by selecting either **Manual** or **Automatic** in the **Startup type** box.)</span></span> 
    
> [!NOTE]
> <span data-ttu-id="f55f3-117">Otvaranje biblioteke Explorer datoteka je praktičan ako trebate kopirati ili premjestiti više datoteka i mapa jednom, ali ako želite redovito raditi u biblioteci, preporučujemo da ga sinkroniziranje.</span><span class="sxs-lookup"><span data-stu-id="f55f3-117">Opening a library in File Explorer is handy if you need to copy or move multiple files and folders once, but if you want to regularly work in the library, we recommend syncing it.</span></span> <span data-ttu-id="f55f3-118">Za rješavanje problema s otvaranjem datoteka Explorer vidjeti [otvorene u programu Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="f55f3-118">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="f55f3-119">Info o postavljanju sinkronizacije potražite [SharePoint sinkronizaciju datoteke s novom klijentu sinkronizaciju OneDrive](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="f55f3-119">For info about setting up sync, see [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span>
  
<span data-ttu-id="f55f3-120">Pogledajte članak [kako koristiti naredbu "Otvori s Explorer" otklanjanje poteškoća u SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) dodatne informacije.</span><span class="sxs-lookup"><span data-stu-id="f55f3-120">Please see the article [How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) for more information.</span></span> 
  

