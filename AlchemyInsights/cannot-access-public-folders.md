---
title: Nije moguće pristupiti javnim mapama
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: d63a193585cb73c2ce8e160d413db4e837100d33
ms.sourcegitcommit: d3ace2376195d54229ee1e232daf8133ba4e58a9
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/03/2020
ms.locfileid: "47341395"
---
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="f21c2-102">Outlook se ne može povezati s javnim mapama</span><span class="sxs-lookup"><span data-stu-id="f21c2-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="f21c2-103">Ako pristup javnoj mapi ne funkcionira za neke korisnike, pokušajte sljedeće:</span><span class="sxs-lookup"><span data-stu-id="f21c2-103">If public folder access isn't working for some users, try the following:</span></span>

<span data-ttu-id="f21c2-104">Povežite se s programom EXO PowerShell i konfigurirajte parametar Defaultpublifoldermailbox na korisničkom računu problema da bi odgovarao parametru na radnom korisničkom računu.</span><span class="sxs-lookup"><span data-stu-id="f21c2-104">Connect to EXO PowerShell and configure the DefaultPublicFolderMailbox parameter on the problem user account to match the parameter on a working user account.</span></span>

<span data-ttu-id="f21c2-105">Primjer</span><span class="sxs-lookup"><span data-stu-id="f21c2-105">Example:</span></span>

<span data-ttu-id="f21c2-106">Nabavite-Mailbox WorkingUser | ft Defaultpublifoldermailbox, Effectivepublifoldermailbox</span><span class="sxs-lookup"><span data-stu-id="f21c2-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="f21c2-107">Problem s postavkom poštanskog sandučića – Defaultpublifoldermailbox \<value from previous command></span><span class="sxs-lookup"><span data-stu-id="f21c2-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="f21c2-108">Pričekajte najmanje jedan sat da bi promjena stupila na kraj.</span><span class="sxs-lookup"><span data-stu-id="f21c2-108">Wait at least one hour for the change to take effect.</span></span>

<span data-ttu-id="f21c2-109">Ako problem ostaje, slijedite [ovaj postupak](https://aka.ms/pfcte) da biste otklonili poteškoće s pristupom javnim mapama pomoću programa Outlook.</span><span class="sxs-lookup"><span data-stu-id="f21c2-109">If the issue remains, please follow [this procedure](https://aka.ms/pfcte) to troubleshoot public folder access issues using Outlook.</span></span>
 
<span data-ttu-id="f21c2-110">**Da biste kontrolirali koji korisnici mogu pristupati javnim mapama pomoću programa Outlook**:</span><span class="sxs-lookup"><span data-stu-id="f21c2-110">**To control which users can access public folders using Outlook**:</span></span>

1.  <span data-ttu-id="f21c2-111">Korištenje servisa set-CASMailbox <mailboxname> -publifolderclientaccess $TRUE ili $FALSE</span><span class="sxs-lookup"><span data-stu-id="f21c2-111">Use Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false</span></span>  
      
    <span data-ttu-id="f21c2-112">$true: korisnicima dopusti pristup javnim mapama u programu Outlook</span><span class="sxs-lookup"><span data-stu-id="f21c2-112">$true: Allow users access public folders in Outlook</span></span>  
      
    <span data-ttu-id="f21c2-113">$false: Onemogućivanje korisničkog pristupa javnim mapama u programu Outlook.</span><span class="sxs-lookup"><span data-stu-id="f21c2-113">$false: Prevent user access to public folders in Outlook.</span></span> <span data-ttu-id="f21c2-114">To je zadana vrijednost.</span><span class="sxs-lookup"><span data-stu-id="f21c2-114">This is the default value.</span></span>  
        
2.  <span data-ttu-id="f21c2-115">Set-OrganizationConfig-PublicFolderShowClientControl $true</span><span class="sxs-lookup"><span data-stu-id="f21c2-115">Set-OrganizationConfig -PublicFolderShowClientControl $true</span></span>   
      
<span data-ttu-id="f21c2-116">**Notes** Ovaj postupak može upravljati vezama samo s klijentskim računalima programa Outlook za Windows.</span><span class="sxs-lookup"><span data-stu-id="f21c2-116">**Note** This procedure can control connections only with Outlook desktop for Windows clients.</span></span> <span data-ttu-id="f21c2-117">Korisnik može nastaviti pristupati javnim mapama pomoću značajke OWA ili programa Outlook za Mac.</span><span class="sxs-lookup"><span data-stu-id="f21c2-117">A user can continue accessing public folders using OWA or Outlook for Mac.</span></span>
 
<span data-ttu-id="f21c2-118">Dodatne informacije potražite u članku [Objavljivanje podrške za kontrolirane veze s javnim mapama u programu Outlook](https://aka.ms/controlpf).</span><span class="sxs-lookup"><span data-stu-id="f21c2-118">For more info, see [Announcing Support for Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf).</span></span>