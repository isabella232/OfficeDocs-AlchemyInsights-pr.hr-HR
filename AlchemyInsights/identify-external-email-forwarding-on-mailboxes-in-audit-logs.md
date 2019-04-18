---
title: Identificiranje prosljeđivanje vanjski e-pošte na poštanskim sandučićima u zapisnika nadzora
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1369
ms.assetid: ''
ms.openlocfilehash: 7fb2c161c558a7eb961f86ca2b86e33750d902fd
ms.sourcegitcommit: ffe2f489b1ac3aae62aa784c959da6a41c3261eb
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/17/2019
ms.locfileid: "31909105"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a><span data-ttu-id="273c3-102">Prepoznati prilikom prosljeđivanja e-pošte vanjskog konfiguriran na poštanski sandučići</span><span class="sxs-lookup"><span data-stu-id="273c3-102">Identify when external email forwarding is configured on mailboxes</span></span>

<span data-ttu-id="273c3-103">Kada korisnik konfigurira prosljeđivanje vanjski e-pošte u poštanski sandučić, aktivnost se nadzirati kao dio cmdlet **Set poštanskog sandučića** .</span><span class="sxs-lookup"><span data-stu-id="273c3-103">When a user configures external email forwarding on a mailbox, the activity is audited as part of the **Set-Mailbox** cmdlet.</span></span> <span data-ttu-id="273c3-104">Možete vidjeti aktivnosti pomoću pretraživanje zapisnika nadzora u & usklađenosti centar sigurnosti.</span><span class="sxs-lookup"><span data-stu-id="273c3-104">You can see the activity using audit log search in the Security & Compliance Center.</span></span>

1. <span data-ttu-id="273c3-105">Prijavite se u sustav [Office 365 sigurnosne & usklađenosti centar](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="273c3-105">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="273c3-106">Kliknite **za pretraživanje i istraživanja** i odaberite **Pretraživanje zapisnika nadzora**.</span><span class="sxs-lookup"><span data-stu-id="273c3-106">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="273c3-107">Odaberite raspon datum u polja **Datum početka** i **Datum završetka** .</span><span class="sxs-lookup"><span data-stu-id="273c3-107">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="273c3-108">Ne morate navesti korisničko ime.</span><span class="sxs-lookup"><span data-stu-id="273c3-108">You don't need to specify a username.</span></span> <span data-ttu-id="273c3-109">Provjerite je li polje **aktivnosti** postavljeno na **Pokaži rezultate za sve aktivnosti**.</span><span class="sxs-lookup"><span data-stu-id="273c3-109">Verify the **Activities** field is set to **Show results for all activities**.</span></span>

4. <span data-ttu-id="273c3-110">Kliknite **Pretraži**.</span><span class="sxs-lookup"><span data-stu-id="273c3-110">Click **Search**.</span></span>

<span data-ttu-id="273c3-111">U rezultatima pritisnite **Rezultate filtra** i upišite **Skup poštanskog sandučića** u okvir filtar aktivnost.</span><span class="sxs-lookup"><span data-stu-id="273c3-111">In the results, click **Filter Results** and type **Set-Mailbox** in the activity filter box.</span></span> <span data-ttu-id="273c3-112">Odaberite zapis nadzora u rezultatima.</span><span class="sxs-lookup"><span data-stu-id="273c3-112">Select an audit record in the results.</span></span> <span data-ttu-id="273c3-113">Potpaleta **pojedinosti** pritisnite **Dodatne informacije**.</span><span class="sxs-lookup"><span data-stu-id="273c3-113">In the **Details** flyout, click **More information**.</span></span> <span data-ttu-id="273c3-114">Imate pogledajte detalje svakog nadzora zapisa da biste ustanovili Ako aktivnost odnosi prosljeđivanja e-pošte.</span><span class="sxs-lookup"><span data-stu-id="273c3-114">You have to look at the details of each audit record to determine if the activity is related to email forwarding.</span></span>

- <span data-ttu-id="273c3-115">**ID objekta**: vrijednost pseudonim poštanskog sandučića koja je izmijenjena.</span><span class="sxs-lookup"><span data-stu-id="273c3-115">**ObjectId**: The alias value of the mailbox that was modified.</span></span>

- <span data-ttu-id="273c3-116">**Parametri**: _ForwardingSmtpAddress_ označava adresu e-pošte za cilj.</span><span class="sxs-lookup"><span data-stu-id="273c3-116">**Parameters**: _ForwardingSmtpAddress_ indicates the target email address.</span></span>

- <span data-ttu-id="273c3-117">**Korisnički ID**: korisnika koji je konfiguriran prosljeđivanja e-pošte na poštanskog sandučića u polju **ID objekta** .</span><span class="sxs-lookup"><span data-stu-id="273c3-117">**UserId**: The user who configured email forwarding on the mailbox in the **ObjectId** field.</span></span>

<span data-ttu-id="273c3-118">Za dodatne informacije pogledajte [Determining tko postaviti poštanski sandučić za prosljeđivanje e-pošte](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).</span><span class="sxs-lookup"><span data-stu-id="273c3-118">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).</span></span>
