---
title: Pristup je odbijen prilikom pregledavanja tijeka rada
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 710775e8b2dee98969df7a4c8410a3e61181aaf6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47688794"
---
# <a name="access-denied-when-viewing-a-workflow"></a>Pristup je odbijen prilikom pregledavanja tijeka rada

Tijekovi rada sustava SharePoint 2013 koji pokušaju poslati poruku e-pošte u grupu sustava SharePoint ne uspijevaju s porukom o pogrešci "Access denied" ako članstvo u grupi sustava SharePoint nije postavljeno na sve.
  
 **Da biste riješili taj problem, učinite sljedeće:**
  
 1. Dopusti svima da vide članove grupe sustava SharePoint.
  
 2. Uklonite grupu sustava SharePoint iz retka prima ili kopija poruke e-pošte.
  
 3. Eksplicitno Dodajte korisnike u redak Prima ili kopija ako se vidljivost članstva ne može promijeniti za grupu sustava SharePoint.
  
Da biste pogledali više detalja, pogledajte [http neovlašten za/_vti_bin/Client.SVC/SP.Utilities.Utility.sendemail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).
  