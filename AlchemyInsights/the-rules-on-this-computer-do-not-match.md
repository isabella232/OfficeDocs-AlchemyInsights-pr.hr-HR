---
title: 'Pogreška: Pravila na ovom računalu ne podudaraju se'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: c0982da82826d1644f437b19e0d343a59d7ac473
ms.sourcegitcommit: e09af4285c6b81ca0a5320fdb811713ac25748c3
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/09/2020
ms.locfileid: "44664238"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a><span data-ttu-id="b4489-102">Pogreška: Pravila na ovom računalu ne podudaraju se</span><span class="sxs-lookup"><span data-stu-id="b4489-102">Error: The rules on this computer do not match</span></span>

<span data-ttu-id="b4489-103">Da biste vidjeli ažurirani status ovog poznatog problema, pogledajte [Pravila na ovom računalu ne odgovaraju pravilima na sustavu Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span><span class="sxs-lookup"><span data-stu-id="b4489-103">To see updated status of this known issue, see [The rules on this computer do not match the rules on Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span></span>

<span data-ttu-id="b4489-104">Tim programa Outlook implementirao je popravak u međuverziji 12928.10000.</span><span class="sxs-lookup"><span data-stu-id="b4489-104">The Outlook Team has implemented a fix in Build 12928.10000.</span></span> <span data-ttu-id="b4489-105">škripac je već at Insider Brz i htijenje otiđite na Mjesec Chanel krajem Lipanj 2020.</span><span class="sxs-lookup"><span data-stu-id="b4489-105">The fix is already at Insider Fast and will go to Monthly Channel in late June 2020.</span></span> <span data-ttu-id="b4489-106">Nakon što ste fiksne graditi možete dobiti upit "Koja pravila želite zadržati" posljednji put.</span><span class="sxs-lookup"><span data-stu-id="b4489-106">Once you have the fixed build you may get the prompt "Which rules do you want to keep" one last time.</span></span> <span data-ttu-id="b4489-107">Odaberite Poslužitelj kada se to od vas zatraži, a zatim se vratite u Outlook i ponovno omogućite sva onemogućena pravila.</span><span class="sxs-lookup"><span data-stu-id="b4489-107">Choose Server when prompted and then go back in Outlook and re-enable any rules that were disabled.</span></span>

<span data-ttu-id="b4489-108">Dok popravak je dostupan, koristite sljedeće zaobilazno rješenje:</span><span class="sxs-lookup"><span data-stu-id="b4489-108">Until the fix is available please use the following workaround:</span></span>

<span data-ttu-id="b4489-109">**Zaobilazno rješenje**: U nedavnim izvješćima došlo je do problema za one koji su stvorili samo klijentska pravila na radnoj površini programa Outlook.</span><span class="sxs-lookup"><span data-stu-id="b4489-109">**Workaround**: In recent reports, the issue has occurred for those that have only created client rules in Outlook desktop.</span></span> <span data-ttu-id="b4489-110">Ako nastavite s time, razmislite o brisanju pravila, a zatim stvorite i uredite pravila samo u programu OWA (Outlook Web App) dok se problem ne riješi.</span><span class="sxs-lookup"><span data-stu-id="b4489-110">If you continue to run into the problem, consider deleting the rules and then create and edit rules only in OWA (Outlook Web App) until the issue is resolved.</span></span>

<span data-ttu-id="b4489-111">Ako pravila ne možete ručno izbrisati, možete pokrenuti naredbu programa Outlook kada pokrenete Outlook pokretanjem programa Outlook.exe /cleanrules.</span><span class="sxs-lookup"><span data-stu-id="b4489-111">If you cannot delete the rules manually you can run an Outlook command when you start Outlook by running Outlook.exe /cleanrules.</span></span> <span data-ttu-id="b4489-112">Time će se izbrisati pravila klijenta i poslužitelja.</span><span class="sxs-lookup"><span data-stu-id="b4489-112">This will delete both the client and server rules.</span></span> <span data-ttu-id="b4489-113">Izbrisat će sva pravila za sve račune u profilu programa Outlook.</span><span class="sxs-lookup"><span data-stu-id="b4489-113">It will delete all of the rules for all of the accounts in the Outlook Profile.</span></span> <span data-ttu-id="b4489-114">Ova naredba je dodatno dokumentirana u članku Command-line skretnice.</span><span class="sxs-lookup"><span data-stu-id="b4489-114">This command is further documented in the Command-line switches article.</span></span>

