---
title: Dijeljenje s vanjskim korisnicima ne radi
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 5/18/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: d4c8fc75ff8db2319b88a20bea9b3ee661f2e36e
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 10/18/2019
ms.locfileid: "36502223"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a>Rješavanje problema s dijeljenjem SharePointovog sadržaja s vanjskim korisnicima

Provjerite je li vanjsko zajedničko korištenje uključeno za vašu organizaciju:
  
1. Idite na [stranicu dodataka &amp; za usluge u centru za administraciju Microsoft 365](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)i kliknite **web-mjesta**.
    
2. Provjerite je li postavka uključena u "uključeno". Ako je odabran "samo postojeći vanjski korisnici", provjerite je li vanjski korisnik naveden u centru za administraciju Microsoft 365.
    
Provjerite je li vanjsko dijeljenje uključeno za web-mjesto. Za klasičnu zbirku web-mjesta:
  
1. U novom centru za administraciju sustava SharePoint u lijevom oknu kliknite **web-mjesta**.
    
2. Odaberite web-mjesto ili web-mjesta, a zatim na vrpci kliknite **dijeljenje**.
    
Za timsko web-mjesto koje pripada grupi sustava Office 365 ili web-mjestu za komunikaciju:
  
- Te nove vrste web-mjesta imaju jednaku postavku dijeljenja kao i postavku za vašu organizaciju, osim ako postavka na razini organizacije omogućuje dijeljenje datoteka pomoću veza koje ne zahtijevaju prijavu. U tom slučaju web-mjesta dopuštaju dijeljenje s novim i postojećim vanjskim korisnicima koji se prijave. Da biste promijenili postavku za određena web-mjesta, upotrijebite novi centar za administraciju sustava SharePoint ili PowerShell. [Saznajte više](https://go.microsoft.com/fwlink/?linkid=871863).
    
> [!NOTE]
> Postavka vanjskog dijeljenja za bilo koje web-mjesto može biti restriktivnija od postavke u cijeloj organizaciji, ali ne više popustljiva od postavke u cijeloj organizaciji. 
  

