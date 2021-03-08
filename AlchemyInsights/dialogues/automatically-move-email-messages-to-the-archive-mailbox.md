---
title: Automatsko premještanje poruka e-pošte u arhivski poštanski sandučić
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100008"
- "7217"
ms.openlocfilehash: 14ded561ee2b3c244fadbdab42fd0e833a1c66d5
ms.sourcegitcommit: 7fa9bf6f9fc7438791aa9241a440e5be817d4401
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/08/2021
ms.locfileid: "50524097"
---
# <a name="automatically-move-email-messages-to-the-archive-mailbox"></a><span data-ttu-id="8ee22-102">Automatsko premještanje poruka e-pošte u arhivski poštanski sandučić</span><span class="sxs-lookup"><span data-stu-id="8ee22-102">Automatically move email messages to the archive mailbox</span></span>

<span data-ttu-id="8ee22-103">Slijede upute za postavljanje pravilnika da bi se korisnikova stara e-pošta automatski pomakila u poštanski sandučić arhive:</span><span class="sxs-lookup"><span data-stu-id="8ee22-103">Here's how to set up a policy to automatically move a user's old email to the archive mailbox:</span></span>

1. <span data-ttu-id="8ee22-104">Idite na [**sigurnosnu &**](https://go.microsoft.com/fwlink/p/?linkid=2077143)  >  **arhivu upravljanje podacima**  >   o usklađenosti da biste potvrdili da je za korisnika omogućen arhivski poštanski sandučić.</span><span class="sxs-lookup"><span data-stu-id="8ee22-104">Go to [**Security & Compliance**](https://go.microsoft.com/fwlink/p/?linkid=2077143) > **Data governance** > **Archive** to verify an archive mailbox has been enabled for the user.</span></span> <span data-ttu-id="8ee22-105">Ako nije, kliknite **Omogući** **da** u okviru upozorenje.</span><span class="sxs-lookup"><span data-stu-id="8ee22-105">If it hasn't, click **Enable** then **Yes** in the warning box.</span></span>
2. <span data-ttu-id="8ee22-106">Otvorite [**centar za administratore sustava Exchange > upravljanje usklađivanjem > oznake zadržavanja**](https://go.microsoft.com/fwlink/?linkid=2059104).</span><span class="sxs-lookup"><span data-stu-id="8ee22-106">Go to [**Exchange admin center > compliance management > retention tags**](https://go.microsoft.com/fwlink/?linkid=2059104).</span></span>
3. <span data-ttu-id="8ee22-107">Odaberite ikonu +, a zatim odaberite **automatski primijeni na cijeli poštanski sandučić**.</span><span class="sxs-lookup"><span data-stu-id="8ee22-107">Choose the + icon then choose **automatically apply to entire mailbox**.</span></span>
4. <span data-ttu-id="8ee22-108">Dodijelite naziv oznake zadržavanja, a zatim odaberite **Premjesti u arhivu**.</span><span class="sxs-lookup"><span data-stu-id="8ee22-108">Assign a name to the retention tag, and choose **Move to Archive**.</span></span> <span data-ttu-id="8ee22-109">Za razdoblje zadržavanja unesite željeno vrijeme, kao što je 90 days.</span><span class="sxs-lookup"><span data-stu-id="8ee22-109">For the retention period, enter the time you want, such as 90 days.</span></span> <span data-ttu-id="8ee22-110">Kliknite **Spremi**.</span><span class="sxs-lookup"><span data-stu-id="8ee22-110">Click **Save**.</span></span>
5. <span data-ttu-id="8ee22-111">Sada stvorite pravilnik o zadržavanju: odaberite **pravila zadržavanja**, odaberite ikonu da biste dodali novo pravilo.</span><span class="sxs-lookup"><span data-stu-id="8ee22-111">Now create a retention policy: choose **retention policies**, choose the icon to add a new policy.</span></span>
6. <span data-ttu-id="8ee22-112">Dodijelite naziv pravilima zadržavanja, a zatim kliknite, a zatim se pomaknite da biste pronašli i dodali oznaku zadržavanja koju ste upravo stvorili.</span><span class="sxs-lookup"><span data-stu-id="8ee22-112">Assign a name to the retention policy, then click and scroll to find and add the retention tag you just created.</span></span> <span data-ttu-id="8ee22-113">Kliknite **Spremi**.</span><span class="sxs-lookup"><span data-stu-id="8ee22-113">Click **Save**.</span></span>
7. <span data-ttu-id="8ee22-114">Konačno, primijenite pravilnik o zadržavanju na korisnikov poštanski sandučić: još uvijek u centru za administratore sustava Exchange idite na  >  **poštanske sandučiće** primatelja.</span><span class="sxs-lookup"><span data-stu-id="8ee22-114">Finally, apply the retention policy to the user's mailbox: still in the Exchange admin center, go to **recipients** > **mailboxes**.</span></span> <span data-ttu-id="8ee22-115">Odaberite sve korisnike na koje želite primijeniti pravilo, a zatim odaberite **Uređivanje** (ikona olovke).</span><span class="sxs-lookup"><span data-stu-id="8ee22-115">Choose all the users who you want to apply the policy to, then choose **Edit** (the pencil icon).</span></span>
8. <span data-ttu-id="8ee22-116">U dijaloškom okviru kliknite **značajke poštanskog sandučića**.</span><span class="sxs-lookup"><span data-stu-id="8ee22-116">In the dialog box, click **mailbox features**.</span></span> <span data-ttu-id="8ee22-117">U odjeljku **pravilnik o zadržavanju** primijenite pravilo koje ste upravo stvorili > **Spremanje**.</span><span class="sxs-lookup"><span data-stu-id="8ee22-117">Under **Retention policy**, apply the policy you just created > **Save**.</span></span>
9. <span data-ttu-id="8ee22-118">Upute za primjenu Pravilnika na sve korisnike potražite u članku [Primjena pravilnika o zadržavanju na poštanske sandučiće](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy).</span><span class="sxs-lookup"><span data-stu-id="8ee22-118">For instructions for applying the policy to all users, see [Apply a retention policy to mailboxes](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy).</span></span>
