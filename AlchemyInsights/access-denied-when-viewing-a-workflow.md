---
title: Pristup odbijen kada gledate tijeka rada
ms.author: kirks
author: Techwriter40
ms.date: 11/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: cced887b03876eef527e0166a5a3c9be4b553029
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29461772"
---
# <a name="access-denied-when-viewing-a-workflow"></a>Pristup odbijen kada gledate tijeka rada

SharePoint 2013 tijekovi rada pokušati poslati poruku e-pošte SharePoint grupi može uspjeti s poruku o pogrešci "Pristup je odbijen" ako članstva SharePoint grupe ne postavite svima.
  
 **Da biste riješili taj problem, učinite sljedeće korake:**
  
 1. Dopusti svima da biste vidjeli članovi SharePoint grupe. 
  
 2. Uklonite SharePoint grupu iz Prima ili Kopija redak e-pošte. 
  
 3. Izričito dodati korisnike da Prima ili Kopija redak ako vidljivost članstva ne može promijeniti za SharePoint grupu. 
  
Za prikaz više pojedinosti pogledajte [HTTP neovlašteno za /_vti_bin/client.svc/sp.utilities.utility.SendEmail ](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).
  

