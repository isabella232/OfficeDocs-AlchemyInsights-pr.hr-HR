---
title: Omogućivanje provjere autentičnosti i otklanjanja poteškoća s SMTP-om
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "5652"
ms.openlocfilehash: 4695a2f111823739c4d87fa2b262a5e64e080955
ms.sourcegitcommit: 2103d706492ad7ee9596344714c0520569ebd6af
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/23/2021
ms.locfileid: "53077643"
---
# <a name="enable-smtp-authentication-and-troubleshooting"></a><span data-ttu-id="54362-102">Omogućivanje provjere autentičnosti i otklanjanja poteškoća s SMTP-om</span><span class="sxs-lookup"><span data-stu-id="54362-102">Enable SMTP authentication and troubleshooting</span></span>

<span data-ttu-id="54362-103">Ako želite omogućiti SMTP provjeru autentičnosti za poštanski sandučić ili vam se prikazuje pogreška "Klijent nije provjeren", "Provjera autentičnosti nije uspješna" ili pogreška "SmtpClientAuthentication" s kodom 5.7.57 ili 5.7.3 ili 5.7.139 kada pokušate prenijeti e-poštu provjerom autentičnosti uređaja ili aplikacije pomoću programa Microsoft 365, izvršite sljedeće tri radnje da biste riješili problem:</span><span class="sxs-lookup"><span data-stu-id="54362-103">If you want to enable SMTP authentication for a mailbox or you're getting a "Client not authenticated", "Authentication unsuccessful", or "SmtpClientAuthentication" error with code 5.7.57 or 5.7.3 or 5.7.139 when you try to relay email by authenticating a device or application with Microsoft 365, perform these three actions to resolve the issue:</span></span>

1. <span data-ttu-id="54362-104">Onemogućivanje [sigurnosnih zadanih postavki](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) za Azure tako da sigurnosne zadane **postavke omogućite** na **Ne**.</span><span class="sxs-lookup"><span data-stu-id="54362-104">Disable the [Azure security defaults](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) by toggling **Enable security defaults** to **No**.</span></span>

    <span data-ttu-id="54362-105">a.</span><span class="sxs-lookup"><span data-stu-id="54362-105">a.</span></span> <span data-ttu-id="54362-106">Prijavite se na portal Azure kao administrator sigurnosti, administrator uvjetnog pristupa ili globalni administrator.</span><span class="sxs-lookup"><span data-stu-id="54362-106">Sign in to the Azure portal as a Security administrator, Conditional Access administrator, or global administrator.</span></span><BR/>
    <span data-ttu-id="54362-107">b.</span><span class="sxs-lookup"><span data-stu-id="54362-107">b.</span></span> <span data-ttu-id="54362-108">Idite na Azure Active Directory > **Svojstva**.</span><span class="sxs-lookup"><span data-stu-id="54362-108">Browse to Azure Active Directory > **Properties**.</span></span><BR/>
    <span data-ttu-id="54362-109">c.</span><span class="sxs-lookup"><span data-stu-id="54362-109">c.</span></span> <span data-ttu-id="54362-110">Odaberite **Upravljanje sigurnosnim zadanim postavkama**.</span><span class="sxs-lookup"><span data-stu-id="54362-110">Select **Manage security defaults**.</span></span><BR/>
    <span data-ttu-id="54362-111">d.</span><span class="sxs-lookup"><span data-stu-id="54362-111">d.</span></span> <span data-ttu-id="54362-112">Postavite **Omogući zadane sigurnosne postavke** na **Ne**.</span><span class="sxs-lookup"><span data-stu-id="54362-112">Set **Enable security defaults** to **No**.</span></span><BR/>
    <span data-ttu-id="54362-113">e.</span><span class="sxs-lookup"><span data-stu-id="54362-113">e.</span></span> <span data-ttu-id="54362-114">Odaberite **Spremi**.</span><span class="sxs-lookup"><span data-stu-id="54362-114">Select **Save**.</span></span>

2. <span data-ttu-id="54362-115">[Omogućivanje slanja klijentskog SMTP-a](/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission#enable-smtp-auth-for-specific-mailboxes) u licenciranom poštanskom sandučiću.</span><span class="sxs-lookup"><span data-stu-id="54362-115">[Enable Client SMTP submission](/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission#enable-smtp-auth-for-specific-mailboxes) on the licensed mailbox.</span></span>

    <span data-ttu-id="54362-116">a.</span><span class="sxs-lookup"><span data-stu-id="54362-116">a.</span></span> <span data-ttu-id="54362-117">Na Centar za administratore okruženja Microsoft 365 odaberite Aktivni **korisnici** pa odaberite korisnika.</span><span class="sxs-lookup"><span data-stu-id="54362-117">From the Microsoft 365 admin center, go to **Active Users**, and select the user.</span></span><BR/>
    <span data-ttu-id="54362-118">b.</span><span class="sxs-lookup"><span data-stu-id="54362-118">b.</span></span> <span data-ttu-id="54362-119">Idite na karticu Pošta pa u odjeljku **Aplikacije za e-poštu** odaberite **Upravljanje aplikacijama za e-poštu**.</span><span class="sxs-lookup"><span data-stu-id="54362-119">Go to Mail tab, and under **Email apps**, select **Manage email apps**.</span></span><BR/>
    <span data-ttu-id="54362-120">d.</span><span class="sxs-lookup"><span data-stu-id="54362-120">d.</span></span> <span data-ttu-id="54362-121">Provjerite je **li potvrđena provjera autentičnosti SMTP-a** (omogućeno).</span><span class="sxs-lookup"><span data-stu-id="54362-121">Make sure **Authenticated SMTP** is checked (enabled).</span></span><BR/>
    <span data-ttu-id="54362-122">e.</span><span class="sxs-lookup"><span data-stu-id="54362-122">e.</span></span> <span data-ttu-id="54362-123">Odaberite **Spremi promjene**.</span><span class="sxs-lookup"><span data-stu-id="54362-123">Select **Save changes**.</span></span><BR/>

3. <span data-ttu-id="54362-124">[Onemogućivanje višestruke provjere autentičnosti (MFA)](/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication#turn-off-legacy-per-user-mfa) u licenciranom poštanskom sandučiću.</span><span class="sxs-lookup"><span data-stu-id="54362-124">[Disable Multi-Factor Authentication (MFA)](/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication#turn-off-legacy-per-user-mfa) on the licensed mailbox.</span></span>

    <span data-ttu-id="54362-125">a.</span><span class="sxs-lookup"><span data-stu-id="54362-125">a.</span></span> <span data-ttu-id="54362-126">Idite na Centar za administratore okruženja Microsoft 365, a zatim na lijevom navigacijskom izborniku **odaberite Korisnici**  >  **Aktivni korisnici**.</span><span class="sxs-lookup"><span data-stu-id="54362-126">Go to the Microsoft 365 admin center, and in the left navigation menu select **Users** > **Active users**.</span></span><BR/>
    <span data-ttu-id="54362-127">b.</span><span class="sxs-lookup"><span data-stu-id="54362-127">b.</span></span> <span data-ttu-id="54362-128">Odaberite **Višestruka provjera autentičnosti**.</span><span class="sxs-lookup"><span data-stu-id="54362-128">Select **Multi-factor authentication**.</span></span><BR/>
    <span data-ttu-id="54362-129">c.</span><span class="sxs-lookup"><span data-stu-id="54362-129">c.</span></span> <span data-ttu-id="54362-130">Odaberite korisnika i **onemogućite višestruku provjeru**.</span><span class="sxs-lookup"><span data-stu-id="54362-130">Select the user and disable **Multi-Factor auth**.</span></span><BR/>
