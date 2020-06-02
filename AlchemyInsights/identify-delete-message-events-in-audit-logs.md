---
title: Prepoznavanje događaja brisanja poruka u zapisnicima nadzora
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 641c0216491186aeb423a13854c6b39ee005e5df
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508980"
---
# <a name="audit-logs-for-deleted-email-messages"></a><span data-ttu-id="6ff49-102">Zapisnici nadzora za izbrisane poruke e-pošte</span><span class="sxs-lookup"><span data-stu-id="6ff49-102">Audit logs for deleted email messages</span></span>

<span data-ttu-id="6ff49-103">Počevši od siječnja 2019.</span><span class="sxs-lookup"><span data-stu-id="6ff49-103">Starting in January 2019, Microsoft is turning on mailbox audit logging by default.</span></span> <span data-ttu-id="6ff49-104">U suprotnom, da biste pregledali događaje brisanja poruka za određenog korisnika, morate ručno omogućiti akcije brisanja za nadzor.</span><span class="sxs-lookup"><span data-stu-id="6ff49-104">Otherwise, to review delete message events for a specific user, you need to manually enable the delete actions for auditing.</span></span> <span data-ttu-id="6ff49-105">Ako je zapisivanje nadzora poštanskog sandučića već omogućeno za vašu tvrtku ili ustanovu ili za određenog korisnika, slijedite korake u nastavku.</span><span class="sxs-lookup"><span data-stu-id="6ff49-105">If mailbox audit logging is already enabled for your organization or for the specific user, follow the steps below.</span></span>

1. <span data-ttu-id="6ff49-106">Prijavite se u Centar za [usklađenost sa sigurnosnim & sustava Microsoft 365](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="6ff49-106">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="6ff49-107">Kliknite **Pretraživanje i istraživanje** i odaberite Pretraživanje **zapisnika nadzora**.</span><span class="sxs-lookup"><span data-stu-id="6ff49-107">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="6ff49-108">Odaberite datumski raspon u poljima **Datum početka** i **Datum završetka.**</span><span class="sxs-lookup"><span data-stu-id="6ff49-108">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="6ff49-109">Navedite korisničko ime za korisnika koje želite istražiti (korisnika koji je izbrisao stavke).</span><span class="sxs-lookup"><span data-stu-id="6ff49-109">Specify username for the user that you want to investigate (the user who deleted the items).</span></span> <span data-ttu-id="6ff49-110">U polju **Aktivnosti** odaberite **Izbrisane poruke iz mape Izbrisane stavke** i **Premještene poruke u mapu Izbrisane stavke**.</span><span class="sxs-lookup"><span data-stu-id="6ff49-110">In the **Activities** field, select **Deleted messages from Deleted Items folder** and **Moved messages to Deleted Items folder**.</span></span>

4. <span data-ttu-id="6ff49-111">Kliknite **Pretraži**.</span><span class="sxs-lookup"><span data-stu-id="6ff49-111">Click **Search**.</span></span>

<span data-ttu-id="6ff49-112">U rezultatima odaberite zapis nadzora.</span><span class="sxs-lookup"><span data-stu-id="6ff49-112">In the results, select an audit record.</span></span> <span data-ttu-id="6ff49-113">U potpaleti pojedinosti kliknite **Dodatne informacije**.</span><span class="sxs-lookup"><span data-stu-id="6ff49-113">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="6ff49-114">Dodatne informacije o izbrisanoj stavci (na primjer, redak predmeta i mjesto stavke kada je izbrisana) prikazuju se u polju **Zahvaćeneite.**</span><span class="sxs-lookup"><span data-stu-id="6ff49-114">Additional information about the deleted item (for example, the subject line and the location of the item when it was deleted) is displayed in the **AffectedItems** field.</span></span> <span data-ttu-id="6ff49-115">Svojstvo **ClientInfoString** prikazat će se je li brisanje došlo u programu Outlook, Outlook na webu (ranije poznat kao Outlook Web App) ili bilo kojem drugom uređaju.</span><span class="sxs-lookup"><span data-stu-id="6ff49-115">The **ClientInfoString** property will show if the deletion occurred in Outlook, Outlook on the web (formerly known as Outlook Web App), or any other device.</span></span>

<span data-ttu-id="6ff49-116">Dodatne informacije potražite [u odjeljku Određivanje tko je postavio prosljeđivanje e-pošte za poštanski sandučić](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items).</span><span class="sxs-lookup"><span data-stu-id="6ff49-116">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items).</span></span>

<span data-ttu-id="6ff49-117">**Napomena:** izbrisane stavke ne možete dohvatiti pomoću značajke zapisnika nadzora.</span><span class="sxs-lookup"><span data-stu-id="6ff49-117">**Note**: You can't retrieve deleted items using the audit log feature.</span></span> <span data-ttu-id="6ff49-118">Da biste dohvatili izbrisane poruke u programu Outlook na webu, pročitajte članak [Oporavak izbrisanih stavki u web-aplikaciji Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span><span class="sxs-lookup"><span data-stu-id="6ff49-118">To retrieve deleted messages in Outlook on the web, see [Recover deleted items in Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span></span>
