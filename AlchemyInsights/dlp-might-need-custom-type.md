---
title: DLP možda će trebati prilagođenu vrstu
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 1ec8959a479f1a8f7bfcffb55f440e8c4ab435fb
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507506"
---
# <a name="dlp-might-need-a-custom-type"></a><span data-ttu-id="a2838-102">DLP možda će trebati prilagođenu vrstu</span><span class="sxs-lookup"><span data-stu-id="a2838-102">DLP might need a custom type</span></span>

<span data-ttu-id="a2838-103">**Važno**: Tijekom ovih neočekivanih vremena poduzimamo korake kako bismo osigurali da servisi SharePoint Online i OneDrive i dalje budu široko raspoloživi – dodatne informacije potražite u [Privremene prilagodbe značajke SharePoint Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="a2838-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="a2838-104">**DLP može zahtijevati prilagođenu vrstu informacija**</span><span class="sxs-lookup"><span data-stu-id="a2838-104">**DLP may require a custom information type**</span></span>

<span data-ttu-id="a2838-105">Pomoću pravila za sprječavanje gubitka podataka (DLP) možete identificirati i zaštititi osjetljive podatke u tvrtki ili ustanovi.</span><span class="sxs-lookup"><span data-stu-id="a2838-105">With a data loss prevention (DLP) policy, you can identify and protect sensitive data in your organization.</span></span> <span data-ttu-id="a2838-106">U nekim ćete scenarijima možda morati stvoriti vlastitu prilagođenu vrstu **osjetljivih** informacija da biste zaštitili podatke tvrtke ili ustanove.</span><span class="sxs-lookup"><span data-stu-id="a2838-106">In some scenarios, you might need to create your own **custom** sensitive information type to protect your organization's data.</span></span>

<span data-ttu-id="a2838-107">Na primjer, vaša tvrtka ili ustanova možda će morati identificirati i zaštititi ID-ove zaposlenika ili druge podatke u nekom obliku određenom za vašu tvrtku ili ustanovu. Ako je tako, dodatne informacije potražite u sljedećim člancima.</span><span class="sxs-lookup"><span data-stu-id="a2838-107">For example, your organization might need to identify and protect employee IDs or other data in some format specific to your org. If so, see the following articles for more information.</span></span>
  
 <span data-ttu-id="a2838-108">**Prilagodba ugrađene vrste osjetljivih informacija**</span><span class="sxs-lookup"><span data-stu-id="a2838-108">**Customize a built-in sensitive information type**</span></span>
  
<span data-ttu-id="a2838-109">Ako bi ugrađena vrsta osjetljivih informacija zadovoljila vaše potrebe sa samo nekoliko ugađanja, možete [prilagoditi ugrađenu vrstu osjetljivih informacija](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="a2838-109">If a built-in sensitive information type would meet your needs with just a few tweaks, you can [customize a built-in sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type).</span></span> <span data-ttu-id="a2838-110">Na primjer, možete dodati ili ukloniti ključne riječi ili dodati ili ukloniti popratne dokaze kao što su datum ili adresa.</span><span class="sxs-lookup"><span data-stu-id="a2838-110">For example, you can add or remove keywords, or add or remove supporting evidence such as a date or address.</span></span>
  
 <span data-ttu-id="a2838-111">**Stvaranje prilagođene vrste osjetljivih informacija**</span><span class="sxs-lookup"><span data-stu-id="a2838-111">**Create a custom sensitive information type**</span></span>
  
<span data-ttu-id="a2838-112">No ako trebate potpuno identificirati i zaštititi drugu vrstu osjetljivih informacija, možete [stvoriti prilagođenu osjetljivu vrstu informacija](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) u korisničkom sučelju centra za usklađenost & sigurnosti.</span><span class="sxs-lookup"><span data-stu-id="a2838-112">But if you need to identify and protect a different type of sensitive information altogether, you can [create a custom sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) in the UI of the Security & Compliance Center.</span></span>
  
<span data-ttu-id="a2838-113">**Stvaranje prilagođene vrste osjetljivih informacija u dodatku PowerShell centar sigurnosti & usklađenosti**</span><span class="sxs-lookup"><span data-stu-id="a2838-113">**Create a custom sensitive information type in Security & Compliance Center PowerShell**</span></span>

<span data-ttu-id="a2838-114">Konačno, ako korisničko & ne nudi sve potrebne mogućnosti, možete [stvoriti prilagođenu vrstu osjetljivih informacija u sigurnosnoj & PowerShell centra za usklađenost](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="a2838-114">Finally, if the UI doesn't provide all the options you need, you can [create a custom sensitive information type in Security & Compliance Center PowerShell](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span></span> <span data-ttu-id="a2838-115">Počevši od XML datoteke možete koristiti svaku dostupnu mogućnost.</span><span class="sxs-lookup"><span data-stu-id="a2838-115">By starting with an XML file, you can use every option available.</span></span>
