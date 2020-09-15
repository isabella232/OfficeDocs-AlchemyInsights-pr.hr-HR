---
title: Otklanjanje poteškoća s zabranom pristupa porukama
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: f49cfc50142b3d98a5f431a38e9a943eb5624523
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47691675"
---
# <a name="troubleshoot-access-denied-messages"></a>Otklanjanje poteškoća s zabranom pristupa porukama

Ako prilikom pokušaja pregledavanja web-mjesta sustava SharePoint Online primate poruku o uskraćenog pristupa, pročitajte članak u nastavku.

**Dodavanje i licenciranje korisnika**

Provjerite jeste li [korisnicima dodijelili licence u programu Microsoft 365 za tvrtke](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).

**Dodjela dozvola**

Ako je korisniku dodijeljena licenca za SharePoint i još uvijek dobiva poruku o uskraćenom pristupu, provjerite ima li [dodijeljenu odgovarajuću razinu dozvola](https://docs.microsoft.com/sharepoint/understanding-permission-levels).

**Razmislite o korištenju značajke zahtjeva za Access**

Značajka [zahtjeva za pristup](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) omogućuje korisnicima da zatraže pristup sadržaju koji trenutno nemaju dozvolu za pregled. 

**Omogućivanje prilagođene skripte može uzrokovati probleme s uskraćanjem programa Access**

Postoje određeni scenariji u kojima značajka "Dopusti prilagođenu skriptu" možda predstavlja zabranjen pristup. Popis značajki koje su zahvaćene sigurnosnim razmišljanjima i mogućnost onemogućivanja značajke. Posjetite, [omogućite ili onemogućite prilagođenu skriptu](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

Pažnja: Ako web-mjesto servisa OneDrive ili SharePoint nije dostupno većem broju korisnika koji su prethodno imali pristup, možda postoji privremeni problem s servisom. [Provjerite nadzornu ploču zdravstvenog stanja servisa](https://portal.office.com/adminportal/home#/servicehealth).


  

