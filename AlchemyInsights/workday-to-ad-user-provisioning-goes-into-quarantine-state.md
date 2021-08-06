---
title: Radni dan u ad user provisioning ulazi u stanje karantene
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
ms.openlocfilehash: 32a5d010b95b9587e121ca1526def743fd8f371b13d1d73d3578c692839edf19
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54036484"
---
# <a name="workday-to-ad-user-provisioning-goes-into-quarantine-state"></a>Radni dan u ad user provisioning ulazi u stanje karantene

**Radno vrijeme za dodjeljivanje resursa korisnika u AD-u ulazi u stanje karantene i u AD-u se ne stvaraju korisnici**

Zadatak dodjele resursa korisnika za Radni dan u AD-u otišao je u stanje karantene, a zapisnici nadzora prikazuju događaje neuspješnog izvoza s porukom o pogrešci **Pogreška: OperationsError-SvcErr: došlo je do pogreške u operaciji. Za imenički servis nije konfigurirana nadređena referenca. Imenički servis stoga ne može izdavati preporuke objektima izvan ove šume**. Ta se pogreška obično prikazuje ako OU spremnika servisa Active Directory nije pravilno postavljen ili ako postoje problemi s mapiranjem izraza koji se koristi za **nadređeniOdaziv.**

U parametru Zadani OU za nove korisnike provjerite **ima li** pogrešaka u pisanju. Provjerite postoji li navedeni OU već u vašem AD-u. Ako u **mapiranju atributa koristite parentDistinguishedName,** provjerite je li uvijek vrednovan u poznati spremnik unutar ad domene. Provjerite događaj Izvoz u zapisnicima nadzora da biste vidjeli generiranu vrijednost.

Dodatne informacije o konfiguriranju radnog dana za automatizirano dodjeljivanje resursa potražite u članku [Vodič: Konfiguriranje radnog dana za automatsko dodjeljivanje resursa korisnicima.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)

