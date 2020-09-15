---
title: Prepoznavanje događaja za brisanje poruka u evidenciji nadzora
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
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: bc78076706aee15a3133c4b1a89064591f790b58
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696505"
---
# <a name="audit-logs-for-deleted-email-messages"></a><span data-ttu-id="d3f0b-102">Zapisnici nadzora za izbrisane poruke e-pošte</span><span class="sxs-lookup"><span data-stu-id="d3f0b-102">Audit logs for deleted email messages</span></span>

<span data-ttu-id="d3f0b-103">Počevši od siječnja 2019, Microsoft će po zadanom uključiti evidentiranje nadzora poštanskih sandučića.</span><span class="sxs-lookup"><span data-stu-id="d3f0b-103">Starting in January 2019, Microsoft is turning on mailbox audit logging by default.</span></span> <span data-ttu-id="d3f0b-104">U suprotnom, da biste pregledali brisanje događaja poruke za određenog korisnika, morate ručno omogućiti postupke brisanja za nadzor.</span><span class="sxs-lookup"><span data-stu-id="d3f0b-104">Otherwise, to review delete message events for a specific user, you need to manually enable the delete actions for auditing.</span></span> <span data-ttu-id="d3f0b-105">Ako je zapisivanje nadzornog sandučića već omogućeno za vašu tvrtku ili ustanovu ili za određenog korisnika, slijedite upute u nastavku.</span><span class="sxs-lookup"><span data-stu-id="d3f0b-105">If mailbox audit logging is already enabled for your organization or for the specific user, follow the steps below.</span></span>

1. <span data-ttu-id="d3f0b-106">Prijavite se u [centar za sigurnost & sustava Microsoft 365](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="d3f0b-106">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="d3f0b-107">Kliknite **pretraživanje i istraživanje** te odaberite **pretraživanje zapisnika nadzora**.</span><span class="sxs-lookup"><span data-stu-id="d3f0b-107">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="d3f0b-108">Odaberite raspon datuma u poljima **Datum početka** i **Datum završetka** .</span><span class="sxs-lookup"><span data-stu-id="d3f0b-108">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="d3f0b-109">Navedite korisničko ime za korisnika koje želite istražiti (korisnik koji je izbrisao stavke).</span><span class="sxs-lookup"><span data-stu-id="d3f0b-109">Specify username for the user that you want to investigate (the user who deleted the items).</span></span> <span data-ttu-id="d3f0b-110">U polju **aktivnosti** odaberite **izbrisane poruke iz mape Izbrisane stavke** i **premjestite poruke u mapu Izbrisane stavke**.</span><span class="sxs-lookup"><span data-stu-id="d3f0b-110">In the **Activities** field, select **Deleted messages from Deleted Items folder** and **Moved messages to Deleted Items folder**.</span></span>

4. <span data-ttu-id="d3f0b-111">Kliknite **Pretraživanje**.</span><span class="sxs-lookup"><span data-stu-id="d3f0b-111">Click **Search**.</span></span>

<span data-ttu-id="d3f0b-112">U rezultatima odaberite zapis nadzora.</span><span class="sxs-lookup"><span data-stu-id="d3f0b-112">In the results, select an audit record.</span></span> <span data-ttu-id="d3f0b-113">U nastavku pojedinosti kliknite **više informacija**.</span><span class="sxs-lookup"><span data-stu-id="d3f0b-113">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="d3f0b-114">Dodatne informacije o izbrisanoj stavci (na primjer, redak predmeta i mjesto stavke kada je izbrisana) prikazuju se u polju **Afecteditems** .</span><span class="sxs-lookup"><span data-stu-id="d3f0b-114">Additional information about the deleted item (for example, the subject line and the location of the item when it was deleted) is displayed in the **AffectedItems** field.</span></span> <span data-ttu-id="d3f0b-115">Svojstvo **Clientinfostring** prikazat će se ako je brisanje došlo u programu Outlook, Outlook na webu (prethodno poznat kao Outlook Web App) ili bilo koji drugi uređaj.</span><span class="sxs-lookup"><span data-stu-id="d3f0b-115">The **ClientInfoString** property will show if the deletion occurred in Outlook, Outlook on the web (formerly known as Outlook Web App), or any other device.</span></span>

<span data-ttu-id="d3f0b-116">Dodatne informacije potražite u članku [određivanje tko je postavio prosljeđivanje e-pošte za poštanski sandučić](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items).</span><span class="sxs-lookup"><span data-stu-id="d3f0b-116">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items).</span></span>

<span data-ttu-id="d3f0b-117">**Pažnja**: izbrisane stavke ne možete dohvatiti pomoću značajke zapisnika nadzora.</span><span class="sxs-lookup"><span data-stu-id="d3f0b-117">**Note**: You can't retrieve deleted items using the audit log feature.</span></span> <span data-ttu-id="d3f0b-118">Upute za dohvaćanje izbrisanih poruka u programu Outlook na webu potražite [u članku Oporavak izbrisanih stavki u web-aplikaciji programa Outlook](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span><span class="sxs-lookup"><span data-stu-id="d3f0b-118">To retrieve deleted messages in Outlook on the web, see [Recover deleted items in Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span></span>
