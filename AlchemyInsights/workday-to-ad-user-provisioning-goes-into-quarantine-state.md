---
title: Radni dan za dodjelu resursa korisniku oglasa prelazi u stanje karantene
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8471"
- "9004687"
ms.openlocfilehash: 0fc519c8170de498c9bcb1fc41a76116bda48b1f
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50480965"
---
# <a name="workday-to-ad-user-provisioning-goes-into-quarantine-state"></a><span data-ttu-id="61a73-102">Radni dan za dodjelu resursa korisniku oglasa prelazi u stanje karantene</span><span class="sxs-lookup"><span data-stu-id="61a73-102">Workday to AD User Provisioning goes into quarantine state</span></span>

<span data-ttu-id="61a73-103">**Radni dan za dodjelu resursa korisniku oglasa prelazi u stanje karantene i nema korisnika koji se stvaraju u AD-u**</span><span class="sxs-lookup"><span data-stu-id="61a73-103">**Workday to AD User Provisioning goes into quarantine state and no users are created in AD**</span></span>

<span data-ttu-id="61a73-104">Radni dan za dodjelu resursa korisniku oglasa otišao je u stanje karantene, a zapisi nadzora prikazuju događaje s pogreškama u pogrešci **: Operacijepogreška-SvcErr: došlo je do pogreške u operaciji. Za servis direktorija nije konfiguriran nijedan nadređeni referenca. Imenički servis stoga ne može izdati preporuke objektima izvan ove šume**.</span><span class="sxs-lookup"><span data-stu-id="61a73-104">The Workday to AD User Provisioning job has gone into quarantine state and the audit logs show export failure events with the error message **Error: OperationsError-SvcErr: An operation error occurred. No superior reference has been configured for the directory service. The directory service is therefore unable to issue referrals to objects outside this forest**.</span></span> <span data-ttu-id="61a73-105">Ta se pogreška obično prikazuje ako kontejner servisa Active Directory OU nije pravilno postavljen ili ako postoje problemi s preslikavanjem izraza koji se koristi za **Parentdistinguishednaziv**.</span><span class="sxs-lookup"><span data-stu-id="61a73-105">This error usually shows up if the Active Directory Container OU is not set correctly or if there are issues with the Expression Mapping used for **parentDistinguishedName**.</span></span>

<span data-ttu-id="61a73-106">Potvrdite zadani parametar za **nove korisnike** za pogreške u pisanju.</span><span class="sxs-lookup"><span data-stu-id="61a73-106">Check the Default OU for **New Users** parameter for typos.</span></span> <span data-ttu-id="61a73-107">Uvjerite se da navedeni OU već postoji u vašem OGLASU.</span><span class="sxs-lookup"><span data-stu-id="61a73-107">Ensure that the specified OU already exists in your AD.</span></span> <span data-ttu-id="61a73-108">Ako u preslikaču atributa koristite **Parentdistinguishednaziv** , pobrinite se da uvijek bude vredan poznatom kontejneru unutar domene oglasa.</span><span class="sxs-lookup"><span data-stu-id="61a73-108">If you are using **parentDistinguishedName** in the attribute mapping, ensure that it always evaluates to a known container within the AD domain.</span></span> <span data-ttu-id="61a73-109">Provjerite događaj izvoza u zapisnicima nadzora da biste vidjeli generiranu vrijednost.</span><span class="sxs-lookup"><span data-stu-id="61a73-109">Check the Export event in the audit logs to see the generated value.</span></span>

<span data-ttu-id="61a73-110">Dodatne informacije o konfiguriranju radnog dana za automatiziranu dodjelu resursa potražite u članku [Udžbenik: Konfiguriranje radnog dana za automatsku dodjelu korisnika](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span><span class="sxs-lookup"><span data-stu-id="61a73-110">For more details on configuring workday for automated provisioning, see [Tutorial: Configure Workday for automatic user provisioning](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>

