---
title: Stvaranje oznaka ili grupa uređaja i upravljanje njima
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11446"
- "9003537"
ms.openlocfilehash: 3a7d53beaaf830055904f0634f09a3e9e447006e
ms.sourcegitcommit: 1226e9a9601dc8fc8ec427235f3c2dd88ff84ced
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/02/2021
ms.locfileid: "52731340"
---
# <a name="create-and-manage-device-tags-or-groups"></a><span data-ttu-id="6002e-102">Stvaranje oznaka ili grupa uređaja i upravljanje njima</span><span class="sxs-lookup"><span data-stu-id="6002e-102">Create and manage device tags or groups</span></span>

<span data-ttu-id="6002e-103">Dodajte oznake na uređajima da biste stvorili pripadnost logičkoj grupi.</span><span class="sxs-lookup"><span data-stu-id="6002e-103">Add tags on devices to create a logical group affiliation.</span></span> <span data-ttu-id="6002e-104">Oznake uređaja podržavaju pravilno mapiranje mreže, što omogućuje prilaganje različitih oznaka radi snimanja konteksta i omogućivanja stvaranja dinamičkog popisa u sklopu incidenta.</span><span class="sxs-lookup"><span data-stu-id="6002e-104">Device tags support proper mapping of the network, enabling you to attach different tags to capture context and to enable dynamic list creation as part of an incident.</span></span> <span data-ttu-id="6002e-105">Oznake se mogu koristiti kao filtar u prikazu popisa Uređaji ili za grupiranje uređaja.</span><span class="sxs-lookup"><span data-stu-id="6002e-105">Tags can be used as a filter in Devices list view, or to group devices.</span></span> <span data-ttu-id="6002e-106">Dodatne informacije o grupiranje uređaja potražite u članku Stvaranje [oznaka uređaja i upravljanje njima.](/microsoft-365/security/defender-endpoint/machine-tags)</span><span class="sxs-lookup"><span data-stu-id="6002e-106">For more information on device grouping, see [Create and manage device tags](/microsoft-365/security/defender-endpoint/machine-tags).</span></span>

<span data-ttu-id="6002e-107">Oznake na uređajima možete dodati na sljedeće:</span><span class="sxs-lookup"><span data-stu-id="6002e-107">You can add tags on devices by:</span></span>

- <span data-ttu-id="6002e-108">Korištenje portala</span><span class="sxs-lookup"><span data-stu-id="6002e-108">Using the portal</span></span>

- <span data-ttu-id="6002e-109">Postavljanje vrijednosti ključa registra</span><span class="sxs-lookup"><span data-stu-id="6002e-109">Setting a registry key value</span></span>
 
<span data-ttu-id="6002e-110">**Napomena:** Može biti kašnjenja između vremena dodavanja oznake na uređaj i dostupnosti na popisu uređaja i na stranici uređaja.</span><span class="sxs-lookup"><span data-stu-id="6002e-110">**Note:** There could be latency between the time a tag is added to a device and its availability in the devices list and device page.</span></span>

<span data-ttu-id="6002e-111">Da biste dodali oznake uređaja pomoću API-ja, [pogledajte dodavanje ili uklanjanje API oznaka uređaja](/microsoft-365/security/defender-endpoint/add-or-remove-machine-tags).</span><span class="sxs-lookup"><span data-stu-id="6002e-111">To add device tags using API, see [Add or remove device tags API](/microsoft-365/security/defender-endpoint/add-or-remove-machine-tags).</span></span>

## <a name="add-and-manage-device-tags-using-the-portal"></a><span data-ttu-id="6002e-112">Dodavanje oznaka uređaja i upravljanje njima pomoću portala</span><span class="sxs-lookup"><span data-stu-id="6002e-112">Add and manage device tags using the portal</span></span>

1. <span data-ttu-id="6002e-113">Odaberite uređaj na koji želite upravljati oznakama.</span><span class="sxs-lookup"><span data-stu-id="6002e-113">Select the device that you want to manage tags on.</span></span> <span data-ttu-id="6002e-114">Uređaj možete odabrati ili potražiti iz bilo kojeg od sljedećih prikaza:</span><span class="sxs-lookup"><span data-stu-id="6002e-114">You can select or search for a device from any of the following views:</span></span>

    - <span data-ttu-id="6002e-115">**Nadzorna ploča sigurnosnih operacija** U odjeljku Top uređaji s aktivnim upozorenjima odaberite naziv uređaja.</span><span class="sxs-lookup"><span data-stu-id="6002e-115">**Security operations dashboard** Select the device name from the Top devices with active alerts section.</span></span>
    - <span data-ttu-id="6002e-116">**Red čekanja upozorenja** – odaberite naziv uređaja pokraj ikone uređaja iz reda čekanja upozorenja.</span><span class="sxs-lookup"><span data-stu-id="6002e-116">**Alerts queue** - Select the device name beside the device icon from the alerts queue.</span></span>
    - <span data-ttu-id="6002e-117">**Popis uređaji** – na popisu uređaja odaberite naziv uređaja.</span><span class="sxs-lookup"><span data-stu-id="6002e-117">**Devices list** - Select the device name from the list of devices.</span></span>
    - <span data-ttu-id="6002e-118">**Okvir za** pretraživanje – na padajućem izborniku odaberite Uređaj pa unesite naziv uređaja.</span><span class="sxs-lookup"><span data-stu-id="6002e-118">**Search box** - Select Device from the drop-down menu and enter the device name.</span></span>

    <span data-ttu-id="6002e-119">Stranicu upozorenja možete doći i putem prikaza datoteke i IP-a.</span><span class="sxs-lookup"><span data-stu-id="6002e-119">You can also get to the alert page through the file and IP views.</span></span>

1. <span data-ttu-id="6002e-120">U **retku Akcija** odgovora odaberite Upravljanje oznakama.</span><span class="sxs-lookup"><span data-stu-id="6002e-120">Select **Manage Tags** from the row of Response actions.</span></span>

1. <span data-ttu-id="6002e-121">Upišite da biste pronašli ili stvorili oznake.</span><span class="sxs-lookup"><span data-stu-id="6002e-121">Type to find or create tags.</span></span>

<span data-ttu-id="6002e-122">Oznake se dodaju u prikaz uređaja i odražavaju se na prikazu popisa Uređaji.</span><span class="sxs-lookup"><span data-stu-id="6002e-122">Tags are added to the device view and are reflected on the Devices list view.</span></span> <span data-ttu-id="6002e-123">Zatim pomoću filtra Oznake možete vidjeti odgovarajući popis uređaja.</span><span class="sxs-lookup"><span data-stu-id="6002e-123">You can then use the Tags filter to see the relevant list of devices.</span></span>

<span data-ttu-id="6002e-124">Dodatne informacije potražite u članku [Stvaranje oznaka uređaja i upravljanje njima.](/microsoft-365/security/defender-endpoint/machine-tags)</span><span class="sxs-lookup"><span data-stu-id="6002e-124">For more information, see [Create and manage device tags](/microsoft-365/security/defender-endpoint/machine-tags).</span></span>