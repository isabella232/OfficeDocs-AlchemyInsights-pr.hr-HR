---
title: Nije moguće pristupiti javnim mapama
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: af5bd57512ee917d6e22d3838d55a2a1d62750d4
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819504"
---
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="f99a7-102">Outlook se ne može povezati s javnim mapama</span><span class="sxs-lookup"><span data-stu-id="f99a7-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="f99a7-103">Ako pristup javnim mapama ne funkcionira za neke korisnike, pokušajte sljedeće:</span><span class="sxs-lookup"><span data-stu-id="f99a7-103">If public folder access isn't working for some users, try the following:</span></span>

<span data-ttu-id="f99a7-104">Povežite se s ljuskom EXO PowerShell i konfigurirajte parametar DefaultPublicFolderMailbox na korisničkom računu problema tako da odgovara parametru na radnom korisničkom računu.</span><span class="sxs-lookup"><span data-stu-id="f99a7-104">Connect to EXO PowerShell and configure the DefaultPublicFolderMailbox parameter on the problem user account to match the parameter on a working user account.</span></span>

<span data-ttu-id="f99a7-105">Primjer:</span><span class="sxs-lookup"><span data-stu-id="f99a7-105">Example:</span></span>

<span data-ttu-id="f99a7-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span><span class="sxs-lookup"><span data-stu-id="f99a7-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="f99a7-107">Set-Mailbox Korisnik -DefaultPublicFolderMailbox \<value from previous command></span><span class="sxs-lookup"><span data-stu-id="f99a7-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="f99a7-108">Pričekajte najmanje jedan sat da bi promjena snazi.</span><span class="sxs-lookup"><span data-stu-id="f99a7-108">Wait at least one hour for the change to take effect.</span></span>

<span data-ttu-id="f99a7-109">Ako problem i dalje postoji, slijedite ovaj [postupak da biste otklonili](https://aka.ms/pfcte) poteškoće s pristupom javnim mapama pomoću programa Outlook.</span><span class="sxs-lookup"><span data-stu-id="f99a7-109">If the issue remains, please follow [this procedure](https://aka.ms/pfcte) to troubleshoot public folder access issues using Outlook.</span></span>
 
<span data-ttu-id="f99a7-110">**Da biste upravljali korisnicima koji mogu pristupati javnim mapama pomoću programa Outlook:**</span><span class="sxs-lookup"><span data-stu-id="f99a7-110">**To control which users can access public folders using Outlook**:</span></span>

1.  <span data-ttu-id="f99a7-111">Korištenje Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true ili $false</span><span class="sxs-lookup"><span data-stu-id="f99a7-111">Use Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false</span></span>  
      
    <span data-ttu-id="f99a7-112">$true: omogući korisnicima pristup javnim mapama u programu Outlook</span><span class="sxs-lookup"><span data-stu-id="f99a7-112">$true: Allow users access public folders in Outlook</span></span>  
      
    <span data-ttu-id="f99a7-113">$false: onemogućivanje korisničkog pristupa javnim mapama u programu Outlook.</span><span class="sxs-lookup"><span data-stu-id="f99a7-113">$false: Prevent user access to public folders in Outlook.</span></span> <span data-ttu-id="f99a7-114">To je zadana vrijednost.</span><span class="sxs-lookup"><span data-stu-id="f99a7-114">This is the default value.</span></span>  
        
2.  <span data-ttu-id="f99a7-115">Set-OrganizationConfig -PublicFolderShowClientControl $true</span><span class="sxs-lookup"><span data-stu-id="f99a7-115">Set-OrganizationConfig -PublicFolderShowClientControl $true</span></span>   
      
<span data-ttu-id="f99a7-116">**Napomena** Taj postupak može upravljati vezama samo s klijentima programa Outlook za računala za Windows.</span><span class="sxs-lookup"><span data-stu-id="f99a7-116">**Note** This procedure can control connections only with Outlook desktop for Windows clients.</span></span> <span data-ttu-id="f99a7-117">Korisnik može nastaviti pristupati javnim mapama pomoću aplikacije OWA ili Outlook za Mac.</span><span class="sxs-lookup"><span data-stu-id="f99a7-117">A user can continue accessing public folders using OWA or Outlook for Mac.</span></span>
 
<span data-ttu-id="f99a7-118">Dodatne informacije potražite u članku [Najava podrške za kontrolirane veze s javnim mapama u programu Outlook](https://aka.ms/controlpf).</span><span class="sxs-lookup"><span data-stu-id="f99a7-118">For more info, see [Announcing Support for Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf).</span></span>