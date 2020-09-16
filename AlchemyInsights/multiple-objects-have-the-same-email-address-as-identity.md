---
title: Više objekata ima istu adresu e-pošte kao identitet
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1834"
- "9000247"
ms.openlocfilehash: 05fb43133bc68b71ccdbab44d28679a1f659e762
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47724607"
---
# <a name="multiple-objects-have-the-same-email-address-as-identity"></a><span data-ttu-id="49994-102">Više objekata ima istu adresu e-pošte kao identitet</span><span class="sxs-lookup"><span data-stu-id="49994-102">Multiple objects have the same email address as identity</span></span>

<span data-ttu-id="49994-103">**Više objekata**</span><span class="sxs-lookup"><span data-stu-id="49994-103">**Multiple objects**</span></span>

<span data-ttu-id="49994-104">Jedan od običnih razloga te pogreške ne može pravilno usmjeravati zahtjev za Outlook Web Access u prisustvu više objekata koji imaju istu adresu e-pošte kao identitet.</span><span class="sxs-lookup"><span data-stu-id="49994-104">One of the common reasons of this error is not being able to route an Outlook Web Access request properly in a presence of multiple objects having the same email address as identity.</span></span> <span data-ttu-id="49994-105">Da biste pronašli ove objekte, pokrenite sljedeće naredbe:</span><span class="sxs-lookup"><span data-stu-id="49994-105">To find these objects, run the following commands:</span></span>

<span data-ttu-id="49994-106">· Dohvaćanje primatelja <email address></span><span class="sxs-lookup"><span data-stu-id="49994-106">· Get-Recipient <email address></span></span>

<span data-ttu-id="49994-107">· Dohvaćanje korisnika <email address></span><span class="sxs-lookup"><span data-stu-id="49994-107">· Get-User <email address></span></span>

<span data-ttu-id="49994-108">· Nabavite-user <email address> -softdeleteduser</span><span class="sxs-lookup"><span data-stu-id="49994-108">· Get-User <email address> -SoftDeletedUser</span></span>

<span data-ttu-id="49994-109">· Dohvaćanje kontakta <email address></span><span class="sxs-lookup"><span data-stu-id="49994-109">· Get-Contact <email address></span></span>

<span data-ttu-id="49994-110">· Nabavite-Mailbox <email address> -publifolder</span><span class="sxs-lookup"><span data-stu-id="49994-110">· Get-Mailbox <email address> -PublicFolder</span></span>

<span data-ttu-id="49994-111">· Nabavite-Mailbox <email address> – includesoftdeletedmailbox</span><span class="sxs-lookup"><span data-stu-id="49994-111">· Get-Mailbox <email address> -IncludeSoftDeletedMailbox</span></span>

<span data-ttu-id="49994-112">· Dohvaćanje poštanskog sandučića <email address> -inactivemailboxonly</span><span class="sxs-lookup"><span data-stu-id="49994-112">· Get-Mailbox <email address> -InactiveMailboxOnly</span></span>

<span data-ttu-id="49994-113">Da biste riješili problem, uklonite više objekata s istim identitetom e-pošte i provjerite postoji li jedan objekt s određenim identitetom e-pošte te je li njegova vrsta primatelja UserMailbox.</span><span class="sxs-lookup"><span data-stu-id="49994-113">To resolve the issue, remove multiple objects with the same email identity and make sure that there is a single object with the specific email identity and that its recipient type is UserMailbox.</span></span>

<span data-ttu-id="49994-114">**Ista adresa koristi se za poštanske sandučiće tvrtke i potrošača**</span><span class="sxs-lookup"><span data-stu-id="49994-114">**Same address is used for business and consumer mailboxes**</span></span>

<span data-ttu-id="49994-115">Drugi je uzrok kada se ista adresa koristi za poslovne i potrošačke poštanske sandučiće.</span><span class="sxs-lookup"><span data-stu-id="49994-115">Another cause is when the same address is used for business and consumer mailboxes.</span></span> <span data-ttu-id="49994-116">U ovom slučaju korisnik mora promijeniti pseudonim primarnog potrošača dok Cafe ne podržava ovaj scenarij.</span><span class="sxs-lookup"><span data-stu-id="49994-116">In this case, the user must change their primary consumer alias until Cafe supports this scenario.</span></span> <span data-ttu-id="49994-117">To je trajna pogreška koja ne nestaje bez intervencije.</span><span class="sxs-lookup"><span data-stu-id="49994-117">This is a permanent error that does not go away without intervention.</span></span>

<span data-ttu-id="49994-118">Pojedinosti potražite u članku [Promjena adrese e-pošte ili telefonskog broja za Microsoftov račun](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account).</span><span class="sxs-lookup"><span data-stu-id="49994-118">For details, see [Change the email address or phone number for your Microsoft account](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account).</span></span>