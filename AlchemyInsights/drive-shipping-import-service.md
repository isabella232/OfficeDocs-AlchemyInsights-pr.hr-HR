---
title: Drive shipping in the Microsoft 365 Import Service
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11514"
- "9003046"
ms.openlocfilehash: 85d6e723e56b01fd9914165d8c9740f3b055947d
ms.sourcegitcommit: 1226e9a9601dc8fc8ec427235f3c2dd88ff84ced
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/02/2021
ms.locfileid: "52731336"
---
# <a name="drive-shipping-in-the-microsoft-365-import-service"></a><span data-ttu-id="ee767-102">Drive shipping in the Microsoft 365 Import Service</span><span class="sxs-lookup"><span data-stu-id="ee767-102">Drive shipping in the Microsoft 365 Import Service</span></span>

<span data-ttu-id="ee767-103">Koristite dostavu pogona kopiranjem PST-ova na tvrdi disk, a zatim slanjem tvrdog diska Microsoftu.</span><span class="sxs-lookup"><span data-stu-id="ee767-103">Use Drive shipping by copying PSTs to a hard drive and then shipping the hard drive to Microsoft.</span></span>

<span data-ttu-id="ee767-104">Da biste započeli posao:</span><span class="sxs-lookup"><span data-stu-id="ee767-104">To start the job:</span></span>

1. <span data-ttu-id="ee767-105">U centru za Microsoft 365 usklađenosti u odjeljku **Upravljanje informacijama** odaberite **Uvoz**.</span><span class="sxs-lookup"><span data-stu-id="ee767-105">In the Microsoft 365 Compliance Center under **Information Governance**, select **Import**.</span></span>

1. <span data-ttu-id="ee767-106">Odaberite **Odabir vrste posla uvoza**, a zatim **Dalje**.</span><span class="sxs-lookup"><span data-stu-id="ee767-106">Select **Choose import job type**, and then select **Next**.</span></span>

1. <span data-ttu-id="ee767-107">Da biste vidjeli korake za tu mogućnost uvoza, **odaberite Otpremi tvrde diskove na jednu od naših fizičkih mjesta**.</span><span class="sxs-lookup"><span data-stu-id="ee767-107">To see the steps for this import option, select **Ship hard drives to one of our physical locations**.</span></span>

<span data-ttu-id="ee767-108">Evo nekoliko stvari koje treba zapamtiti:</span><span class="sxs-lookup"><span data-stu-id="ee767-108">Here are some things to remember:</span></span>

- <span data-ttu-id="ee767-109">Da biste uvezli PST datoteke u poštanske sandučiće, morate Exchange Online ulogu uvoza uvoza poštanskih sandučića u Microsoft 365 poštanske sandučiće.</span><span class="sxs-lookup"><span data-stu-id="ee767-109">You must be assigned the Mailbox Import Export role in Exchange Online to import PST files to Microsoft 365 mailboxes.</span></span>
<span data-ttu-id="ee767-110">Na performanse je moguće utjecati za PST-ove veće od 20 GB.</span><span class="sxs-lookup"><span data-stu-id="ee767-110">Performance might be impacted for PSTs larger than 20GB.</span></span>

- <span data-ttu-id="ee767-111">Podržani su samo 2,5-inčni solid-state pogoni (SSD-ovi) ili 2,5-inčni ili 3,5-inčni SATA II/III interni tvrdi diskovi.</span><span class="sxs-lookup"><span data-stu-id="ee767-111">Only 2.5-inch solid-state drives (SSDs) or 2.5-inch or 3.5-inch SATA II/III internal hard drives are supported.</span></span>
<span data-ttu-id="ee767-112">Tvrdi disk koji sadrži PST datoteke mora biti šifriran pomoću BitLocker.</span><span class="sxs-lookup"><span data-stu-id="ee767-112">Hard drive containing PST files must be encrypted with BitLocker.</span></span>

- <span data-ttu-id="ee767-113">Trošak uvoza PST datoteka u poštanske Microsoft 365 poštanskim sandučićima koji koriste dostavu pogona iznosi 2 USD po GB podataka.</span><span class="sxs-lookup"><span data-stu-id="ee767-113">The cost to import PST files to Microsoft 365 mailboxes using drive shipping is $2 USD per GB of data.</span></span>

<span data-ttu-id="ee767-114">Dodatne informacije o korištenju načina dostave pogona za uvoz PST-ova potražite u članku Korištenje isporuke pogona [za uvoz PST datoteka tvrtke ili ustanove.](/microsoft-365/compliance/use-drive-shipping-to-import-pst-files-to-office-365)</span><span class="sxs-lookup"><span data-stu-id="ee767-114">For additional information on using the Drive shipping method for importing PSTs, see [Use drive shipping to import your organization's PST files](/microsoft-365/compliance/use-drive-shipping-to-import-pst-files-to-office-365).</span></span>