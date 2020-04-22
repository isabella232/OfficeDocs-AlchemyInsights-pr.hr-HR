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
ms.openlocfilehash: 797a4b1146862faf91d2b9e8d74feade90f71650
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716488"
---
# <a name="audit-logs-for-deleted-email-messages"></a><span data-ttu-id="3694c-102">Nadzor zapisnika za izbrisane poruke e-pošte</span><span class="sxs-lookup"><span data-stu-id="3694c-102">Audit logs for deleted email messages</span></span>

<span data-ttu-id="3694c-103">Počevši od siječnja 2019, Microsoft po zadanom uključuje zapisivanje nadzora poštanskog sandučića.</span><span class="sxs-lookup"><span data-stu-id="3694c-103">Starting in January 2019, Microsoft is turning on mailbox audit logging by default.</span></span> <span data-ttu-id="3694c-104">U suprotnom, da biste pregledali događaje brisanja poruka za određenog korisnika, morate ručno omogućiti akcije brisanja za nadzor.</span><span class="sxs-lookup"><span data-stu-id="3694c-104">Otherwise, to review delete message events for a specific user, you need to manually enable the delete actions for auditing.</span></span> <span data-ttu-id="3694c-105">Ako je zapisivanje nadzora poštanskog sandučića već omogućeno za vašu tvrtku ili ustanovu ili za određenog korisnika, slijedite korake u nastavku.</span><span class="sxs-lookup"><span data-stu-id="3694c-105">If mailbox audit logging is already enabled for your organization or for the specific user, follow the steps below.</span></span>

1. <span data-ttu-id="3694c-106">Prijava u Centar za [& sigurnosti sustava Microsoft 365](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="3694c-106">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="3694c-107">Kliknite **Pretraživanje i istraživanje** i odaberite Pretraživanje **zapisnika nadzora**.</span><span class="sxs-lookup"><span data-stu-id="3694c-107">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="3694c-108">Odaberite datumski raspon u poljima **Datum početka** i **Datum završetka.**</span><span class="sxs-lookup"><span data-stu-id="3694c-108">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="3694c-109">Navedite korisničko ime za korisnika kojeg želite istražiti (korisnika koji je izbrisao stavke).</span><span class="sxs-lookup"><span data-stu-id="3694c-109">Specify username for the user that you want to investigate (the user who deleted the items).</span></span> <span data-ttu-id="3694c-110">U polju **Aktivnosti** odaberite **Izbrisane poruke iz mape Izbrisane stavke** i **Premještene poruke u mapu Izbrisane stavke**.</span><span class="sxs-lookup"><span data-stu-id="3694c-110">In the **Activities** field, select **Deleted messages from Deleted Items folder** and **Moved messages to Deleted Items folder**.</span></span>

4. <span data-ttu-id="3694c-111">Kliknite **Pretraživanje**.</span><span class="sxs-lookup"><span data-stu-id="3694c-111">Click **Search**.</span></span>

<span data-ttu-id="3694c-112">U rezultatima odaberite zapis nadzora.</span><span class="sxs-lookup"><span data-stu-id="3694c-112">In the results, select an audit record.</span></span> <span data-ttu-id="3694c-113">U potpaleti pojedinosti kliknite **Dodatne informacije**.</span><span class="sxs-lookup"><span data-stu-id="3694c-113">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="3694c-114">Dodatne informacije o izbrisanoj stavci (na primjer, retku predmeta i mjestu artikla prilikom brisanja) prikazuju se u polju **ZahvaćeniArtikli.**</span><span class="sxs-lookup"><span data-stu-id="3694c-114">Additional information about the deleted item (for example, the subject line and the location of the item when it was deleted) is displayed in the **AffectedItems** field.</span></span> <span data-ttu-id="3694c-115">Svojstvo **ClientInfoString** prikazat će se je li došlo do brisanja u programu Outlook, programu Outlook na webu (ranije poznatom kao Outlook Web App) ili bilo kojem drugom uređaju.</span><span class="sxs-lookup"><span data-stu-id="3694c-115">The **ClientInfoString** property will show if the deletion occurred in Outlook, Outlook on the web (formerly known as Outlook Web App), or any other device.</span></span>

<span data-ttu-id="3694c-116">Dodatne informacije potražite u [odjeljku Određivanje tko je postavio prosljeđivanje e-pošte za poštanski sandučić](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items).</span><span class="sxs-lookup"><span data-stu-id="3694c-116">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items).</span></span>

<span data-ttu-id="3694c-117">**Napomena:** Izbrisane stavke ne možete dohvatiti pomoću značajke zapisnika nadzora.</span><span class="sxs-lookup"><span data-stu-id="3694c-117">**Note**: You can't retrieve deleted items using the audit log feature.</span></span> <span data-ttu-id="3694c-118">Da biste dohvatili izbrisane poruke u programu Outlook na webu, [pročitajte članak Oporavak izbrisanih stavki u web-aplikaciji Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span><span class="sxs-lookup"><span data-stu-id="3694c-118">To retrieve deleted messages in Outlook on the web, see [Recover deleted items in Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span></span>
