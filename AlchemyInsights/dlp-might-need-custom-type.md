---
title: DLP možda trebati prilagođenu vrstu
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: ''
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 890bba57bc36c034c507e6124cd6593ef4d92af8
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932650"
---
# <a name="dlp-might-need-a-custom-type"></a><span data-ttu-id="2c1a6-102">DLP možda trebati prilagođenu vrstu</span><span class="sxs-lookup"><span data-stu-id="2c1a6-102">DLP might need a custom type</span></span>

<span data-ttu-id="2c1a6-103">**Važno**: Mnogi korisnici sustava SharePoint Online i OneDrive pokrenuti poslovne kritične aplikacije protiv servisa koji se izvodi u pozadini.</span><span class="sxs-lookup"><span data-stu-id="2c1a6-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="2c1a6-104">To uključuje migraciju sadržaja, sprječavanje gubitka podataka (DLP) i sigurnosna rješenja.</span><span class="sxs-lookup"><span data-stu-id="2c1a6-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="2c1a6-105">Tijekom ovih dosad nezabilježenih vremena poduzimamo korake kako bismo osigurali da usluge sustava SharePoint Online i OneDrive ostanu vrlo dostupne i pouzdane za korisnike koji više nego ikad ovise o usluzi.</span><span class="sxs-lookup"><span data-stu-id="2c1a6-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="2c1a6-106">U prilog tom cilju, implementirali smo stroža ograničenja regulacije pozadinskih aplikacija (migracije, DLP i backup rješenja) tijekom radnih dana.</span><span class="sxs-lookup"><span data-stu-id="2c1a6-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="2c1a6-107">Trebali biste očekivati da ove aplikacije će postići vrlo ograničen propusnost tijekom tih vremena.</span><span class="sxs-lookup"><span data-stu-id="2c1a6-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="2c1a6-108">Međutim, tijekom večernjih i vikend sati za regiju, usluga će biti spremna za obradu znatno veći volumen zahtjeva iz pozadinskih aplikacija.</span><span class="sxs-lookup"><span data-stu-id="2c1a6-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="2c1a6-109">**DLP može zahtijevati prilagođenu vrstu informacija**</span><span class="sxs-lookup"><span data-stu-id="2c1a6-109">**DLP may require a custom information type**</span></span>

<span data-ttu-id="2c1a6-110">Pomoću pravila za sprječavanje gubitka podataka (DLP) možete prepoznati i zaštititi osjetljive podatke u svojoj tvrtki ili ustanovi.</span><span class="sxs-lookup"><span data-stu-id="2c1a6-110">With a data loss prevention (DLP) policy, you can identify and protect sensitive data in your organization.</span></span> <span data-ttu-id="2c1a6-111">U nekim ćete scenarijima možda morati stvoriti vlastitu prilagođenu vrstu **osjetljivih** informacija da biste zaštitili podatke svoje tvrtke ili ustanove.</span><span class="sxs-lookup"><span data-stu-id="2c1a6-111">In some scenarios, you might need to create your own **custom** sensitive information type to protect your organization's data.</span></span>

<span data-ttu-id="2c1a6-112">Na primjer, vaša će tvrtka ili ustanova možda morati identificirati i zaštititi ID-ove zaposlenika ili druge podatke u nekom obliku specifičnom za vašu tvrtku ili ustanovu. Ako je tako, dodatne informacije potražite u sljedećim člancima.</span><span class="sxs-lookup"><span data-stu-id="2c1a6-112">For example, your organization might need to identify and protect employee IDs or other data in some format specific to your org. If so, see the following articles for more information.</span></span>
  
 <span data-ttu-id="2c1a6-113">**Prilagodba ugrađene osjetljive vrste informacija**</span><span class="sxs-lookup"><span data-stu-id="2c1a6-113">**Customize a built-in sensitive information type**</span></span>
  
<span data-ttu-id="2c1a6-114">Ako bi ugrađena osjetljiva vrsta informacija zadovoljila vaše potrebe uz samo nekoliko ugađanja, možete [prilagoditi ugrađenu vrstu osjetljivih informacija](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="2c1a6-114">If a built-in sensitive information type would meet your needs with just a few tweaks, you can [customize a built-in sensitive information type](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span></span> <span data-ttu-id="2c1a6-115">Na primjer, možete dodati ili ukloniti ključne riječi ili dodati ili ukloniti popratne dokaze kao što su datum ili adresa.</span><span class="sxs-lookup"><span data-stu-id="2c1a6-115">For example, you can add or remove keywords, or add or remove supporting evidence such as a date or address.</span></span>
  
 <span data-ttu-id="2c1a6-116">**Stvaranje prilagođene vrste osjetljivih informacija**</span><span class="sxs-lookup"><span data-stu-id="2c1a6-116">**Create a custom sensitive information type**</span></span>
  
<span data-ttu-id="2c1a6-117">No ako trebate potpuno prepoznati i zaštititi drugu vrstu osjetljivih podataka, možete [stvoriti prilagođenu vrstu osjetljivih informacija](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) u ubedi centra za & sigurnost.</span><span class="sxs-lookup"><span data-stu-id="2c1a6-117">But if you need to identify and protect a different type of sensitive information altogether, you can [create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) in the UI of the Security & Compliance Center.</span></span>
  
<span data-ttu-id="2c1a6-118">**Stvaranje prilagođene vrste osjetljivih informacija u centru za sigurnost & PowerShell centra za &**</span><span class="sxs-lookup"><span data-stu-id="2c1a6-118">**Create a custom sensitive information type in Security & Compliance Center PowerShell**</span></span>

<span data-ttu-id="2c1a6-119">Konačno, ako utis ne pruža sve potrebne mogućnosti, možete [stvoriti prilagođenu vrstu osjetljivih informacija u sigurnosnoj & Centru za usklađenost PowerShell](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="2c1a6-119">Finally, if the UI doesn't provide all the options you need, you can [create a custom sensitive information type in Security & Compliance Center PowerShell](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span></span> <span data-ttu-id="2c1a6-120">Počevši od XML datoteke, možete koristiti svaku dostupnu mogućnost.</span><span class="sxs-lookup"><span data-stu-id="2c1a6-120">By starting with an XML file, you can use every option available.</span></span>
