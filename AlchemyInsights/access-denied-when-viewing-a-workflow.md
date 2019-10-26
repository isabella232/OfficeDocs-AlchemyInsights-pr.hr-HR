---
title: Pristup je odbijen prilikom gledanja tijeka rada
ms.author: pebaum
author: Techwriter40
ms.date: 11/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 4ca65583fbd98867026e9e3cc8f36fe38798aa85
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 10/25/2019
ms.locfileid: "36747740"
---
# <a name="access-denied-when-viewing-a-workflow"></a>Pristup je odbijen prilikom gledanja tijeka rada

SharePoint 2013 tijekovi rada koji pokušaju slanja e-pošte u SharePoint grupu mogu uspjeti s porukom o pogrešci "pristup je odbijen" ako članstvo u SharePoint grupi nije postavljeno na svatko.
  
 **Da biste riješili taj problem, učinite ove korake:**
  
 1. Dopustite svima da vide članove SharePoint grupe.
  
 2. Uklonite SharePoint grupu iz retka do ili kopija e-pošte.
  
 3. Izričito Dodajte korisnike u redak u ili CC ako se vidljivost članstva ne može promijeniti za SharePoint grupu.
  
Za prikaz više detalja molimo pogledajte [http neovlašteno na/_vti_bin/Client.SVC/SP.Utilities.Utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).
  