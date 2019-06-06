---
title: Rješavanje problema s porukama pristup odbijen
ms.author: kirks
author: Techwriter40
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 5958ad06ca905f713b5f56aa5c536e95a485f01c
ms.sourcegitcommit: 241e21b6da226563bf70bdb1f5bad3d91c38cd2c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/05/2019
ms.locfileid: "34735730"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="4dfb6-102">Rješavanje problema s porukama pristup odbijen</span><span class="sxs-lookup"><span data-stu-id="4dfb6-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="4dfb6-103">Ako primate uskraćen prilikom pokušaja Pregledaj web-mjesta Sharepoint Online pristup, Molim pogledajte u ispod članaka.</span><span class="sxs-lookup"><span data-stu-id="4dfb6-103">If you are receiving an access denied message when attempting to browse a Sharepoint Online site, please see the below articles.</span></span>

## <a name="add-and-license-the-user"></a><span data-ttu-id="4dfb6-104">Dodajte i licence korisnika</span><span class="sxs-lookup"><span data-stu-id="4dfb6-104">Add and License the user</span></span>

<span data-ttu-id="4dfb6-105">Provjerite koje ste [dodijelili licence korisnicima u Office 365 poslovne](https://docs.microsoft.com/en-us/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span><span class="sxs-lookup"><span data-stu-id="4dfb6-105">Ensure that you [Assign licenses to users in Office 365 for business](https://docs.microsoft.com/en-us/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span></span>

<span data-ttu-id="4dfb6-106">Dodijelite dozvole</span><span class="sxs-lookup"><span data-stu-id="4dfb6-106">Assign Permissions</span></span>

<span data-ttu-id="4dfb6-107">Ako korisnik je dodijeljena licenca Sharepoint i još uvijek primanje uskraćen pristup, provjerite imaju [odgovarajuću razinu dozvole dodijeljene](https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="4dfb6-107">If the user has been assigned a Sharepoint license and is still receiving an access denied message, please ensure they have the [appropriate permission level assigned](https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels).</span></span>

<span data-ttu-id="4dfb6-108">Razmislite o korištenju značajke zahtjeva pristupa</span><span class="sxs-lookup"><span data-stu-id="4dfb6-108">Consider using the access request feature</span></span>

<span data-ttu-id="4dfb6-109">Značajka [zahtjev access](https://support.office.com/en-us/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) omogućuje korisnicima zatražili pristup sadržaju trenutno nemaju dozvolu za prikaz.</span><span class="sxs-lookup"><span data-stu-id="4dfb6-109">The [access request](https://support.office.com/en-us/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) feature allows people to request access to content that they do not currently have permission to see.</span></span> 

<span data-ttu-id="4dfb6-110">Dopusti Prilagođena skripta može uzrokovati pristup odbijen problemi</span><span class="sxs-lookup"><span data-stu-id="4dfb6-110">Allow custom script may cause access denied issues</span></span>

<span data-ttu-id="4dfb6-111">Postoje određene scenarije gdje "Dopusti Prilagođena skripta" značajka možda biti dosljedna odbijen pristup.</span><span class="sxs-lookup"><span data-stu-id="4dfb6-111">There are certain scenarios where the "Allow custom script" feature may be presenting an access denied.</span></span> <span data-ttu-id="4dfb6-112">Za popis utječe na sljedeće značajke, Sigurnosna razmatranja i onemogućiti značajku.</span><span class="sxs-lookup"><span data-stu-id="4dfb6-112">For a list of features affected, security considerations and the ability to disable the feature.</span></span> <span data-ttu-id="4dfb6-113">Posjetite, [Dopusti ili spriječiti prilagođene skripte](https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script)</span><span class="sxs-lookup"><span data-stu-id="4dfb6-113">Please visit , [Allow or prevent custom script](https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script)</span></span>

<span data-ttu-id="4dfb6-114">Napomena: Ako OneDrive ili SharePoint web-mjesta nije dostupno više korisnike koji su prethodno imali pristup, možda postoji problem privremeni servisa.</span><span class="sxs-lookup"><span data-stu-id="4dfb6-114">Note: If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> <span data-ttu-id="4dfb6-115">[Provjerite servisa stanja nadzorne ploče](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="4dfb6-115">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


  

