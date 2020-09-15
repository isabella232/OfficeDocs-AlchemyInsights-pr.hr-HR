---
title: Prepoznavanje vanjskih prosljeđivanja e-pošte u poštanskom sandučiću u evidenciji nadzora
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: d06ef83adcae1342173a6fe75f79525c7e1797ce
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696289"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a><span data-ttu-id="13c1e-102">Određivanje kada je vanjsko prosljeđivanje e-pošte konfigurirano na poštanskim sandučićima</span><span class="sxs-lookup"><span data-stu-id="13c1e-102">Identify when external email forwarding is configured on mailboxes</span></span>

<span data-ttu-id="13c1e-103">Kada korisnik Microsoft 365 u poštanskom sandučiću konfigurira vanjsku prosljeđivanje e-pošte, aktivnost se nadzire kao dio cmdleta **Set-Mailbox** .</span><span class="sxs-lookup"><span data-stu-id="13c1e-103">When a Microsoft 365 user configures external email forwarding on a mailbox, the activity is audited as part of the **Set-Mailbox** cmdlet.</span></span> <span data-ttu-id="13c1e-104">Aktivnost možete vidjeti pomoću pretraživanja zapisnika nadzora u centru za sigurnost & usklađenosti.</span><span class="sxs-lookup"><span data-stu-id="13c1e-104">You can see the activity using audit log search in the Security & Compliance Center.</span></span>

1. <span data-ttu-id="13c1e-105">Prijavite se u [centar za sigurnost & sustava Microsoft 365](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="13c1e-105">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="13c1e-106">Idite na stranicu **Search**  >  **pretraživanja zapisnika nadzora** pretraživanja.</span><span class="sxs-lookup"><span data-stu-id="13c1e-106">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="13c1e-107">Odaberite raspon datuma u poljima **Datum početka** i **Datum završetka** .</span><span class="sxs-lookup"><span data-stu-id="13c1e-107">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="13c1e-108">Ne morate navesti korisničko ime.</span><span class="sxs-lookup"><span data-stu-id="13c1e-108">You don't need to specify a username.</span></span> <span data-ttu-id="13c1e-109">Provjerite je li polje **aktivnosti** postavljeno **tako da pokazuje rezultate za sve aktivnosti**.</span><span class="sxs-lookup"><span data-stu-id="13c1e-109">Verify the **Activities** field is set to **Show results for all activities**.</span></span>

4. <span data-ttu-id="13c1e-110">Kliknite **Pretraživanje**.</span><span class="sxs-lookup"><span data-stu-id="13c1e-110">Click **Search**.</span></span>

<span data-ttu-id="13c1e-111">U rezultatima kliknite **Filtriraj rezultate** , a zatim u okvir Filtar aktivnosti upišite **skup poštanskih sandučića** .</span><span class="sxs-lookup"><span data-stu-id="13c1e-111">In the results, click **Filter Results** and type **Set-Mailbox** in the activity filter box.</span></span> <span data-ttu-id="13c1e-112">Odaberite zapis nadzora u rezultatima.</span><span class="sxs-lookup"><span data-stu-id="13c1e-112">Select an audit record in the results.</span></span> <span data-ttu-id="13c1e-113">U nastavku **Pojedinosti** kliknite **više informacija**.</span><span class="sxs-lookup"><span data-stu-id="13c1e-113">In the **Details** flyout, click **More information**.</span></span> <span data-ttu-id="13c1e-114">Da biste utvrdili je li aktivnost povezana s prosljeđivanjem e-pošte, morate pogledati pojedinosti o svakom zapisu nadzora.</span><span class="sxs-lookup"><span data-stu-id="13c1e-114">You have to look at the details of each audit record to determine if the activity is related to email forwarding.</span></span>

- <span data-ttu-id="13c1e-115">**Objektand**: vrijednost pseudonima poštanskog sandučića koji je promijenjen.</span><span class="sxs-lookup"><span data-stu-id="13c1e-115">**ObjectId**: The alias value of the mailbox that was modified.</span></span>

- <span data-ttu-id="13c1e-116">**Parametri**: _forwardingsmtpaddress_ označava ciljnu adresu e-pošte.</span><span class="sxs-lookup"><span data-stu-id="13c1e-116">**Parameters**: _ForwardingSmtpAddress_ indicates the target email address.</span></span>

- <span data-ttu-id="13c1e-117">**Userid**: korisnik koji je konfigurirao prosljeđivanje e-pošte na poštanskom sandučiću u polju **Objekt** .</span><span class="sxs-lookup"><span data-stu-id="13c1e-117">**UserId**: The user who configured email forwarding on the mailbox in the **ObjectId** field.</span></span>

<span data-ttu-id="13c1e-118">Dodatne informacije potražite u članku [određivanje tko je postavio prosljeđivanje e-pošte za poštanski sandučić](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).</span><span class="sxs-lookup"><span data-stu-id="13c1e-118">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).</span></span>
