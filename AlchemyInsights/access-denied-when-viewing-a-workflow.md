---
title: Pristup je odbijen prilikom gledanja tijeka rada
ms.author: pebaum
author: pebaum
ms.date: 11/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 1cfda8e08ada05858a28f2bede8c31261f9de351
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 12/15/2019
ms.locfileid: "40050517"
---
# <a name="access-denied-when-viewing-a-workflow"></a>Pristup je odbijen prilikom gledanja tijeka rada

SharePoint 2013 tijekovi rada koji pokušaju slanja e-pošte u SharePoint grupu mogu uspjeti s porukom o pogrešci "pristup je odbijen" ako članstvo u SharePoint grupi nije postavljeno na svatko.
  
 **Da biste riješili taj problem, učinite ove korake:**
  
 1. Dopustite svima da vide članove SharePoint grupe.
  
 2. Uklonite SharePoint grupu iz retka do ili kopija e-pošte.
  
 3. Izričito Dodajte korisnike u redak u ili CC ako se vidljivost članstva ne može promijeniti za SharePoint grupu.
  
Da biste pogledali više detalja, molimo pogledajte [http neovlašteno na/_vti_bin/Client.SVC/SP.Utilities.Utility.sendemail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).
  