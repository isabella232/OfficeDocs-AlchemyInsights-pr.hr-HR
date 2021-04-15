---
title: 'Pogreška: pravila na ovom računalu ne odgovaraju'
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: c46eb856baafbef9bc3b7fa34a0258ef16923fb8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51782944"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a><span data-ttu-id="2bac4-102">Pogreška: pravila na ovom računalu ne odgovaraju</span><span class="sxs-lookup"><span data-stu-id="2bac4-102">Error: The rules on this computer do not match</span></span>

<span data-ttu-id="2bac4-103">Da biste vidjeli ažurirani status tog poznatog problema, [pogledajte članak Pravila na ovom računalu ne](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0) odgovaraju pravilima u sustavu Microsoft Exchange</span><span class="sxs-lookup"><span data-stu-id="2bac4-103">To see updated status of this known issue, see [The rules on this computer do not match the rules on Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span></span>

<span data-ttu-id="2bac4-104">Tim za Outlook implementiran je popravak u međuverziji 12928.10000.</span><span class="sxs-lookup"><span data-stu-id="2bac4-104">The Outlook Team has implemented a fix in Build 12928.10000.</span></span> <span data-ttu-id="2bac4-105">Popravak se već nalazi u programu Insider Fast i krajem lipnja 2020. idite na Mjesečni kanal.</span><span class="sxs-lookup"><span data-stu-id="2bac4-105">The fix is already at Insider Fast and will go to Monthly Channel in late June 2020.</span></span> <span data-ttu-id="2bac4-106">Kada popravite međuverziju, možda će vam se po posljednji put pojaviti upit "Koja pravila želite zadržati".</span><span class="sxs-lookup"><span data-stu-id="2bac4-106">Once you have the fixed build you may get the prompt "Which rules do you want to keep" one last time.</span></span> <span data-ttu-id="2bac4-107">Kada se to od vas zatraži, odaberite Poslužitelj, a zatim se vratite u Outlook i ponovno omogućite sva onemogućena pravila.</span><span class="sxs-lookup"><span data-stu-id="2bac4-107">Choose Server when prompted and then go back in Outlook and re-enable any rules that were disabled.</span></span>

<span data-ttu-id="2bac4-108">Dok popravak ne bude dostupan, upotrijebite sljedeće zaobilazno rješenje:</span><span class="sxs-lookup"><span data-stu-id="2bac4-108">Until the fix is available please use the following workaround:</span></span>

<span data-ttu-id="2bac4-109">**Zaobilazno** rješenje: u nedavnim izvješćima pojavio se problem za one koji su stvorili samo klijentska pravila u programu Outlook za stolna računala.</span><span class="sxs-lookup"><span data-stu-id="2bac4-109">**Workaround**: In recent reports, the issue has occurred for those that have only created client rules in Outlook desktop.</span></span> <span data-ttu-id="2bac4-110">Ako naiđete na problem, razmislite o brisanju pravila, a zatim pravila stvarajte i uređujte samo u aplikaciji OWA (Outlook Web App) dok se problem ne riješi.</span><span class="sxs-lookup"><span data-stu-id="2bac4-110">If you continue to run into the problem, consider deleting the rules and then create and edit rules only in OWA (Outlook Web App) until the issue is resolved.</span></span>

<span data-ttu-id="2bac4-111">Ako ne možete ručno izbrisati pravila, prilikom pokretanja programa Outlook možete pokrenuti naredbu programa Outlook pokretanjem Outlook.exe /cleanrules.</span><span class="sxs-lookup"><span data-stu-id="2bac4-111">If you cannot delete the rules manually you can run an Outlook command when you start Outlook by running Outlook.exe /cleanrules.</span></span> <span data-ttu-id="2bac4-112">Time ćete izbrisati i pravila klijenta i poslužitelja.</span><span class="sxs-lookup"><span data-stu-id="2bac4-112">This will delete both the client and server rules.</span></span> <span data-ttu-id="2bac4-113">Izbrisat će sva pravila za sve račune u profilu programa Outlook.</span><span class="sxs-lookup"><span data-stu-id="2bac4-113">It will delete all of the rules for all of the accounts in the Outlook Profile.</span></span> <span data-ttu-id="2bac4-114">Ta je naredba dodatno dokumentirana u članku s prebacivanjem naredbenog retka.</span><span class="sxs-lookup"><span data-stu-id="2bac4-114">This command is further documented in the Command-line switches article.</span></span>

