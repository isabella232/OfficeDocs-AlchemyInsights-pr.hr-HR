---
title: Prepoznavanje aktivnosti pravila ulazne pošte u zapisnicima nadzora
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 1f252836d624b4550e1f3c87cf4fd7309dec6e91
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58331115"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a>Prepoznavanje aktivnosti pravila ulazne pošte u zapisnicima nadzora

Pretraživanje zapisnika nadzora možete koristiti u Centar za usklađenost okruženja Microsoft 365 za prikaz događaja pravila ulazne pošte (stvaranje, izmjena i brisanje pravila ulazne pošte).

1. Učinite nešto od sljedećeg:
   - U Centar za usklađenost okruženja Microsoft 365 na <https://compliance.microsoft.com> idite na **Nadzor** \> **rješenja**. Možete i izravno pristupiti stranici **Nadzor** pomoću sustava <https://compliance.microsoft.com/auditlogsearch> .
   - Na portalu Microsoft 365 Defender idite <https://security.microsoft.com> na **Nadzor**. Možete i izravno pristupiti stranici **Nadzor** pomoću sustava <https://security.microsoft.com/auditlogsearch> .

2. Na kartici **Pretraživanje** na **stranici Nadzor** konfigurirajte sljedeće postavke:
   - **Raspon datuma i vremena:** odaberite raspon datuma/vremena u **okvirima Početak** **i** Kraj.
   - **Aktivnosti**: odaberite jednu ili više sljedećih vrijednosti:
     - **Novo-ulazna poštaRule Stvori pravilo ulazne pošte iz Outlook Web App**
     - **Pravilo za promjenu postavki ulazne pošte iz Outlook Web App**.
     - **Ažuriranje pravila ulazne pošte iz Outlook klijenta**

3. Kada završite, kliknite **Pretraživanje**. Aktivnosti se prikazuju na novoj stranici **pretraživanja nadzora.**

4. Odaberite aktivnost u rezultatima da biste otvorili letak s detaljima. Informacije o postavkama pravila ulazne pošte prikazuju se u **polju** Parametri.

Dodatne informacije potražite u članku [Utvrđivanje je li korisnik stvorio pravilo ulazne pošte](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-created-an-inbox-rule).
