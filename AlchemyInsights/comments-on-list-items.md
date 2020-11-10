---
title: Komentari na stavkama popisa
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
- "9003821"
- "6841"
ms.openlocfilehash: 5940d1a96324c5ca77331485a115689abe547ef7
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 11/09/2020
ms.locfileid: "48982433"
---
# <a name="comments-on-list-items"></a><span data-ttu-id="ddda8-102">Komentari na stavkama popisa</span><span class="sxs-lookup"><span data-stu-id="ddda8-102">Comments on List items</span></span>

<span data-ttu-id="ddda8-103">Korisnici će uskoro moći dodavati i brisati komentare na stavkama popisa.</span><span class="sxs-lookup"><span data-stu-id="ddda8-103">Users will soon be able to add and delete comments on list items.</span></span> <span data-ttu-id="ddda8-104">Korisnici mogu pregledavati sve komentare na stavci popisa i filtrirati prikaze koji prikazuju komentare ili aktivnost povezane s artiklom.</span><span class="sxs-lookup"><span data-stu-id="ddda8-104">Users can view all comments on a list item and filter between views that show comments or activity related to an item.</span></span>

<span data-ttu-id="ddda8-105">**Timing** :</span><span class="sxs-lookup"><span data-stu-id="ddda8-105">**Timing** :</span></span>

<span data-ttu-id="ddda8-106">**Ciljano izdanje** : postupno iskotrljati sredinom listopada i očekuje se da će završiti do sredine studenog</span><span class="sxs-lookup"><span data-stu-id="ddda8-106">**Targeted release** : Gradual roll out in mid-October and expected to complete by mid-November</span></span>

<span data-ttu-id="ddda8-107">**Standardno izdanje** : postupno iskotrljati sredinom studenog i očekuje se da će završiti početkom prosinca</span><span class="sxs-lookup"><span data-stu-id="ddda8-107">**Standard release** : Gradual roll out in mid-November and expected to complete by early December</span></span>

<span data-ttu-id="ddda8-108">**Primjena** : ciljano izdanje za cijelu tvrtku ili ustanovu</span><span class="sxs-lookup"><span data-stu-id="ddda8-108">**Rollout** : Targeted release for the entire organization</span></span>

<span data-ttu-id="ddda8-109">Korisnici moraju napomenuti sljedeće da bi mogli dodavati i brisati komentare:</span><span class="sxs-lookup"><span data-stu-id="ddda8-109">Users need to note the following before they can add and delete comments:</span></span>

- <span data-ttu-id="ddda8-110">Komentari slijede postavke dozvola koje su prisutne u sustavu SharePoint.</span><span class="sxs-lookup"><span data-stu-id="ddda8-110">Comments follow the permission settings inherent in SharePoint.</span></span>
- <span data-ttu-id="ddda8-111">Klasični popisi koji još nisu ugrađeni da bi se prikazivale u modernim korisničkim sučeljima, kao što su popisi zadataka, neće imati ovu značajku komentiranja.</span><span class="sxs-lookup"><span data-stu-id="ddda8-111">Classic lists that are not yet built to show up in modern user interfaces, like task lists, will not have this commenting feature.</span></span>
- <span data-ttu-id="ddda8-112">Komentiranje popisa u timovima nije dostupno uz ovo izdanje.</span><span class="sxs-lookup"><span data-stu-id="ddda8-112">Commenting on lists in Teams is not available with this release.</span></span>
- <span data-ttu-id="ddda8-113">Komentari se ne indeksiraju pomoću pretraživanja.</span><span class="sxs-lookup"><span data-stu-id="ddda8-113">Comments are not indexed by Search.</span></span>

<span data-ttu-id="ddda8-114">Administratori mogu onemogućiti ovu značajku na razini tvrtke ili ustanove promjenom parametra **Commentsonlistitemsdisabled** u **cmdletu Set-spostanar** PowerShell.</span><span class="sxs-lookup"><span data-stu-id="ddda8-114">Admins can disable this feature at the organization level by changing the **CommentsOnListItemsDisabled** parameter in the **Set-SPOTenant** PowerShell cmdlet.</span></span>

<span data-ttu-id="ddda8-115">Trenutno nije moguće onemogućiti komentiranje na razini web-mjesta ili popisa.</span><span class="sxs-lookup"><span data-stu-id="ddda8-115">It is not currently possible to disable commenting at the site or list level.</span></span> <span data-ttu-id="ddda8-116">Nadamo se da ćemo te kontrole imati u kasnijim ažuriranju, vjerojatno u prvom tromjesečju 2021.</span><span class="sxs-lookup"><span data-stu-id="ddda8-116">We hope to have those controls in a later update, likely in the first quarter 2021.</span></span>
