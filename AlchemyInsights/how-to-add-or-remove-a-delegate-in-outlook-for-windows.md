---
title: Dodavanje i uklanjanje delegata u programu Outlook za Windows
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800004"
- "7334"
ms.openlocfilehash: fcbd6082c104f0e1bca022a23cbbeb6e3363a6c5
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573304"
---
# <a name="how-to-add-or-remove-a-delegate-in-outlook-for-windows"></a><span data-ttu-id="88529-102">Dodavanje i uklanjanje delegata u programu Outlook za Windows</span><span class="sxs-lookup"><span data-stu-id="88529-102">How to add or remove a Delegate in Outlook for Windows</span></span>

<span data-ttu-id="88529-103">Da biste dodali delegata u programu Outlook za Windows, učinite sljedeće:</span><span class="sxs-lookup"><span data-stu-id="88529-103">To add a Delegate in Outlook for Windows:</span></span> 

1. <span data-ttu-id="88529-104">Kliknite karticu **datoteka** , a zatim **Postavke računa**, a zatim odaberite **pristup delegiranju**.</span><span class="sxs-lookup"><span data-stu-id="88529-104">Click on the **File** tab followed by **Account Settings**, and then choose **Delegate Access**.</span></span>
2. <span data-ttu-id="88529-105">Kliknite **Dodaj**.</span><span class="sxs-lookup"><span data-stu-id="88529-105">Click on **Add**.</span></span> <span data-ttu-id="88529-106">Ako se **Dodavanje** ne prikazuje, aktivna veza možda ne postoji između programa Outlook i sustava Exchange.</span><span class="sxs-lookup"><span data-stu-id="88529-106">If **Add** doesn’t appear, an active connection might not exist between Outlook and Exchange.</span></span> <span data-ttu-id="88529-107">Traka stanja programa Outlook prikazuje status veze.</span><span class="sxs-lookup"><span data-stu-id="88529-107">The Outlook status bar displays the connection status.</span></span>
3. <span data-ttu-id="88529-108">Upišite ime osobe koju želite označiti kao delegat ili pretražite i odaberite naziv na popisu rezultata pretraživanja.</span><span class="sxs-lookup"><span data-stu-id="88529-108">Type the name of the person you want to designate as your delegate, or search and choose the name in the search results list.</span></span>

    > [!NOTE]
    > <span data-ttu-id="88529-109">Delegat mora biti osoba na globalnom popisu adresa sustava Exchange tvrtke ili ustanove (GAL).</span><span class="sxs-lookup"><span data-stu-id="88529-109">The delegate must be a person in your organization's Exchange Global Address List (GAL).</span></span>
4. <span data-ttu-id="88529-110">Kliknite **Dodaj** , a zatim **u redu**.</span><span class="sxs-lookup"><span data-stu-id="88529-110">Click on **Add** followed by **OK**.</span></span>
5. <span data-ttu-id="88529-111">U dijaloškom okviru **dozvole delegata** prihvatite zadane postavke dozvola ili odaberite prilagođene razine pristupa za mape sustava Exchange.</span><span class="sxs-lookup"><span data-stu-id="88529-111">In the **Delegate Permissions** dialog box, accept the default permission settings or select custom access levels for Exchange folders.</span></span>

    - <span data-ttu-id="88529-112">Ako delegatu treba dozvola za rad samo sa zahtevima za sastanak i odgovorima, zadane postavke dozvola, kao što je **delegira, primaju kopije poruka vezanih uz sastanak poslane meni** su dovoljne.</span><span class="sxs-lookup"><span data-stu-id="88529-112">If a delegate needs permission to work only with meeting requests and responses, the default permission settings such as **Delegate receives copies of meeting-related messages sent to me** are sufficient.</span></span> <span data-ttu-id="88529-113">Postavku dozvola **ulazne pošte** možete ostaviti na servisu **none**.</span><span class="sxs-lookup"><span data-stu-id="88529-113">You can leave the **Inbox** permission setting at **None**.</span></span> <span data-ttu-id="88529-114">Zahtjevi za sastanak i odgovori izravno će doći do ulazne pošte delegata.</span><span class="sxs-lookup"><span data-stu-id="88529-114">Meeting requests and responses will go directly to the delegate's inbox.</span></span>

    > [!NOTE]
    > <span data-ttu-id="88529-115">Delegat je po zadanom odobren za **urednika (može čitati, stvarati i mijenjati stavke)** u mapu **kalendara** .</span><span class="sxs-lookup"><span data-stu-id="88529-115">By default, the delegate is granted **Editor (can read, create, and modify items)** permission to your **Calendar** folder.</span></span> <span data-ttu-id="88529-116">Kada delegira sastanak u vaše ime, on se automatski dodaje u mapu **kalendara** .</span><span class="sxs-lookup"><span data-stu-id="88529-116">When the delegate responds to a meeting on your behalf, it is automatically added to your **Calendar** folder.</span></span>

5. <span data-ttu-id="88529-117">Da biste slali poruku da biste obavijestili delegata o promijenjenim dozvolama, potvrdite okvir **automatski šalji poruku delegiranju sažetka tih dozvola** .</span><span class="sxs-lookup"><span data-stu-id="88529-117">To send a message to notify the delegate of the changed permissions, select the **Automatically send a message to delegate summarizing these permissions** check box.</span></span>
6. <span data-ttu-id="88529-118">Ako želite, potvrdite okvir **delegat može vidjeti moje privatne stavke** .</span><span class="sxs-lookup"><span data-stu-id="88529-118">If you want, select the **Delegate can see my private items** check box.</span></span>

    > [!IMPORTANT]
    > <span data-ttu-id="88529-119">Ta postavka utječe na sve mape sustava Exchange.</span><span class="sxs-lookup"><span data-stu-id="88529-119">This setting affects all Exchange folders.</span></span> <span data-ttu-id="88529-120">To obuhvaća sve mape pošta, kontakti, kalendar, zadaci, bilješke i dnevnik.</span><span class="sxs-lookup"><span data-stu-id="88529-120">This includes all Mail, Contacts, Calendar, Tasks, Notes, and Journal folders.</span></span> <span data-ttu-id="88529-121">Pristup privatnim stavkama ne može se omogućiti samo u navedenim mapama.</span><span class="sxs-lookup"><span data-stu-id="88529-121">There is no way to grant access to private items in only specified folders.</span></span>

7. <span data-ttu-id="88529-122">Odaberite **u redu**.</span><span class="sxs-lookup"><span data-stu-id="88529-122">Choose **OK**.</span></span>

    > [!NOTE]
    >
    > - <span data-ttu-id="88529-123">Poruke poslane s **dozvolama za slanje** u ime obuhvaćaju i delegate i vaša imena pokraj pošiljatelja.</span><span class="sxs-lookup"><span data-stu-id="88529-123">Messages sent with Send on Behalf permissions include both the delegate's and your names next to **From**.</span></span> <span data-ttu-id="88529-124">Kada se poruka pošalje s dozvolama za slanje kao, prikazat će se samo vaše ime.</span><span class="sxs-lookup"><span data-stu-id="88529-124">When a message is sent with Send As permissions, only your name appears.</span></span>
    > - <span data-ttu-id="88529-125">Kada nekoga dodate kao delegata, možete dodati poštanski sandučić sustava Exchange u njegov profil programa Outlook.</span><span class="sxs-lookup"><span data-stu-id="88529-125">Once you add someone as a delegate, they can add your Exchange mailbox to their Outlook profile.</span></span> <span data-ttu-id="88529-126">Upute potražite u članku [Upravljanje stavkama pošte i kalendara neke druge osobe](https://support.microsoft.com/office/manage-another-person-s-mail-and-calendar-items-afb79d6b-2967-43b9-a944-a6b953190af5).</span><span class="sxs-lookup"><span data-stu-id="88529-126">For instructions, see [Manage another person's mail and calendar items](https://support.microsoft.com/office/manage-another-person-s-mail-and-calendar-items-afb79d6b-2967-43b9-a944-a6b953190af5).</span></span>

<span data-ttu-id="88529-127">Da biste uklonili delegata u programu Outlook za Windows, učinite sljedeće:</span><span class="sxs-lookup"><span data-stu-id="88529-127">To remove a Delegate in Outlook for Windows:</span></span>

1. <span data-ttu-id="88529-128">Kliknite karticu **datoteka** .</span><span class="sxs-lookup"><span data-stu-id="88529-128">Click on the **File** tab.</span></span>
2. <span data-ttu-id="88529-129">Kliknite **Postavke računa** , a zatim **pristupite delegiranju**.</span><span class="sxs-lookup"><span data-stu-id="88529-129">Click on **Account Settings** followed by **Delegate Access**.</span></span>
3. <span data-ttu-id="88529-130">Odaberite naziv delegata za kojeg želite promijeniti dozvole, a zatim kliknite **Ukloni** , a zatim **u redu**.</span><span class="sxs-lookup"><span data-stu-id="88529-130">Choose the name of the delegate for whom you want to change permissions, and then click on **Remove** followed by **OK**.</span></span>
