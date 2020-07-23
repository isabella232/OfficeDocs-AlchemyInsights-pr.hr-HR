---
title: Rješavanje problema sa sinkronizacijom lozinkom
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 54b5a033b7cbb99520425b31800364ed4a99a4e6
ms.sourcegitcommit: 1d01b8b48eef2d5d10c375dcf802cd36e9d6bf61
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 07/23/2020
ms.locfileid: "45387869"
---
# <a name="troubleshoot-password-synchronization"></a>Rješavanje problema sa sinkronizacijom lozinkom

Da biste otklonili poteškoće sa sinkronizacijom lozinkom, pokrenite ovaj zadatak za otklanjanje poteškoća s AAD Connectom da biste odredili zašto se lozinke ne sinkroniziraju. Da biste započeli, idite na [Upravljanje izravnom sinkronizacijom](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).  

1. Otvorite novu sesiju komponente Windows PowerShell na poslužitelju Azure AD Connect i odaberite mogućnost **Pokreni kao administrator.**

2. Pokrenite Set-ExecutionPolicy RemoteSigned ili Set-ExecutionPolicy neograničeno.

3. Pokrenite čarobnjak za Azure AD Connect.

4. Idite na stranicu Dodatni zadaci > **Otklanjanje poteškoća**  >  **Sljedeće**.

5. Odaberite **Pokreni** da biste otvorili izbornik za otklanjanje poteškoća sa ljuskom PowerShell.

6. Odaberite **Otklanjanje poteškoća sa sinkronizacijom lozinke**.

    Problem je obično u tome što lozinka nije sinkronizirana za određeni korisnički račun.

    **Bilješke** Sinkronizacija lozinkom ne uspijeva ako je posljednja uspješna sinkronizacija lozinke bila prije nekog vremena.

Dodatna pomoć za otklanjanje poteškoća sa sinkronizacijom [lozinkom potražite u članku Otklanjanje poteškoća sa sinkronizacijom raspršilim lozinkom sa sinkronizacijom azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).