---
title: Datoteka je otvorena samo za čitanje
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: e478572ea82e5ea11bac9fd7eacafb833253235d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813176"
---
# <a name="file-open-read-only"></a><span data-ttu-id="d8f92-102">Datoteka je otvorena samo za čitanje</span><span class="sxs-lookup"><span data-stu-id="d8f92-102">File open read-only</span></span>

<span data-ttu-id="d8f92-103">Možda ćete otkriti da se prilikom otvaranja datoteka otvaraju samo za čitanje.</span><span class="sxs-lookup"><span data-stu-id="d8f92-103">You may find that when you are opening files, they open as read-only.</span></span> <span data-ttu-id="d8f92-104">U nekim se slučajevima radi o dodanoj sigurnosti, primjerice prilikom otvaranja datoteka s interneta, a ponekad i zbog postavke koju je moguće promijeniti.</span><span class="sxs-lookup"><span data-stu-id="d8f92-104">In some cases, this is for added security, such as when you are opening files from the internet, and other times, it can be due to a setting that can be changed.</span></span> <span data-ttu-id="d8f92-105">Evo nekih scenarija u kojima se datoteka otvara samo za čitanje i neke korake koje možete poduzeti da biste to promijenili.</span><span class="sxs-lookup"><span data-stu-id="d8f92-105">Here are some scenarios where a file opens read-only and some steps you can take to change that.</span></span>
  
 <span data-ttu-id="d8f92-106">**Antivirusni program uzrokuje otvaranje samo za čitanje**</span><span class="sxs-lookup"><span data-stu-id="d8f92-106">**My antivirus is causing them to open read-only**</span></span>
  
<span data-ttu-id="d8f92-107">Neki antivirusni programi mogu vas zaštititi od potencijalno nesigurnih datoteka tako da ih otvore samo za čitanje.</span><span class="sxs-lookup"><span data-stu-id="d8f92-107">Some antivirus programs may protect you from potentially unsafe files by opening them read-only.</span></span> <span data-ttu-id="d8f92-108">Možda ćete morati kod davatelja antivirusnog programa provjeriti kako prilagoditi te postavke.</span><span class="sxs-lookup"><span data-stu-id="d8f92-108">You may need to check with your antivirus provider to learn how to adjust these settings.</span></span> <span data-ttu-id="d8f92-109">BitDefender, primjerice, sadrži sadržaj o dodavanju izuzimanja aplikacija ovdje: Dodavanje izuzimanja aplikacija ili procesa [u kontrolnom centru za Bitdefender](https://aka.ms/AA6098i).</span><span class="sxs-lookup"><span data-stu-id="d8f92-109">BitDefender, for example, has content on adding application exclusions here: [How to add application or process exclusions in Bitdefender Control Center](https://aka.ms/AA6098i).</span></span>
  
 <span data-ttu-id="d8f92-110">**Jesu li svojstva datoteke postavljena na samo za čitanje?**</span><span class="sxs-lookup"><span data-stu-id="d8f92-110">**Are the file properties set to read-only?**</span></span>
  
<span data-ttu-id="d8f92-111">Svojstva datoteke možete provjeriti tako da desnom tipkom miša kliknete datoteku, a zatim odaberete Svojstva.</span><span class="sxs-lookup"><span data-stu-id="d8f92-111">You can check the file properties by right-clicking on the file and choosing Properties.</span></span> <span data-ttu-id="d8f92-112">Ako je potvrđen atribut Samo za čitanje, poništite ga i kliknite U redu.</span><span class="sxs-lookup"><span data-stu-id="d8f92-112">If the Read-only attribute is checked, you can uncheck it and click OK.</span></span>
  
 <span data-ttu-id="d8f92-113">**Sadržaj je u zaštićenom prikazu**</span><span class="sxs-lookup"><span data-stu-id="d8f92-113">**The content is in protected view**</span></span>
  
<span data-ttu-id="d8f92-114">Datoteke s interneta i s drugih potencijalno nesigurnih mjesta mogu sadržavati viruse, crve ili druge vrste zlonamjernog softvera koje mogu oštetiti računalo.</span><span class="sxs-lookup"><span data-stu-id="d8f92-114">Files from the Internet and from other potentially unsafe locations can contain viruses, worms, or other kinds of malware that can harm your computer.</span></span> <span data-ttu-id="d8f92-115">To je obično slučaj i s privicima e-pošte ili datotekama koje ste preuzeli.</span><span class="sxs-lookup"><span data-stu-id="d8f92-115">This is also commonly the case with email attachments or files you've downloaded.</span></span> <span data-ttu-id="d8f92-116">Da biste zaštitili računalo, datoteke s tih potencijalno nesigurnih mjesta otvaraju se u zaštićenom prikazu.</span><span class="sxs-lookup"><span data-stu-id="d8f92-116">To help protect your computer, files from these potentially unsafe locations are opened in Protected View.</span></span> <span data-ttu-id="d8f92-117">Pomoću zaštićenog prikaza možete pročitati datoteku i vidjeti njezin sadržaj uz smanjenje rizika.</span><span class="sxs-lookup"><span data-stu-id="d8f92-117">By using Protected View, you can read a file and see its contents while reducing the risks.</span></span> <span data-ttu-id="d8f92-118">Dodatne informacije o zaštićenom prikazu i promjenama postavki potražite u ovom članku: [Što je zaštićeni prikaz?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span><span class="sxs-lookup"><span data-stu-id="d8f92-118">For more information on Protected view and how to change settings, see this article: [What is Protected View?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span></span>
  
 <span data-ttu-id="d8f92-119">**Je li OneDrive pun?**</span><span class="sxs-lookup"><span data-stu-id="d8f92-119">**Is OneDrive full?**</span></span>
  
<span data-ttu-id="d8f92-120">Ako je datoteka pohranjena na servisu OneDrive i prostor za pohranu na servisu OneDrive je pun, nećete moći spremiti dokument dok se ne nalazite ispod dodijeljenog prostora.</span><span class="sxs-lookup"><span data-stu-id="d8f92-120">If the file is stored on OneDrive and your OneDrive storage space is full, you will be unable to save the document until you are under your allotted space.</span></span> <span data-ttu-id="d8f92-121">Slobodni prostor na servisu OneDrive možete provjeriti klikom na ikonu servisa OneDrive u centru za obavijesti i odabirom mogućnosti Upravljanje prostorom za pohranu ili se možete prijaviti, a zatim zabilježiti količinu iskorištenog prostora u donjem [https://onedrive.live.com](https://onedrive.live.com) lijevom kutu zaslona.</span><span class="sxs-lookup"><span data-stu-id="d8f92-121">You can check your free space on OneDrive by clicking the OneDrive icon in the notification center and choosing Manage storage, or you can go to [https://onedrive.live.com](https://onedrive.live.com), sign in, and note the amount of used space in the lower left of the screen.</span></span>
  
 <span data-ttu-id="d8f92-122">**Je li Office aktiviran?**</span><span class="sxs-lookup"><span data-stu-id="d8f92-122">**Is Office activated?**</span></span>
  
<span data-ttu-id="d8f92-123">Ako Office nije aktiviran ili je pretplata istekla, možda ste u načinu rada smanjene funkcionalnosti samo za čitanje.</span><span class="sxs-lookup"><span data-stu-id="d8f92-123">If Office is not activated, or if your subscription has expired, you could be in read-only Reduced Functionality Mode.</span></span> <span data-ttu-id="d8f92-124">Informacije o aktivaciji sustava Office potražite u članku: [Nelicencirani proizvod i pogreške prilikom aktivacije u sustavu Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span><span class="sxs-lookup"><span data-stu-id="d8f92-124">For information on how to Activate Office, see: [Unlicensed Product and activation errors in Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>
  
 <span data-ttu-id="d8f92-125">**Ako sve ostalo ne uspije...**</span><span class="sxs-lookup"><span data-stu-id="d8f92-125">**If all else fails...**</span></span>
  
- <span data-ttu-id="d8f92-126">Pokušajte ponovno pokrenuti računalo</span><span class="sxs-lookup"><span data-stu-id="d8f92-126">Try restarting the computer</span></span>
    
- <span data-ttu-id="d8f92-127">Instalacija ažuriranja sustava Office</span><span class="sxs-lookup"><span data-stu-id="d8f92-127">Install Office updates</span></span>
    
- <span data-ttu-id="d8f92-128">Izvođenje mrežnog popravka sustava Office</span><span class="sxs-lookup"><span data-stu-id="d8f92-128">Perform an Online repair of Office</span></span>
    

