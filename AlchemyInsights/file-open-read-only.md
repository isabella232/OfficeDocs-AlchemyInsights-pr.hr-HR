---
title: Datoteka je otvorena samo za čitanje
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 39748581-d319-403c-8501-9b785e4a0ed8
ms.custom:
- "765"
- "2200014"
ms.openlocfilehash: 2fdb4f048c2bee022a49c2cca2ce9770f42a87a2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47745567"
---
# <a name="file-open-read-only"></a><span data-ttu-id="54fd8-102">Datoteka je otvorena samo za čitanje</span><span class="sxs-lookup"><span data-stu-id="54fd8-102">File open read-only</span></span>

<span data-ttu-id="54fd8-103">Kada otvarate datoteke, možda će se otvoriti kao samo za čitanje.</span><span class="sxs-lookup"><span data-stu-id="54fd8-103">You may find that when you are opening files, they open as read-only.</span></span> <span data-ttu-id="54fd8-104">U nekim slučajevima to je za dodatnu sigurnost, kao što je kada otvarate datoteke s interneta, a drugi puta, to može biti zbog postavke koja se može promijeniti.</span><span class="sxs-lookup"><span data-stu-id="54fd8-104">In some cases, this is for added security, such as when you are opening files from the internet, and other times, it can be due to a setting that can be changed.</span></span> <span data-ttu-id="54fd8-105">Slijede neki scenariji u kojima se datoteka otvara samo za čitanje i neki koraci koje možete poduzeti da biste to promijenili.</span><span class="sxs-lookup"><span data-stu-id="54fd8-105">Here are some scenarios where a file opens read-only and some steps you can take to change that.</span></span>
  
 <span data-ttu-id="54fd8-106">**Protuvirusni program uzrokuje otvaranje samo za čitanje**</span><span class="sxs-lookup"><span data-stu-id="54fd8-106">**My antivirus is causing them to open read-only**</span></span>
  
<span data-ttu-id="54fd8-107">Neki antivirusni programi mogu vas zaštititi od potencijalno nesigurnih datoteka tako da ih otvorite samo za čitanje.</span><span class="sxs-lookup"><span data-stu-id="54fd8-107">Some antivirus programs may protect you from potentially unsafe files by opening them read-only.</span></span> <span data-ttu-id="54fd8-108">Da biste doznali kako prilagoditi te postavke, možda ćete morati provjeriti uz davatelja usluge antivirusnog softvera.</span><span class="sxs-lookup"><span data-stu-id="54fd8-108">You may need to check with your antivirus provider to learn how to adjust these settings.</span></span> <span data-ttu-id="54fd8-109">BitDefender, primjerice, ima sadržaj na dodavanju izuzeća aplikacija ovdje: [Kako dodati isključenja aplikacija i procesa u Control Center BitDefender](https://aka.ms/AA6098i).</span><span class="sxs-lookup"><span data-stu-id="54fd8-109">BitDefender, for example, has content on adding application exclusions here: [How to add application or process exclusions in Bitdefender Control Center](https://aka.ms/AA6098i).</span></span>
  
 <span data-ttu-id="54fd8-110">**Jesu li svojstva datoteke postavljena na samo za čitanje?**</span><span class="sxs-lookup"><span data-stu-id="54fd8-110">**Are the file properties set to read-only?**</span></span>
  
<span data-ttu-id="54fd8-111">Svojstva datoteke možete provjeriti tako da desnom tipkom miša kliknete datoteku i odaberete Svojstva.</span><span class="sxs-lookup"><span data-stu-id="54fd8-111">You can check the file properties by right-clicking on the file and choosing Properties.</span></span> <span data-ttu-id="54fd8-112">Ako je potvrđen atribut samo za čitanje, možete ga poništiti i kliknuti u redu.</span><span class="sxs-lookup"><span data-stu-id="54fd8-112">If the Read-only attribute is checked, you can uncheck it and click OK.</span></span>
  
 <span data-ttu-id="54fd8-113">**Sadržaj je u zaštićenom prikazu**</span><span class="sxs-lookup"><span data-stu-id="54fd8-113">**The content is in protected view**</span></span>
  
<span data-ttu-id="54fd8-114">Datoteke s interneta i na drugim potencijalno nesigurnim mjestima mogu sadržavati viruse, crve ili druge vrste zlonamjernog softvera koje mogu naštetiti računalu.</span><span class="sxs-lookup"><span data-stu-id="54fd8-114">Files from the Internet and from other potentially unsafe locations can contain viruses, worms, or other kinds of malware that can harm your computer.</span></span> <span data-ttu-id="54fd8-115">To je najčešće i slučaj s privicima e-pošte ili preuzetim datotekama.</span><span class="sxs-lookup"><span data-stu-id="54fd8-115">This is also commonly the case with email attachments or files you've downloaded.</span></span> <span data-ttu-id="54fd8-116">Da bi zaštitili računalo, datoteke s tih potencijalno nesigurnih mjesta otvaraju se u zaštićenom prikazu.</span><span class="sxs-lookup"><span data-stu-id="54fd8-116">To help protect your computer, files from these potentially unsafe locations are opened in Protected View.</span></span> <span data-ttu-id="54fd8-117">Pomoću zaštićenog prikaza možete pročitati datoteku i vidjeti njezin sadržaj pri smanjenju rizika.</span><span class="sxs-lookup"><span data-stu-id="54fd8-117">By using Protected View, you can read a file and see its contents while reducing the risks.</span></span> <span data-ttu-id="54fd8-118">Dodatne informacije o zaštićenom prikazu i načinu promjene postavki potražite u ovom članku: [što je zaštićeni prikaz?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span><span class="sxs-lookup"><span data-stu-id="54fd8-118">For more information on Protected view and how to change settings, see this article: [What is Protected View?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span></span>
  
 <span data-ttu-id="54fd8-119">**Je li OneDrive pun?**</span><span class="sxs-lookup"><span data-stu-id="54fd8-119">**Is OneDrive full?**</span></span>
  
<span data-ttu-id="54fd8-120">Ako je datoteka pohranjena na servisu OneDrive, a prostor za pohranu na servisu OneDrive pun, nećete moći spremiti dokument dok se ne pronađete u zadanom prostoru.</span><span class="sxs-lookup"><span data-stu-id="54fd8-120">If the file is stored on OneDrive and your OneDrive storage space is full, you will be unable to save the document until you are under your allotted space.</span></span> <span data-ttu-id="54fd8-121">Besplatni prostor na servisu OneDrive možete provjeriti tako da kliknete ikonu servisa OneDrive u centru za obavijesti i odaberete Upravljanje spremištem ili možete otići na [https://onedrive.live.com](https://onedrive.live.com) , prijaviti se i primijetiti iznos korištenog razmaka u donjem lijevoj strani zaslona.</span><span class="sxs-lookup"><span data-stu-id="54fd8-121">You can check your free space on OneDrive by clicking the OneDrive icon in the notification center and choosing Manage storage, or you can go to [https://onedrive.live.com](https://onedrive.live.com), sign in, and note the amount of used space in the lower left of the screen.</span></span>
  
 <span data-ttu-id="54fd8-122">**Je li Office aktiviran?**</span><span class="sxs-lookup"><span data-stu-id="54fd8-122">**Is Office activated?**</span></span>
  
<span data-ttu-id="54fd8-123">Ako Office nije aktiviran ili ako vam je pretplata istekla, možete biti u načinu rada za smanjene funkcionalnosti samo za čitanje.</span><span class="sxs-lookup"><span data-stu-id="54fd8-123">If Office is not activated, or if your subscription has expired, you could be in read-only Reduced Functionality Mode.</span></span> <span data-ttu-id="54fd8-124">Informacije o tome kako aktivirati Office potražite [u članku nelicencirani proizvodi i pogreške pri aktivaciji u sustavu Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span><span class="sxs-lookup"><span data-stu-id="54fd8-124">For information on how to Activate Office, see: [Unlicensed Product and activation errors in Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>
  
 <span data-ttu-id="54fd8-125">**Ako sve drugo ne uspije...**</span><span class="sxs-lookup"><span data-stu-id="54fd8-125">**If all else fails...**</span></span>
  
- <span data-ttu-id="54fd8-126">Pokušajte ponovno pokrenuti računalo</span><span class="sxs-lookup"><span data-stu-id="54fd8-126">Try restarting the computer</span></span>
    
- <span data-ttu-id="54fd8-127">Instalacija ažuriranja sustava Office</span><span class="sxs-lookup"><span data-stu-id="54fd8-127">Install Office updates</span></span>
    
- <span data-ttu-id="54fd8-128">Izvođenje internetskog popravka sustava Office</span><span class="sxs-lookup"><span data-stu-id="54fd8-128">Perform an Online repair of Office</span></span>
    

