---
title: Pristup je odbijen prilikom pregledavanja tijeka rada
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: c576bf88225582f2577e0b59506a7482cf9f38d5
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43687322"
---
# <a name="access-denied-when-viewing-a-workflow"></a>Pristup je odbijen prilikom pregledavanja tijeka rada

Tijekovi rada sustava SharePoint 2013 koji pokušaju slanja e-pošte sharepoint grupi možda neće uspjeti s porukom o pogrešci "Pristup je odbijen" ako članstvo u sharepoint grupi nije postavljeno na Svi.
  
 **Da biste riješili taj problem, učinite sljedeće:**
  
 1. Dopustite svima da vide članove SharePoint grupe.
  
 2. Uklonite sharepoint grupu iz retka Prima ili KOPIJA e-pošte.
  
 3. Eksplicitno dodajte korisnike u redak Prima ili KOPIJA ako se vidljivost članstva ne može promijeniti za SharePoint grupu.
  
Da biste vidjeli više detalja, pogledajte [HTTP Neovlašteno na /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).
  