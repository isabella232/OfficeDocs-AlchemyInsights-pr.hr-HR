---
title: Otklanjanje poteškoća s sinkronizacijom lozinke
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
ms.openlocfilehash: 96f63f2ae8e5de246bce7fc15a9b2c3d604f2eb8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664918"
---
# <a name="troubleshoot-password-synchronization"></a>Otklanjanje poteškoća s sinkronizacijom lozinke

Da biste otklonili poteškoće s sinkronizacijom lozinki, započnite pomoću tog zadatka AAD Connect otklanjanje poteškoća da biste utvrdili zašto se lozinke ne sinkroniziraju. Da biste započeli, otvorite [Upravljanje izravnim sinkronizacijom](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).  

1. Otvorite novu sesiju komponente Windows PowerShell na poslužitelju Azure AD Connect, a zatim odaberite mogućnost **Pokreni kao administrator** .

2. Pokretanje pravilnika za Remotepotpisana ili skupa izvršnih pravila za postavljanje pogubljenja

3. Pokrenite čarobnjak za Azure AD Connect.

4. Idite na stranicu dodatni zadaci > **Otklanjanje poteškoća**  >  **dalje**.

5. Odaberite **Pokreni** da biste otvorili izbornik otklanjanja poteškoća sa pomoću komponente PowerShell.

6. Odaberite **Otklanjanje poteškoća s sinkronizacijom lozinke**.

    Problem je obično što lozinka nije sinkronizirana za određeni korisnički račun.

    **Bilješke** Sinkronizacija lozinke neće uspjeti ako je posljednja uspješna sinkronizacija lozinki bila prije nekog vremena.

Dodatne informacije o otklanjanju poteškoća s sinkronizacijom lozinke potražite [u članku Otklanjanje poteškoća s sinkronizacijom lozinke uz sinkronizaciju servisa Azure ad Connect](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).