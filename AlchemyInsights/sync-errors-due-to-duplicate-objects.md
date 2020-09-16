---
title: 902 (pogreške pri sinkronizaciji zbog dupliciranih objekata)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: 33b8ad0a33eb02eb9ec5bd26f94b00e5645b3fd7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47737333"
---
# <a name="sync-errors-due-to-duplicate-objects"></a><span data-ttu-id="ca9cb-102">Pogreške prilikom sinkronizacije zbog dupliciranih objekata</span><span class="sxs-lookup"><span data-stu-id="ca9cb-102">Sync errors due to duplicate objects</span></span>

<span data-ttu-id="ca9cb-103">Možda će vam se prikazati jedna od sljedećih poruka o pogrešci kada sinkronizacija direktorija završi u programu Microsoft 365:</span><span class="sxs-lookup"><span data-stu-id="ca9cb-103">You might receive one of the following error messages when directory synchronization finishes in Microsoft 365:</span></span>

- <span data-ttu-id="ca9cb-104">Nije moguće ažurirati ovaj objekt u Microsoftovim internetskim servisima jer sljedeći atributi pridruženi ovom objektu imaju vrijednosti koje su možda već povezane s drugim objektom u lokalnom direktoriju.</span><span class="sxs-lookup"><span data-stu-id="ca9cb-104">Unable to update this object in Microsoft Online Services because the following attributes associated with this object have values that may already be associated with another object in your local directory.</span></span>

- <span data-ttu-id="ca9cb-105">Sinkronizirani objekt s istom proxy adresom već postoji u direktoriju Microsoftova internetskih servisa.</span><span class="sxs-lookup"><span data-stu-id="ca9cb-105">A synchronized object with the same proxy address already exists in your Microsoft Online Services directory.</span></span>

- <span data-ttu-id="ca9cb-106">Ovaj objekt nije moguće ažurirati jer sljedeći atributi pridruženi ovom objektu imaju vrijednosti koje se možda već povezuju s drugim objektom u lokalnim imeničkim servisima: UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="ca9cb-106">Unable to update this object because the following attributes associated with this object have values that may already be associated with another object in your local directory services: UserPrincipalName.</span></span>

<span data-ttu-id="ca9cb-107">Da biste identificirali i riješili problem, Preuzmite i pokrenite [alat za ispravljanje pogrešaka u Idfix DirSync](https://www.microsoft.com/download/details.aspx?id=36832).</span><span class="sxs-lookup"><span data-stu-id="ca9cb-107">To identify and fix the issue, download and run the [IdFix DirSync Error Remediation Tool](https://www.microsoft.com/download/details.aspx?id=36832).</span></span>

<span data-ttu-id="ca9cb-108">Dodatne informacije potražite u članku [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span><span class="sxs-lookup"><span data-stu-id="ca9cb-108">For more information, see [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span></span>
