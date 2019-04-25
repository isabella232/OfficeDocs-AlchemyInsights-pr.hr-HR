---
title: Odredite Brisanje poruke događaja u zapisnika nadzora
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1370
ms.assetid: ''
ms.openlocfilehash: 93f8a192af6e689e2b2d04013f35b8da2b69e607
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32416702"
---
# <a name="audit-logs-for-deleted-email-messages"></a><span data-ttu-id="5038f-102">Evidencija nadzora za poruke e-pošte izbrisane</span><span class="sxs-lookup"><span data-stu-id="5038f-102">Audit logs for deleted email messages</span></span>

<span data-ttu-id="5038f-103">Početni 2019 siječanj, Microsoft je uključivanje zapisivanja po zadanom nadzor poštanskog sandučića.</span><span class="sxs-lookup"><span data-stu-id="5038f-103">Starting in January 2019, Microsoft is turning on mailbox audit logging by default.</span></span> <span data-ttu-id="5038f-104">U suprotnom, za pregled brisanje poruka događaje za određenog korisnika, morate ručno omogućiti brisanje akcije za nadzor.</span><span class="sxs-lookup"><span data-stu-id="5038f-104">Otherwise, to review delete message events for a specific user, you need to manually enable the delete actions for auditing.</span></span> <span data-ttu-id="5038f-105">Nadzor poštanskog sandučića zapisivanje već omogućeno za organizaciju ili za određenog korisnika, slijedite dolje navedene korake.</span><span class="sxs-lookup"><span data-stu-id="5038f-105">If mailbox audit logging is already enabled for your organization or for the specific user, follow the steps below.</span></span>

1. <span data-ttu-id="5038f-106">Prijavite se u sustav [Office 365 sigurnosne & usklađenosti centar](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="5038f-106">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="5038f-107">Kliknite **za pretraživanje i istraživanja** i odaberite **Pretraživanje zapisnika nadzora**.</span><span class="sxs-lookup"><span data-stu-id="5038f-107">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="5038f-108">Odaberite raspon datum u polja **Datum početka** i **Datum završetka** .</span><span class="sxs-lookup"><span data-stu-id="5038f-108">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="5038f-109">Navedite korisničko ime korisnika koji želite istražiti (korisnik koji izbrisane stavke).</span><span class="sxs-lookup"><span data-stu-id="5038f-109">Specify username for the user that you want to investigate (the user who deleted the items).</span></span> <span data-ttu-id="5038f-110">U polju **aktivnosti** odaberite **Izbrisane poruke iz mape Izbrisane stavke** i **Moved poruke u mapu Izbrisane stavke**.</span><span class="sxs-lookup"><span data-stu-id="5038f-110">In the **Activities** field, select **Deleted messages from Deleted Items folder** and **Moved messages to Deleted Items folder**.</span></span>

4. <span data-ttu-id="5038f-111">Kliknite **Pretraži**.</span><span class="sxs-lookup"><span data-stu-id="5038f-111">Click **Search**.</span></span>

<span data-ttu-id="5038f-112">U rezultatima, odaberite nadzora zapisa.</span><span class="sxs-lookup"><span data-stu-id="5038f-112">In the results, select an audit record.</span></span> <span data-ttu-id="5038f-113">Potpaleta pojedinosti kliknite **Dodatne informacije**.</span><span class="sxs-lookup"><span data-stu-id="5038f-113">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="5038f-114">Dodatne informacije o izbrisana stavka (na primjer, redak predmeta i mjesto artikla kada je izbrisana) prikazuje se u polju **AffectedItems** .</span><span class="sxs-lookup"><span data-stu-id="5038f-114">Additional information about the deleted item (for example, the subject line and the location of the item when it was deleted) is displayed in the **AffectedItems** field.</span></span> <span data-ttu-id="5038f-115">Svojstvo **ClientInfoString** će prikazati ako brisanja došlo je do u programu Outlook, Outlook na webu (nekadašnjeg naziva Outlook Web App) ili drugi uređaj.</span><span class="sxs-lookup"><span data-stu-id="5038f-115">The **ClientInfoString** property will show if the deletion occurred in Outlook, Outlook on the web (formerly known as Outlook Web App), or any other device.</span></span>

<span data-ttu-id="5038f-116">Za dodatne informacije pogledajte [Determining tko postaviti poštanski sandučić za prosljeđivanje e-pošte](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items).</span><span class="sxs-lookup"><span data-stu-id="5038f-116">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items).</span></span>

<span data-ttu-id="5038f-117">**Napomena**: nije moguće dohvatiti izbrisane stavke pomoću značajke zapisnika nadzora.</span><span class="sxs-lookup"><span data-stu-id="5038f-117">**Note**: You can't retrieve deleted items using the audit log feature.</span></span> <span data-ttu-id="5038f-118">Dohvatiti izbrisane poruke u programu Outlook na webu potražite [Oporavi izbrisane stavke u Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span><span class="sxs-lookup"><span data-stu-id="5038f-118">To retrieve deleted messages in Outlook on the web, see [Recover deleted items in Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span></span>
