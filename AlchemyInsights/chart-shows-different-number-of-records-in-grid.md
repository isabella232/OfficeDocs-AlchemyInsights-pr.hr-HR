---
title: Grafikon sadrži različit broj zapisa u rešetki
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5611"
- "9002930"
ms.openlocfilehash: e499a439e7cf7e9ecbb6566f9f089f3b7b82f48e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47793750"
---
# <a name="chart-shows-different-number-of-records-in-grid"></a><span data-ttu-id="8e1ff-102">Grafikon sadrži različit broj zapisa u rešetki</span><span class="sxs-lookup"><span data-stu-id="8e1ff-102">Chart shows different number of records in grid</span></span>

<span data-ttu-id="8e1ff-103">**Simptom**</span><span class="sxs-lookup"><span data-stu-id="8e1ff-103">**Symptom**</span></span>

<span data-ttu-id="8e1ff-104">Za grafikon na stranici nadzorne ploče kada kliknete grafikon "..." i kliknite "prikaz zapisa", možete se kretati do stranice rešetke da bi vam se prikazale svi zapisi. Ponekad se broj zapisa mijenja.</span><span class="sxs-lookup"><span data-stu-id="8e1ff-104">For chart on dashboard page, when you click on chart "…" and click "View records", you navigate to grid page to see all the records.Sometimes, the number of records changes.</span></span>

<span data-ttu-id="8e1ff-105">**Jer**</span><span class="sxs-lookup"><span data-stu-id="8e1ff-105">**Cause**</span></span>

<span data-ttu-id="8e1ff-106">To je zbog razlike u prikazima između grafikona na izvornoj stranici nadzorne ploče i grafikona na početnoj stranici rešetke.</span><span class="sxs-lookup"><span data-stu-id="8e1ff-106">This is due to the difference of views between the chart on the original dashboard page and the chart on the grid home page.</span></span>  

<span data-ttu-id="8e1ff-107">**Rješenje**</span><span class="sxs-lookup"><span data-stu-id="8e1ff-107">**Solution**</span></span>

1. <span data-ttu-id="8e1ff-108">Provjerite prikaz s izvorne stranice i prikaza u rešetki da biste vidjeli jesu li drukčiji.</span><span class="sxs-lookup"><span data-stu-id="8e1ff-108">Check the view from the original page and the view in the grid to see if they are different.</span></span>
2. <span data-ttu-id="8e1ff-109">Promijenite prikaz u rešetki da bi odgovarao prikazu na izvornoj stranici.</span><span class="sxs-lookup"><span data-stu-id="8e1ff-109">Change the view in grid to match the view in the original page.</span></span>
3. <span data-ttu-id="8e1ff-110">Ako se ne pronađe ispravan prikaz, to obično znači da prikaz nije omogućen u dizajneru aplikacija.</span><span class="sxs-lookup"><span data-stu-id="8e1ff-110">If the correct view cannot be found, usually it means the view is not enabled in app designer.</span></span>
4. <span data-ttu-id="8e1ff-111">Idite na dizajner aplikacije određene aplikacije, odaberite entitet i njegove prikaze, provjerite prikaz koji želite omogućiti, spremiti, objavljivati i zatvarati.</span><span class="sxs-lookup"><span data-stu-id="8e1ff-111">Go to app designer of the specific app, choose the entity and its views, check the view you want to enable, save, publish and close.</span></span>
5. <span data-ttu-id="8e1ff-112">Osvježite stranicu.</span><span class="sxs-lookup"><span data-stu-id="8e1ff-112">Refresh the page.</span></span>