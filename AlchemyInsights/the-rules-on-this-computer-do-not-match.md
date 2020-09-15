---
title: 'Pogreška: pravila na ovom računalu ne podudaraju se'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: c2feb6da651d8b3eb7af6a057335b28d26f9e7f6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690955"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a><span data-ttu-id="52d67-102">Pogreška: pravila na ovom računalu ne podudaraju se</span><span class="sxs-lookup"><span data-stu-id="52d67-102">Error: The rules on this computer do not match</span></span>

<span data-ttu-id="52d67-103">Da biste vidjeli ažurirani status tog poznatog problema, pročitajte članak [pravila na ovom računalu ne podudaraju se s pravilima u sustavu Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span><span class="sxs-lookup"><span data-stu-id="52d67-103">To see updated status of this known issue, see [The rules on this computer do not match the rules on Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span></span>

<span data-ttu-id="52d67-104">Tim za Outlook implementirao je popravak u Međuaplikaciji 12928,10000.</span><span class="sxs-lookup"><span data-stu-id="52d67-104">The Outlook Team has implemented a fix in Build 12928.10000.</span></span> <span data-ttu-id="52d67-105">Popravak je već brzo uključen u Insider i bit će na mjesečnom kanalu krajem lipnja 2020.</span><span class="sxs-lookup"><span data-stu-id="52d67-105">The fix is already at Insider Fast and will go to Monthly Channel in late June 2020.</span></span> <span data-ttu-id="52d67-106">Kada završite s ispravnom izgradnjom, možda ćete dobiti upit "koja pravila želite zadržati" posljednji put.</span><span class="sxs-lookup"><span data-stu-id="52d67-106">Once you have the fixed build you may get the prompt "Which rules do you want to keep" one last time.</span></span> <span data-ttu-id="52d67-107">Kada se to od vas zatraži, odaberite poslužitelj, a zatim se vratite u Outlook i ponovno omogućite onemogućena pravila.</span><span class="sxs-lookup"><span data-stu-id="52d67-107">Choose Server when prompted and then go back in Outlook and re-enable any rules that were disabled.</span></span>

<span data-ttu-id="52d67-108">Dok popravak ne bude dostupan, upotrijebite sljedeće zaobilazno rješenje:</span><span class="sxs-lookup"><span data-stu-id="52d67-108">Until the fix is available please use the following workaround:</span></span>

<span data-ttu-id="52d67-109">**Zaobilazno rješenje**: u nedavnim izvješćima došlo je do problema za one koji su stvorili samo klijentska pravila u radnoj površini programa Outlook.</span><span class="sxs-lookup"><span data-stu-id="52d67-109">**Workaround**: In recent reports, the issue has occurred for those that have only created client rules in Outlook desktop.</span></span> <span data-ttu-id="52d67-110">Ako i dalje pokrenete problem, razmotrite brisanje pravila, a zatim stvaranje i uređivanje pravila samo u aplikaciji OWA (Outlook Web App) dok se problem ne riješi.</span><span class="sxs-lookup"><span data-stu-id="52d67-110">If you continue to run into the problem, consider deleting the rules and then create and edit rules only in OWA (Outlook Web App) until the issue is resolved.</span></span>

<span data-ttu-id="52d67-111">Ako ne možete ručno izbrisati pravila, možete pokrenuti naredbu programa Outlook prilikom pokretanja programa Outlook pokretanjem Outlook.exe/cleanrules.</span><span class="sxs-lookup"><span data-stu-id="52d67-111">If you cannot delete the rules manually you can run an Outlook command when you start Outlook by running Outlook.exe /cleanrules.</span></span> <span data-ttu-id="52d67-112">Time ćete izbrisati i pravila klijenta i poslužitelja.</span><span class="sxs-lookup"><span data-stu-id="52d67-112">This will delete both the client and server rules.</span></span> <span data-ttu-id="52d67-113">Izbrisat će sva pravila za sve račune u profilu programa Outlook.</span><span class="sxs-lookup"><span data-stu-id="52d67-113">It will delete all of the rules for all of the accounts in the Outlook Profile.</span></span> <span data-ttu-id="52d67-114">Ta je naredba dodatno dokumentirana u članku prekidača naredbenog retka.</span><span class="sxs-lookup"><span data-stu-id="52d67-114">This command is further documented in the Command-line switches article.</span></span>

