---
title: Prijava u Windows 10 bez korištenja lozinke
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001690"
- "3766"
ms.openlocfilehash: 839b945c457cb007f13605c5b903ded75dadd1d7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47719945"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a><span data-ttu-id="25a13-102">Prijava u Windows 10 bez korištenja lozinke</span><span class="sxs-lookup"><span data-stu-id="25a13-102">Sign-in to Windows 10 without using a password</span></span>

<span data-ttu-id="25a13-103">Da biste izbjegli unos lozinke pri pokretanju sustava Windows, preporučujemo vam da koristite neku od mogućnosti za prijavu u Windows Hello, kao što su PIN, prepoznavanje lica ili otisak prsta, ako je dostupan.</span><span class="sxs-lookup"><span data-stu-id="25a13-103">To avoid having to type a password at Windows startup, we recommend you use one of the Windows Hello secure sign-in options, like a PIN, face recognition, or fingerprint, if available.</span></span> <span data-ttu-id="25a13-104">Ako zaista želite onemogućiti sigurnu prijavu, pročitajte upute u nastavku: "automatsko prijavljivanje u Windows 10".</span><span class="sxs-lookup"><span data-stu-id="25a13-104">If you really want to disable secure sign-in, see the "Automatically sign in to Windows 10" instructions below.</span></span>

<span data-ttu-id="25a13-105">**Sigurni Windows Hello alternative za lozinku računa**</span><span class="sxs-lookup"><span data-stu-id="25a13-105">**Secure Windows Hello alternatives to the account password**</span></span>

<span data-ttu-id="25a13-106">Idite na **postavke > računi > mogućnosti prijave** (ili kliknite [ovdje](ms-settings:signinoptions?activationSource=GetHelp)).</span><span class="sxs-lookup"><span data-stu-id="25a13-106">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="25a13-107">Dostupne mogućnosti prijave prikazat će se na popisu.</span><span class="sxs-lookup"><span data-stu-id="25a13-107">Available sign-in options will be listed.</span></span> <span data-ttu-id="25a13-108">Na primjer:</span><span class="sxs-lookup"><span data-stu-id="25a13-108">For example:</span></span>

![Mogućnosti prijave](media/sign-in-options.png)

<span data-ttu-id="25a13-110">Kliknite ili dodirnite neku od mogućnosti da biste je konfigurirali.</span><span class="sxs-lookup"><span data-stu-id="25a13-110">Click or tap one of the options to configure it.</span></span> <span data-ttu-id="25a13-111">Kada sljedeći put pokrenete ili otključate Windows, moći ćete koristiti novu mogućnost umjesto lozinke.</span><span class="sxs-lookup"><span data-stu-id="25a13-111">Next time you start or unlock Windows, you will be able to use the new option instead of a password.</span></span> 

<span data-ttu-id="25a13-112">**Automatsko prijavljivanje u Windows 10**</span><span class="sxs-lookup"><span data-stu-id="25a13-112">**Automatically sign-in to Windows 10**</span></span>

<span data-ttu-id="25a13-113">**Pažnja**: automatsko prijavljivanje povoljno je, ali predstavlja sigurnosni rizik, osobito ako je na PC-ju dostupan više osoba.</span><span class="sxs-lookup"><span data-stu-id="25a13-113">**Note**: Automatic sign-in is convenient, but introduces a security risk, especially if your PC is accessible by multiple people.</span></span> 

1. <span data-ttu-id="25a13-114">Kliknite ili dodirnite gumb **Start** na programskoj traci.</span><span class="sxs-lookup"><span data-stu-id="25a13-114">Click or tap the **Start** button in the Taskbar.</span></span>

2. <span data-ttu-id="25a13-115">Upišite **netplwiz** i pritisnite tipku ENTER da biste otvorili prozor korisnički računi.</span><span class="sxs-lookup"><span data-stu-id="25a13-115">Type **netplwiz** and hit the Enter key to open the User Accounts window.</span></span>

3. <span data-ttu-id="25a13-116">Na **korisničkim računima**kliknite račun na koji se želite automatski prijaviti prilikom pokretanja sustava Windows.</span><span class="sxs-lookup"><span data-stu-id="25a13-116">In **User Accounts**, click the account you want to automatically sign in to when Windows starts.</span></span>

4. <span data-ttu-id="25a13-117">Poništite potvrdni okvir "korisnici moraju unositi korisničko ime i lozinku da bi koristili ovo računalo".</span><span class="sxs-lookup"><span data-stu-id="25a13-117">Uncheck the "Users must enter a user name and password to use this computer" checkbox.</span></span>

    ![Korisnici moraju unijeti mogućnost korisničko ime i lozinku.](media/users-must-enter-username.png)

5. <span data-ttu-id="25a13-119">Kliknite **U redu**.</span><span class="sxs-lookup"><span data-stu-id="25a13-119">Click **OK**.</span></span> <span data-ttu-id="25a13-120">Od vas će se zatražiti da unesete i potvrdite lozinku za odabrani račun.</span><span class="sxs-lookup"><span data-stu-id="25a13-120">You will be asked to enter and confirm the password for the account you selected.</span></span> <span data-ttu-id="25a13-121">Kliknite **u redu** da biste završili.</span><span class="sxs-lookup"><span data-stu-id="25a13-121">Click **OK** to finish.</span></span> <span data-ttu-id="25a13-122">Kada se sljedeći put pokrene Windows 10, on će se automatski prijaviti na odabrani račun.</span><span class="sxs-lookup"><span data-stu-id="25a13-122">Next time Windows 10 starts, it will automatically sign in to the account you selected.</span></span>
