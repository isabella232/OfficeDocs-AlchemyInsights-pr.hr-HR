---
title: Access denied when viewing a Workflow
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 2b076ec5dca070555ce51b88631fb6bd619ed9269e59ccc799b23b8b95547c16
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53955193"
---
# <a name="access-denied-when-viewing-a-workflow"></a>Access denied when viewing a Workflow

SharePoint tijekovi rada programa 2013 koji pokušaju poslati poruku e-pošte grupi SharePoint ne mogu uspjeti s porukom o pogrešci "Pristup je odbijen" ako članstvo u grupi SharePoint nije postavljeno na Svi.
  
 **Da biste riješili taj problem, učinite sljedeće:**
  
 1. Omogućite svima da vide članove SharePoint grupe.
  
 2. Uklonite grupu SharePoint iz retka Prima ili KOPIJA poruke e-pošte.
  
 3. Eksplicitno dodajte korisnike u redak Prima ili KOPIJA ako se vidljivost članstva ne može promijeniti za SharePoint grupe.
  
Dodatne pojedinosti potražite u članku [HTTP Neovlašteno za /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).
  