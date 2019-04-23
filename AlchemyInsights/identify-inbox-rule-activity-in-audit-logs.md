---
title: Identificiranje Primljeno pravilo aktivnost u zapisnika nadzora
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1368
ms.assetid: ''
ms.openlocfilehash: 9339d9c58056f568dc994b75bffe39f2c8bbdd34
ms.sourcegitcommit: ffe2f489b1ac3aae62aa784c959da6a41c3261eb
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/17/2019
ms.locfileid: "31909102"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a><span data-ttu-id="4152d-102">Identificiranje Primljeno pravilo aktivnost u zapisnika nadzora</span><span class="sxs-lookup"><span data-stu-id="4152d-102">Identify inbox rule activity in audit logs</span></span>

<span data-ttu-id="4152d-103">Pretraživanje zapisnika nadzora u & sigurnost usklađenosti centar možete koristiti za prikaz mape Primljeno pravilo događaje (Stvaranje, izmjena i brisanje pravila ulazne pošte).</span><span class="sxs-lookup"><span data-stu-id="4152d-103">You can use audit log search in the Security & Compliance Center to view inbox rule events (creating, modifying, and deleting inbox rules).</span></span>

1. <span data-ttu-id="4152d-104">Prijavite se u sustav [Office 365 sigurnosne & usklađenosti centar](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="4152d-104">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="4152d-105">Kliknite **za pretraživanje i istraživanja** i odaberite **Pretraživanje zapisnika nadzora**.</span><span class="sxs-lookup"><span data-stu-id="4152d-105">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="4152d-106">Odaberite raspon datum u polja **Datum početka** i **Datum završetka** .</span><span class="sxs-lookup"><span data-stu-id="4152d-106">Select the date range in the **Start date** and **End date** fields.</span></span>

4. <span data-ttu-id="4152d-107">Pod **Aktivnosti poštanskog sandučića sustava Exchange**, provjerite je li polje **aktivnosti** postavljeno na **InboxRule novo stvori/Izmijeni/Omogući/Onemogući Primljeno pravilo**.</span><span class="sxs-lookup"><span data-stu-id="4152d-107">Under **Exchange Mailbox Activities**, verify the **Activities** field is set to **New-InboxRule Create/modify/enable/disable inbox rule**.</span></span>

5. <span data-ttu-id="4152d-108">Kliknite **Pretraži**.</span><span class="sxs-lookup"><span data-stu-id="4152d-108">Click **Search**.</span></span>

<span data-ttu-id="4152d-109">U rezultatima, odaberite nadzora zapisa.</span><span class="sxs-lookup"><span data-stu-id="4152d-109">In the results, select an audit record.</span></span> <span data-ttu-id="4152d-110">Potpaleta pojedinosti kliknite **Dodatne informacije**.</span><span class="sxs-lookup"><span data-stu-id="4152d-110">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="4152d-111">Informacije o postavkama pravila ulazne pošte prikazuje se u polju **parametre** .</span><span class="sxs-lookup"><span data-stu-id="4152d-111">Information about the inbox rule settings is displayed in the **Parameters** field.</span></span>

<span data-ttu-id="4152d-112">Za dodatne informacije pogledajte [Determining ako je korisnik stvorio pravilo Primljeno](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span><span class="sxs-lookup"><span data-stu-id="4152d-112">For more information, see [Determining if a user created an inbox rule](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span></span>