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
# <a name="workday-to-ad-user-provisioning-goes-into-quarantine-state"></a>Radni dan za dodjelu resursa korisniku oglasa prelazi u stanje karantene

**Radni dan za dodjelu resursa korisniku oglasa prelazi u stanje karantene i nema korisnika koji se stvaraju u AD-u**

Radni dan za dodjelu resursa korisniku oglasa otišao je u stanje karantene, a zapisi nadzora prikazuju događaje s pogreškama u pogrešci **: Operacijepogreška-SvcErr: došlo je do pogreške u operaciji. Za servis direktorija nije konfiguriran nijedan nadređeni referenca. Imenički servis stoga ne može izdati preporuke objektima izvan ove šume**. Ta se pogreška obično prikazuje ako kontejner servisa Active Directory OU nije pravilno postavljen ili ako postoje problemi s preslikavanjem izraza koji se koristi za **Parentdistinguishednaziv**.

Potvrdite zadani parametar za **nove korisnike** za pogreške u pisanju. Uvjerite se da navedeni OU već postoji u vašem OGLASU. Ako u preslikaču atributa koristite **Parentdistinguishednaziv** , pobrinite se da uvijek bude vredan poznatom kontejneru unutar domene oglasa. Provjerite događaj izvoza u zapisnicima nadzora da biste vidjeli generiranu vrijednost.

Dodatne informacije o konfiguriranju radnog dana za automatiziranu dodjelu resursa potražite u članku [Udžbenik: Konfiguriranje radnog dana za automatsku dodjelu korisnika](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).

