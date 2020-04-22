---
title: Prepoznavanje vanjskog prosljeđivanja e-pošte na poštanskim sandučićima u nadzornim zapisnicima
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 156fd0044cdc42230ace0a5db16f49af572bb6fa
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716452"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a><span data-ttu-id="307b1-102">Prepoznavanje kada je vanjsko prosljeđivanje e-pošte konfigurirano na poštanskim sandučićima</span><span class="sxs-lookup"><span data-stu-id="307b1-102">Identify when external email forwarding is configured on mailboxes</span></span>

<span data-ttu-id="307b1-103">Kada korisnik sustava Microsoft 365 konfigurira prosljeđivanje vanjske e-pošte na poštanskom sandučiću, aktivnost se nadzire kao dio cmdleta **Set-Mailbox.**</span><span class="sxs-lookup"><span data-stu-id="307b1-103">When a Microsoft 365 user configures external email forwarding on a mailbox, the activity is audited as part of the **Set-Mailbox** cmdlet.</span></span> <span data-ttu-id="307b1-104">Aktivnost možete vidjeti pomoću pretraživanja zapisnika nadzora u centru za & sigurnosti.</span><span class="sxs-lookup"><span data-stu-id="307b1-104">You can see the activity using audit log search in the Security & Compliance Center.</span></span>

1. <span data-ttu-id="307b1-105">Prijavite se u Centar za [sigurnost sustava Microsoft 365 & .](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="307b1-105">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="307b1-106">Idite na stranicu **za** > **pretraživanje zapisnika nadzora** pretraživanja.</span><span class="sxs-lookup"><span data-stu-id="307b1-106">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="307b1-107">Odaberite datumski raspon u poljima **Datum početka** i **Datum završetka.**</span><span class="sxs-lookup"><span data-stu-id="307b1-107">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="307b1-108">Ne morate navesti korisničko ime.</span><span class="sxs-lookup"><span data-stu-id="307b1-108">You don't need to specify a username.</span></span> <span data-ttu-id="307b1-109">Provjerite je li polje **Aktivnosti** postavljeno na **Prikaži rezultate za sve aktivnosti**.</span><span class="sxs-lookup"><span data-stu-id="307b1-109">Verify the **Activities** field is set to **Show results for all activities**.</span></span>

4. <span data-ttu-id="307b1-110">Kliknite **Pretraživanje**.</span><span class="sxs-lookup"><span data-stu-id="307b1-110">Click **Search**.</span></span>

<span data-ttu-id="307b1-111">U rezultatima kliknite **Filtriraj rezultate** i u okvir filtra aktivnosti upišite Postavi **poštanski sandučić.**</span><span class="sxs-lookup"><span data-stu-id="307b1-111">In the results, click **Filter Results** and type **Set-Mailbox** in the activity filter box.</span></span> <span data-ttu-id="307b1-112">Odaberite zapis nadzora u rezultatima.</span><span class="sxs-lookup"><span data-stu-id="307b1-112">Select an audit record in the results.</span></span> <span data-ttu-id="307b1-113">U potpaleti **Detalji** kliknite **Dodatne informacije**.</span><span class="sxs-lookup"><span data-stu-id="307b1-113">In the **Details** flyout, click **More information**.</span></span> <span data-ttu-id="307b1-114">Morate pogledati pojedinosti svakog zapisa nadzora da biste utvrdili je li aktivnost povezana s prosljeđivanjem e-pošte.</span><span class="sxs-lookup"><span data-stu-id="307b1-114">You have to look at the details of each audit record to determine if the activity is related to email forwarding.</span></span>

- <span data-ttu-id="307b1-115">**ObjectId**: Vrijednost pseudonima izmijenjenog poštanskog sandučića.</span><span class="sxs-lookup"><span data-stu-id="307b1-115">**ObjectId**: The alias value of the mailbox that was modified.</span></span>

- <span data-ttu-id="307b1-116">**Parametri**: _ForwardingSmtpAddress_ označava ciljnu adresu e-pošte.</span><span class="sxs-lookup"><span data-stu-id="307b1-116">**Parameters**: _ForwardingSmtpAddress_ indicates the target email address.</span></span>

- <span data-ttu-id="307b1-117">**UserId**: Korisnik koji je konfigurirao prosljeđivanje e-pošte na poštanskom sandučiću u polju **ObjectId.**</span><span class="sxs-lookup"><span data-stu-id="307b1-117">**UserId**: The user who configured email forwarding on the mailbox in the **ObjectId** field.</span></span>

<span data-ttu-id="307b1-118">Dodatne informacije potražite u [odjeljku Određivanje tko je postavio prosljeđivanje e-pošte za poštanski sandučić](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).</span><span class="sxs-lookup"><span data-stu-id="307b1-118">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).</span></span>
