---
title: Utvrđivanje aktivnosti pravila ulazne pošte u zapisnicima nadzora
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: f946510539b3d28f2ceeec1546cbffce8bd352fd
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716416"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a><span data-ttu-id="2eb98-102">Utvrđivanje aktivnosti pravila ulazne pošte u zapisnicima nadzora</span><span class="sxs-lookup"><span data-stu-id="2eb98-102">Identify inbox rule activity in audit logs</span></span>

<span data-ttu-id="2eb98-103">Pretraživanje zapisnika nadzora u centru za sigurnost sustava Microsoft 365 & usklađenosti možete koristiti za prikaz događaja pravila ulazne pošte (stvaranje, izmjena i brisanje pravila ulazne pošte).</span><span class="sxs-lookup"><span data-stu-id="2eb98-103">You can use audit log search in the Microsoft 365 Security & Compliance Center to view inbox rule events (creating, modifying, and deleting inbox rules).</span></span>

1. <span data-ttu-id="2eb98-104">Prijavite se u Centar za [sigurnost sustava Microsoft 365 & .](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="2eb98-104">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="2eb98-105">Idite na stranicu **za** > **pretraživanje zapisnika nadzora** pretraživanja.</span><span class="sxs-lookup"><span data-stu-id="2eb98-105">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="2eb98-106">Odaberite datumski raspon u poljima **Datum početka** i **Datum završetka.**</span><span class="sxs-lookup"><span data-stu-id="2eb98-106">Select the date range in the **Start date** and **End date** fields.</span></span>

4. <span data-ttu-id="2eb98-107">U odjeljku **Aktivnosti poštanskog sandučića sustava Exchange**provjerite je li polje **Aktivnosti** postavljeno na **Novo- InboxRule Stvaranje/ izmjena/omogućivanje/onemogućivanje pravila ulazne pošte**.</span><span class="sxs-lookup"><span data-stu-id="2eb98-107">Under **Exchange Mailbox Activities**, verify the **Activities** field is set to **New-InboxRule Create/modify/enable/disable inbox rule**.</span></span>

5. <span data-ttu-id="2eb98-108">Kliknite **Pretraživanje**.</span><span class="sxs-lookup"><span data-stu-id="2eb98-108">Click **Search**.</span></span>

<span data-ttu-id="2eb98-109">U rezultatima odaberite zapis nadzora.</span><span class="sxs-lookup"><span data-stu-id="2eb98-109">In the results, select an audit record.</span></span> <span data-ttu-id="2eb98-110">U potpaleti pojedinosti kliknite **Dodatne informacije**.</span><span class="sxs-lookup"><span data-stu-id="2eb98-110">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="2eb98-111">Informacije o postavkama pravila ulazne pošte prikazuju se u polju **Parametri.**</span><span class="sxs-lookup"><span data-stu-id="2eb98-111">Information about the inbox rule settings is displayed in the **Parameters** field.</span></span>

<span data-ttu-id="2eb98-112">Dodatne informacije potražite u [odjeljku Određivanje je li korisnik stvorio pravilo ulazne pošte](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span><span class="sxs-lookup"><span data-stu-id="2eb98-112">For more information, see [Determining if a user created an inbox rule](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span></span>
