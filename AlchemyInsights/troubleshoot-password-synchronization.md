---
title: Otklanjanje poteškoća sa sinkronizacijom lozinke
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: cb782c0d1dc396ee7a9f016afb9629a2cdee93d52f5408b7a73e576e783ebc0a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54105740"
---
# <a name="troubleshoot-password-synchronization"></a>Otklanjanje poteškoća sa sinkronizacijom lozinke

Da biste otklonili poteškoće sa sinkronizacijom lozinke, počnite pomoću ovog zadatka za Povezivanje otklanjanje poteškoća da biste utvrdili zašto se lozinke ne sinkroniziraju. Da biste počeli, idite na [Upravljanje izravnom sinkronizacijom](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).  

1. Otvorite novu Windows PowerShell na poslužitelju servisa Azure AD Povezivanje pa odaberite mogućnost **Pokreni kao administrator.**

2. Pokrenite Set-ExecutionPolicy RemoteSigned ili Set-ExecutionPolicy Unrestricted.

3. Pokrenite čarobnjak za Azure AD Povezivanje.

4. Idite na stranicu Dodatni zadaci > Otklanjanje **poteškoća** sa  >  **značajkom Dalje**.

5. Odaberite **Pokreni** da biste otvorili izbornik otklanjanje poteškoća komponente PowerShell.

6. Odaberite **Otklanjanje poteškoća sa sinkronizacijom lozinke**.

    Problem je u tome što se lozinka obično ne sinkronizira za određeni korisnički račun.

    **Bilješke** Sinkronizacija lozinke ne uspijeva ako je zadnja uspješna sinkronizacija lozinke bila prije nekog vremena.

Dodatne informacije o otklanjanju poteškoća sa sinkronizacijom lozinke potražite u članku Otklanjanje poteškoća sa sinkronizacijom [hasha lozinke pomoću servisa Azure AD Povezivanje sinkronizacije](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).