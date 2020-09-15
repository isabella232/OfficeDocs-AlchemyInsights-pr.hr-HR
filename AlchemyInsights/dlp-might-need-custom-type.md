---
title: DLP možda treba prilagođenu vrstu
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 72b16d437f97de27cbdc364f022c3e2059b31ef0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47712176"
---
# <a name="dlp-might-need-a-custom-type"></a><span data-ttu-id="45bfa-102">DLP možda treba prilagođenu vrstu</span><span class="sxs-lookup"><span data-stu-id="45bfa-102">DLP might need a custom type</span></span>

<span data-ttu-id="45bfa-103">**Važno**: Tijekom ovih neočekivanih vremena poduzimamo korake kako bismo osigurali da servisi SharePoint Online i OneDrive i dalje budu široko raspoloživi – dodatne informacije potražite u [Privremene prilagodbe značajke SharePoint Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="45bfa-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="45bfa-104">**DLP može zahtijevati prilagođenu vrstu podataka**</span><span class="sxs-lookup"><span data-stu-id="45bfa-104">**DLP may require a custom information type**</span></span>

<span data-ttu-id="45bfa-105">Pomoću pravilnika o sprječavanju gubitka podataka (DLP-a) možete identificirati i zaštititi osjetljive podatke u tvrtki ili ustanovi.</span><span class="sxs-lookup"><span data-stu-id="45bfa-105">With a data loss prevention (DLP) policy, you can identify and protect sensitive data in your organization.</span></span> <span data-ttu-id="45bfa-106">U nekim slučajevima možda ćete morati stvoriti vlastite **prilagođene** vrste osjetljivih podataka da biste zaštitili podatke tvrtke ili ustanove.</span><span class="sxs-lookup"><span data-stu-id="45bfa-106">In some scenarios, you might need to create your own **custom** sensitive information type to protect your organization's data.</span></span>

<span data-ttu-id="45bfa-107">Tvrtka ili ustanova možda će, primjerice, morati identificirati i zaštititi ID-ove zaposlenika ili druge podatke u nekom obliku specifičnom za vašu tvrtku ili ustanovu. Ako je tako, dodatne informacije potražite u sljedećim člancima.</span><span class="sxs-lookup"><span data-stu-id="45bfa-107">For example, your organization might need to identify and protect employee IDs or other data in some format specific to your org. If so, see the following articles for more information.</span></span>
  
 <span data-ttu-id="45bfa-108">**Prilagođavanje ugrađene vrste osjetljivih informacija**</span><span class="sxs-lookup"><span data-stu-id="45bfa-108">**Customize a built-in sensitive information type**</span></span>
  
<span data-ttu-id="45bfa-109">Ako bi ugrađena vrsta osjetljive informacije zadovoljile vaše potrebe samo s nekoliko ugađanje, možete [prilagoditi ugrađenu vrstu osjetljivih podataka](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="45bfa-109">If a built-in sensitive information type would meet your needs with just a few tweaks, you can [customize a built-in sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type).</span></span> <span data-ttu-id="45bfa-110">Možete, primjerice, dodavati ili uklanjati ključne riječi ili dodavati ili uklanjati popratne dokaze, kao što su Datum ili adresa.</span><span class="sxs-lookup"><span data-stu-id="45bfa-110">For example, you can add or remove keywords, or add or remove supporting evidence such as a date or address.</span></span>
  
 <span data-ttu-id="45bfa-111">**Stvaranje prilagođene vrste osjetljivih podataka**</span><span class="sxs-lookup"><span data-stu-id="45bfa-111">**Create a custom sensitive information type**</span></span>
  
<span data-ttu-id="45bfa-112">No ako morate identificirati i zaštititi različitu vrstu osjetljivih podataka, možete [stvoriti prilagođenu vrstu osjetljivog podataka](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) u korisničkom sučelju centra za zaštitu & usklađenosti.</span><span class="sxs-lookup"><span data-stu-id="45bfa-112">But if you need to identify and protect a different type of sensitive information altogether, you can [create a custom sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) in the UI of the Security & Compliance Center.</span></span>
  
<span data-ttu-id="45bfa-113">**Stvaranje prilagođene vrste osjetljivih informacija u sigurnosnom & PowerShell centra za usklađenost**</span><span class="sxs-lookup"><span data-stu-id="45bfa-113">**Create a custom sensitive information type in Security & Compliance Center PowerShell**</span></span>

<span data-ttu-id="45bfa-114">Na kraju, ako korisničko sučelje ne sadrži sve potrebne mogućnosti, možete [stvoriti prilagođenu vrstu osjetljivog podataka u sigurnosnom & PowerShell centra za usklađenost](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="45bfa-114">Finally, if the UI doesn't provide all the options you need, you can [create a custom sensitive information type in Security & Compliance Center PowerShell](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span></span> <span data-ttu-id="45bfa-115">Pokretanjem XML datoteke možete koristiti svaku dostupnu mogućnost.</span><span class="sxs-lookup"><span data-stu-id="45bfa-115">By starting with an XML file, you can use every option available.</span></span>
