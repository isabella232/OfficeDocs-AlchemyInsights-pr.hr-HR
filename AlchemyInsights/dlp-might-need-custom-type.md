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
ms.openlocfilehash: 87fcb5c3cc9ccd525265097b66d9d9b3a85c5feb
ms.sourcegitcommit: d108a2da2f5dab05246e30b5108cca5173e09051
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/26/2020
ms.locfileid: "42977262"
---
# <a name="dlp-might-need-a-custom-type"></a><span data-ttu-id="4b8f2-102">DLP možda trebati prilagođenu vrstu</span><span class="sxs-lookup"><span data-stu-id="4b8f2-102">DLP might need a custom type</span></span>

<span data-ttu-id="4b8f2-103">**Važno**: Tijekom ovih dosad nezabilježenih vremena poduzimamo korake kako bismo osigurali da usluge sustava SharePoint Online i onedrive ostanu vrlo dostupne – dodatne informacije [potražite u članku Prilagodbe privremenih značajki sustava SharePoint Online.](https://aka.ms/ODSPAdjustments)</span><span class="sxs-lookup"><span data-stu-id="4b8f2-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="4b8f2-104">**DLP može zahtijevati prilagođenu vrstu informacija**</span><span class="sxs-lookup"><span data-stu-id="4b8f2-104">**DLP may require a custom information type**</span></span>

<span data-ttu-id="4b8f2-105">Pomoću pravila za sprječavanje gubitka podataka (DLP) možete prepoznati i zaštititi osjetljive podatke u svojoj tvrtki ili ustanovi.</span><span class="sxs-lookup"><span data-stu-id="4b8f2-105">With a data loss prevention (DLP) policy, you can identify and protect sensitive data in your organization.</span></span> <span data-ttu-id="4b8f2-106">U nekim ćete scenarijima možda morati stvoriti vlastitu prilagođenu vrstu **osjetljivih** informacija da biste zaštitili podatke svoje tvrtke ili ustanove.</span><span class="sxs-lookup"><span data-stu-id="4b8f2-106">In some scenarios, you might need to create your own **custom** sensitive information type to protect your organization's data.</span></span>

<span data-ttu-id="4b8f2-107">Na primjer, vaša će tvrtka ili ustanova možda morati identificirati i zaštititi ID-ove zaposlenika ili druge podatke u nekom obliku specifičnom za vašu tvrtku ili ustanovu. Ako je tako, dodatne informacije potražite u sljedećim člancima.</span><span class="sxs-lookup"><span data-stu-id="4b8f2-107">For example, your organization might need to identify and protect employee IDs or other data in some format specific to your org. If so, see the following articles for more information.</span></span>
  
 <span data-ttu-id="4b8f2-108">**Prilagodba ugrađene osjetljive vrste informacija**</span><span class="sxs-lookup"><span data-stu-id="4b8f2-108">**Customize a built-in sensitive information type**</span></span>
  
<span data-ttu-id="4b8f2-109">Ako bi ugrađena osjetljiva vrsta informacija zadovoljila vaše potrebe uz samo nekoliko ugađanja, možete [prilagoditi ugrađenu vrstu osjetljivih informacija](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="4b8f2-109">If a built-in sensitive information type would meet your needs with just a few tweaks, you can [customize a built-in sensitive information type](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span></span> <span data-ttu-id="4b8f2-110">Na primjer, možete dodati ili ukloniti ključne riječi ili dodati ili ukloniti popratne dokaze kao što su datum ili adresa.</span><span class="sxs-lookup"><span data-stu-id="4b8f2-110">For example, you can add or remove keywords, or add or remove supporting evidence such as a date or address.</span></span>
  
 <span data-ttu-id="4b8f2-111">**Stvaranje prilagođene vrste osjetljivih informacija**</span><span class="sxs-lookup"><span data-stu-id="4b8f2-111">**Create a custom sensitive information type**</span></span>
  
<span data-ttu-id="4b8f2-112">No ako trebate potpuno prepoznati i zaštititi drugu vrstu osjetljivih podataka, možete [stvoriti prilagođenu vrstu osjetljivih informacija](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) u ubedi centra za & sigurnost.</span><span class="sxs-lookup"><span data-stu-id="4b8f2-112">But if you need to identify and protect a different type of sensitive information altogether, you can [create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) in the UI of the Security & Compliance Center.</span></span>
  
<span data-ttu-id="4b8f2-113">**Stvaranje prilagođene vrste osjetljivih informacija u centru za sigurnost & PowerShell centra za &**</span><span class="sxs-lookup"><span data-stu-id="4b8f2-113">**Create a custom sensitive information type in Security & Compliance Center PowerShell**</span></span>

<span data-ttu-id="4b8f2-114">Konačno, ako utis ne pruža sve potrebne mogućnosti, možete [stvoriti prilagođenu vrstu osjetljivih informacija u sigurnosnoj & Centru za usklađenost PowerShell](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="4b8f2-114">Finally, if the UI doesn't provide all the options you need, you can [create a custom sensitive information type in Security & Compliance Center PowerShell](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span></span> <span data-ttu-id="4b8f2-115">Počevši od XML datoteke, možete koristiti svaku dostupnu mogućnost.</span><span class="sxs-lookup"><span data-stu-id="4b8f2-115">By starting with an XML file, you can use every option available.</span></span>
