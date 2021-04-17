---
title: Prijava u Windows 10 bez lozinke
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
- "9001690"
- "3766"
ms.openlocfilehash: 1c03f00f7b41ea16d3106b19b998edeea6114603
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830538"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a><span data-ttu-id="5b504-102">Prijava u Windows 10 bez lozinke</span><span class="sxs-lookup"><span data-stu-id="5b504-102">Sign-in to Windows 10 without using a password</span></span>

<span data-ttu-id="5b504-103">Da biste izbjegli upis lozinke prilikom pokretanja sustava Windows, preporučujemo da koristite jednu od sigurnih mogućnosti prijave u Windows Hello, kao što su PIN, prepoznavanje lica ili otisak prsta, ako su dostupne.</span><span class="sxs-lookup"><span data-stu-id="5b504-103">To avoid having to type a password at Windows startup, we recommend you use one of the Windows Hello secure sign-in options, like a PIN, face recognition, or fingerprint, if available.</span></span> <span data-ttu-id="5b504-104">Ako zaista želite onemogućiti sigurnu prijavu, pročitajte upute za automatsku prijavu u Windows 10 u nastavku.</span><span class="sxs-lookup"><span data-stu-id="5b504-104">If you really want to disable secure sign-in, see the "Automatically sign in to Windows 10" instructions below.</span></span>

<span data-ttu-id="5b504-105">**Secure Windows Hello alternative to the account password**</span><span class="sxs-lookup"><span data-stu-id="5b504-105">**Secure Windows Hello alternatives to the account password**</span></span>

<span data-ttu-id="5b504-106">Otvorite **Postavke > računi > mogućnosti prijave** (ili kliknite [ovdje).](ms-settings:signinoptions?activationSource=GetHelp)</span><span class="sxs-lookup"><span data-stu-id="5b504-106">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="5b504-107">Na popisu će biti dostupne mogućnosti prijave.</span><span class="sxs-lookup"><span data-stu-id="5b504-107">Available sign-in options will be listed.</span></span> <span data-ttu-id="5b504-108">Na primjer:</span><span class="sxs-lookup"><span data-stu-id="5b504-108">For example:</span></span>

![Mogućnosti prijave.](media/sign-in-options.png)

<span data-ttu-id="5b504-110">Kliknite ili dodirnite jednu od mogućnosti da biste je konfigurirali.</span><span class="sxs-lookup"><span data-stu-id="5b504-110">Click or tap one of the options to configure it.</span></span> <span data-ttu-id="5b504-111">Kada sljedeći put pokrenete ili otključate Windows, moći ćete koristiti novu mogućnost umjesto lozinke.</span><span class="sxs-lookup"><span data-stu-id="5b504-111">Next time you start or unlock Windows, you will be able to use the new option instead of a password.</span></span> 

<span data-ttu-id="5b504-112">**Automatska prijava u Windows 10**</span><span class="sxs-lookup"><span data-stu-id="5b504-112">**Automatically sign-in to Windows 10**</span></span>

<span data-ttu-id="5b504-113">**Napomena:** automatska prijava praktična je, ali predstavlja sigurnosni rizik, osobito ako pc može pristupiti više osoba.</span><span class="sxs-lookup"><span data-stu-id="5b504-113">**Note**: Automatic sign-in is convenient, but introduces a security risk, especially if your PC is accessible by multiple people.</span></span> 

1. <span data-ttu-id="5b504-114">Kliknite ili dodirnite **gumb Start** na programskoj traci.</span><span class="sxs-lookup"><span data-stu-id="5b504-114">Click or tap the **Start** button in the Taskbar.</span></span>

2. <span data-ttu-id="5b504-115">Upišite **netplwiz** i pritisnite tipku Enter da biste otvorili prozor Korisnički računi.</span><span class="sxs-lookup"><span data-stu-id="5b504-115">Type **netplwiz** and hit the Enter key to open the User Accounts window.</span></span>

3. <span data-ttu-id="5b504-116">U **korisničkim računima** kliknite račun na koji se želite automatski prijaviti prilikom pokretanja sustava Windows.</span><span class="sxs-lookup"><span data-stu-id="5b504-116">In **User Accounts**, click the account you want to automatically sign in to when Windows starts.</span></span>

4. <span data-ttu-id="5b504-117">Poništite potvrdni okvir "Korisnici moraju unijeti korisničko ime i lozinku da bi koristili ovo računalo".</span><span class="sxs-lookup"><span data-stu-id="5b504-117">Uncheck the "Users must enter a user name and password to use this computer" checkbox.</span></span>

    ![Korisnici moraju unijeti korisničko ime i lozinku.](media/users-must-enter-username.png)

5. <span data-ttu-id="5b504-119">Kliknite **U redu**.</span><span class="sxs-lookup"><span data-stu-id="5b504-119">Click **OK**.</span></span> <span data-ttu-id="5b504-120">Od vas će se tražiti da unesete i potvrdite lozinku za odabrani račun.</span><span class="sxs-lookup"><span data-stu-id="5b504-120">You will be asked to enter and confirm the password for the account you selected.</span></span> <span data-ttu-id="5b504-121">Kliknite **U redu da** biste dovršili.</span><span class="sxs-lookup"><span data-stu-id="5b504-121">Click **OK** to finish.</span></span> <span data-ttu-id="5b504-122">Prilikom sljedećeg pokretanja sustava Windows 10 automatski će se prijaviti na odabrani račun.</span><span class="sxs-lookup"><span data-stu-id="5b504-122">Next time Windows 10 starts, it will automatically sign in to the account you selected.</span></span>
