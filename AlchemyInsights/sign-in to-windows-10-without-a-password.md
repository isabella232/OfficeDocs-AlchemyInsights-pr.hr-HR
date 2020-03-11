---
title: Prijava u Windows 10 bez korištenja lozinke
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001690"
- "3766"
ms.openlocfilehash: 1f325eb7afb1e88457296e8187f8ba6dff2ebfe0
ms.sourcegitcommit: 00e4266575438f55bdc18db05ed54aafcb75a3c9
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/11/2020
ms.locfileid: "42588273"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a><span data-ttu-id="57467-102">Prijava u Windows 10 bez korištenja lozinke</span><span class="sxs-lookup"><span data-stu-id="57467-102">Sign-in to Windows 10 without using a password</span></span>

<span data-ttu-id="57467-103">Da biste izbjegli unos lozinke pri pokretanju sustava Windows, preporučujemo da koristite jednu od mogućnosti sigurne prijave u sustav Windows Hello, kao što su PIN, prepoznavanje lica ili otisak prsta, ako su dostupne.</span><span class="sxs-lookup"><span data-stu-id="57467-103">To avoid having to type a password at Windows startup, we recommend you use one of the Windows Hello secure sign-in options, like a PIN, face recognition, or fingerprint, if available.</span></span> <span data-ttu-id="57467-104">Ako zaista želite onemogućiti sigurnu prijavu, pogledajte upute "Automatska prijava u Windows 10" u nastavku.</span><span class="sxs-lookup"><span data-stu-id="57467-104">If you really want to disable secure sign-in, see the "Automatically sign in to Windows 10" instructions below.</span></span>

<span data-ttu-id="57467-105">**Sigurne mogućnosti značajke Windows Hello za lozinku računa**</span><span class="sxs-lookup"><span data-stu-id="57467-105">**Secure Windows Hello alternatives to the account password**</span></span>

<span data-ttu-id="57467-106">Idite na **Postavke > Računi > Mogućnosti prijave** (ili kliknite [ovdje](ms-settings:signinoptions?activationSource=GetHelp)).</span><span class="sxs-lookup"><span data-stu-id="57467-106">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="57467-107">Bit će navedene dostupne mogućnosti prijave.</span><span class="sxs-lookup"><span data-stu-id="57467-107">Available sign-in options will be listed.</span></span> <span data-ttu-id="57467-108">Na primjer:</span><span class="sxs-lookup"><span data-stu-id="57467-108">For example:</span></span>

![Opcije prijave.](media/sign-in-options.png)

<span data-ttu-id="57467-110">Kliknite ili dodirnite jednu od mogućnosti da biste je konfigurirali.</span><span class="sxs-lookup"><span data-stu-id="57467-110">Click or tap one of the options to configure it.</span></span> <span data-ttu-id="57467-111">Sljedeći put kada pokrenete ili otključate sustav Windows moći ćete koristiti novu mogućnost umjesto lozinke.</span><span class="sxs-lookup"><span data-stu-id="57467-111">Next time you start or unlock Windows, you will be able to use the new option instead of a password.</span></span> 

<span data-ttu-id="57467-112">**Automatska prijava u Windows 10**</span><span class="sxs-lookup"><span data-stu-id="57467-112">**Automatically sign-in to Windows 10**</span></span>

<span data-ttu-id="57467-113">**Napomena:** Automatska prijava prikladna je, ali predstavlja sigurnosni rizik, osobito ako je vašem PC-ju dostupno više osoba.</span><span class="sxs-lookup"><span data-stu-id="57467-113">**Note**: Automatic sign-in is convenient, but introduces a security risk, especially if your PC is accessible by multiple people.</span></span> 

1. <span data-ttu-id="57467-114">Kliknite ili dodirnite gumb **Start** na programskoj traci.</span><span class="sxs-lookup"><span data-stu-id="57467-114">Click or tap the **Start** button in the Taskbar.</span></span>

2. <span data-ttu-id="57467-115">Tip **netplwiz** i pogodak Ulaziti ključ to OpenBSD Korisnik Računi Windows.</span><span class="sxs-lookup"><span data-stu-id="57467-115">Type **netplwiz** and hit the Enter key to open the User Accounts window.</span></span>

3. <span data-ttu-id="57467-116">U **odjeljku Korisnički računi**kliknite račun na koji se želite automatski prijaviti prilikom pokretanja sustava Windows.</span><span class="sxs-lookup"><span data-stu-id="57467-116">In **User Accounts**, click the account you want to automatically sign in to when Windows starts.</span></span>

4. <span data-ttu-id="57467-117">Koji se ne da nadzirati " korisnik morati ulaziti korisničko ime i lozinka korištenje ovaj računalo" ček.</span><span class="sxs-lookup"><span data-stu-id="57467-117">Uncheck the "Users must enter a user name and password to use this computer" checkbox.</span></span>

    ![Korisnici moraju unijeti opciju korisničkog imena i lozinke.](media/users-must-enter-username.png)

5. <span data-ttu-id="57467-119">Kliknite **U redu**.</span><span class="sxs-lookup"><span data-stu-id="57467-119">Click **OK**.</span></span> <span data-ttu-id="57467-120">Od vas će se tražiti da unesete i potvrdite lozinku za odabrani račun.</span><span class="sxs-lookup"><span data-stu-id="57467-120">You will be asked to enter and confirm the password for the account you selected.</span></span> <span data-ttu-id="57467-121">Kliknite **U redu** da biste završili.</span><span class="sxs-lookup"><span data-stu-id="57467-121">Click **OK** to finish.</span></span> <span data-ttu-id="57467-122">Sljedeći put kada se Sustav Windows 10 pokrene, automatski će se prijaviti na odabrani račun.</span><span class="sxs-lookup"><span data-stu-id="57467-122">Next time Windows 10 starts, it will automatically sign in to the account you selected.</span></span>
