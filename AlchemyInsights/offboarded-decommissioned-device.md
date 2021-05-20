---
title: Problemi s uklanjanjem uređaja izvan pogona ili uređaja izvan pogona iz inventara uređaja
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/11/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002913"
- "11187"
ms.openlocfilehash: 46ac46c583cd0ac956797737d8150277f0d79ba5
ms.sourcegitcommit: c685f197dbf83a9dfd85e9acfdf14a4daf0e9a5a
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 05/11/2021
ms.locfileid: "52564079"
---
# <a name="issues-with-removing-an-offboarded-or-decommissioned-device-from-the-device-inventory"></a><span data-ttu-id="d3834-102">Problemi s uklanjanjem uređaja izvan pogona ili uređaja izvan pogona iz inventara uređaja</span><span class="sxs-lookup"><span data-stu-id="d3834-102">Issues with removing an offboarded or decommissioned device from the Device Inventory</span></span>

<span data-ttu-id="d3834-103">Microsoft Defender za krajnju točku trenutno ne dopušta ručno uklanjanje zapisa uređaja s isključenog uređaja ili uređaja izvan pogona iz inventara uređaja.</span><span class="sxs-lookup"><span data-stu-id="d3834-103">Microsoft Defender for Endpoint does not currently allow manually removing the device record of an offboarded or decommissioned device from the Device Inventory.</span></span>

<span data-ttu-id="d3834-104">U sigurnosne svrhe uređaj ostaje na portalu kao povijesni zapis do 180 dana.</span><span class="sxs-lookup"><span data-stu-id="d3834-104">For security purposes, the device remains in the portal as an historical record for up to 180 days.</span></span> <span data-ttu-id="d3834-105">No podaci o uređaju očišćeni su u skladu s konfiguriranim razdobljem zadržavanja.</span><span class="sxs-lookup"><span data-stu-id="d3834-105">However, the device data is purged according to your configured retention period.</span></span>

<span data-ttu-id="d3834-106">**Napomena:** Isključeni uređaj ili uređaj izvan pogona automatski se prebacuje u **neaktivno** stanje nakon sedam dana.</span><span class="sxs-lookup"><span data-stu-id="d3834-106">**Note:** An offboarded or decommissioned device switches automatically to **Inactive** state after seven days.</span></span> <span data-ttu-id="d3834-107">Osim toga, uređaji koji nisu aktivni u zadnjih 30 dana ne uvrštiraju se u podatke koji odražavaju rezultat izlaganja upravljanje prijetnjama i ranjivostima ili Microsoftov sigurni rezultat za uređaje.</span><span class="sxs-lookup"><span data-stu-id="d3834-107">In addition, devices not active in the last 30 days are not factored into the data that reflects your organization threat and vulnerability management exposure score or Microsoft Secure Score for Devices.</span></span>
 
<span data-ttu-id="d3834-108">Ako i dalje ne želite vidjeti određene uređaje u prikazu inventara uređaja, pokušajte s postavljanjem oznake uređaja filtrirati uređaj izvan pogona iz prikaza Inventar uređaja.</span><span class="sxs-lookup"><span data-stu-id="d3834-108">If you still don't want to see certain devices in Device Inventory view, try placing a device tag to filter out the decommissioned device from the Device Inventory view.</span></span>

<span data-ttu-id="d3834-109">Dodatne informacije potražite u sljedećim člancima:</span><span class="sxs-lookup"><span data-stu-id="d3834-109">For more information, see:</span></span>

[<span data-ttu-id="d3834-110">Offboard devices from the Microsoft Defender for Endpoint service</span><span class="sxs-lookup"><span data-stu-id="d3834-110">Offboard devices from the Microsoft Defender for Endpoint service</span></span>](/microsoft-365/security/defender-endpoint/offboard-machines.md)

[<span data-ttu-id="d3834-111">Rezultat izlaganja u upravljanje prijetnjama i ranjivostima</span><span class="sxs-lookup"><span data-stu-id="d3834-111">Exposure score in threat and vulnerability management</span></span>](/microsoft-365/security/defender-endpoint/tvm-exposure-score.md)

[<span data-ttu-id="d3834-112">Rješavanje problema s nezdravim senzorima u programu Microsoft Defender za krajnju točku</span><span class="sxs-lookup"><span data-stu-id="d3834-112">Fix unhealthy sensors in Microsoft Defender for Endpoint</span></span>](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors#inactive-devices.md)

[<span data-ttu-id="d3834-113">Učinkovito korištenje označavanja (1. dio)</span><span class="sxs-lookup"><span data-stu-id="d3834-113">How to use tagging effectively (Part 1)</span></span>](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-1/ba-p/1964058)

[<span data-ttu-id="d3834-114">Učinkovito korištenje označavanja (2. dio)</span><span class="sxs-lookup"><span data-stu-id="d3834-114">How to use tagging effectively (Part 2)</span></span>](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-2/ba-p/1962008)

[<span data-ttu-id="d3834-115">Učinkovito korištenje označavanja (3. dio)</span><span class="sxs-lookup"><span data-stu-id="d3834-115">How to use tagging effectively (Part 3)</span></span>](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-3/ba-p/1964073)




