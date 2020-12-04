---
title: Napredni koncepti provjere autentičnosti koji se odnose na Microsoft Edge
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003931"
- "6986"
ms.openlocfilehash: 241d594fac6664dd1e85fd60e30a6344c432555e
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573297"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a><span data-ttu-id="bb02c-102">Napredni koncepti provjere autentičnosti koji se odnose na Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="bb02c-102">Advanced authentication concepts applicable to Microsoft Edge</span></span>

<span data-ttu-id="bb02c-103">Slijede Napredni koncepti provjere autentičnosti koji su primjenjivi na Microsoft Edge:</span><span class="sxs-lookup"><span data-stu-id="bb02c-103">Following are the advanced authentication concepts that are applicable to Microsoft Edge:</span></span>

<span data-ttu-id="bb02c-104">**Proaktivna provjera autentičnosti**</span><span class="sxs-lookup"><span data-stu-id="bb02c-104">**Proactive Authentication**</span></span>

<span data-ttu-id="bb02c-105">Kada omogućite pravilo [Proactiveauthenabled](https://go.microsoft.com/fwlink/?linkid=2134621) , Microsoft Edge nastojat će proaktivno provjeriti autentičnost korisnika potpisanih putem Microsoftova servisa.</span><span class="sxs-lookup"><span data-stu-id="bb02c-105">When you enable the [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) policy, Microsoft Edge will try to proactively authenticate signed-in users through Microsoft services.</span></span> <span data-ttu-id="bb02c-106">U pravilnim intervalima koristit će internetski servis za provjeru ažuriranog manifesta koji sadrži konfiguraciju koja regulira proaktivnu provjeru autentičnosti.</span><span class="sxs-lookup"><span data-stu-id="bb02c-106">At regular intervals, it will use an online service to check for an updated manifest that contains the configuration governing Proactive Authentication.</span></span>

<span data-ttu-id="bb02c-107">Prednosti: proaktivna provjera autentičnosti omogućuje provjeru autentičnosti ključnim servisima, kao što je stranica nove kartice sustava Office.</span><span class="sxs-lookup"><span data-stu-id="bb02c-107">Benefits: Proactive Authentication enables authentication to key services, such as the Office New Tab Page.</span></span> <span data-ttu-id="bb02c-108">Osim toga, ako se Bing koristi kao tražilica, proaktivna provjera autentičnosti poboljšava performanse adresne trake i olakšava stvaranje personalizirane rezultate pretraživanja na potrebe poslovanja.</span><span class="sxs-lookup"><span data-stu-id="bb02c-108">Also, if Bing is used as the search engine, Proactive Authentication improves the performance of the address bar and helps generate search results personalized to the needs of your business.</span></span>

<span data-ttu-id="bb02c-109">**Windows Hello CredUI za NTLM provjeru autentičnosti**</span><span class="sxs-lookup"><span data-stu-id="bb02c-109">**Windows Hello CredUI for NTLM Authentication**</span></span>

<span data-ttu-id="bb02c-110">Ako jedinstvena prijava (SSO) nije dostupna kada se web-mjesto pokuša prijavljivati korisniku putem mehanizma NTLM ili pregovara, ta će značajka omogućiti korisniku zajedničko korištenje vjerodajnica za OS uz web-mjesto i zadovoljavanje izazova za provjeru autentičnosti pomoću korisničkog sučelja za Windows Hello Cred.</span><span class="sxs-lookup"><span data-stu-id="bb02c-110">If single sign-on (SSO) isn't available when a website tries to sign on the user through the NTLM or Negotiate mechanism, this feature will allow the user to share the OS credentials with the website and to satisfy the authentication challenge by using Windows Hello Cred UI.</span></span> <span data-ttu-id="bb02c-111">Taj će se tijek prijave prikazivati samo u sustavu Windows 10 i to samo za korisnike koji ne dobiju SSO tijekom programa NTLM ili pregovarača.</span><span class="sxs-lookup"><span data-stu-id="bb02c-111">This sign-on flow will appear only in Windows 10 and only for users who don't get SSO during an NTLM or a Negotiate challenge.</span></span>

<span data-ttu-id="bb02c-112">**Automatsko prijavljivanje pomoću spremljenih lozinki**</span><span class="sxs-lookup"><span data-stu-id="bb02c-112">**Use saved passwords to sign on automatically**</span></span>

<span data-ttu-id="bb02c-113">Korisnici koji spremaju lozinke u pregledniku Microsoft Edge mogu omogućiti automatsko prijavljivanje na web-mjesta na kojima su spremljene vjerodajnice.</span><span class="sxs-lookup"><span data-stu-id="bb02c-113">Users who save passwords in Microsoft Edge can enable automatic sign-on to websites where they have saved credentials.</span></span> <span data-ttu-id="bb02c-114">Korisnici mogu uključiti ili isključiti ovu značajku na servisu edge://settings/passwords, a možete je konfigurirati u pravilima [upravitelja lozinki](https://go.microsoft.com/fwlink/?linkid=2134622) .</span><span class="sxs-lookup"><span data-stu-id="bb02c-114">Users can turn this feature on or off in edge://settings/passwords, and you can configure it in the [password manager](https://go.microsoft.com/fwlink/?linkid=2134622) policies.</span></span>
