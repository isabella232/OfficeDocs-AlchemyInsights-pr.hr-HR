---
title: Zajedničko korištenje s vanjskim korisnicima ne funkcionira
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 9a40f52637bc8aa7894754118f0f862aa6c71fe2
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582767"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a>Rješavanje problema sa zajedničkim korištenjem sadržaja sustava SharePoint s vanjskim korisnicima

Provjerite je li vanjsko zajedničko korištenje uključeno za vašu tvrtku ili ustanovu:
  
1. Otvorite [stranicu dodaci za &amp; servise u centru za administratore sustava Microsoft 365](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), a zatim kliknite **Web- mjesta**.
    
2. Provjerite je li postavka uključena u "Uključeno". Ako je odabrana mogućnost "Samo postojeći vanjski korisnici", provjerite je li vanjski korisnik naveden u centru za administratore sustava Microsoft 365.
    
Provjerite je li vanjsko zajedničko korištenje uključeno za web-mjesto. Za klasičnu zbirku web-mjesta:
  
1. U novom centru za administratore sustava SharePoint u lijevom oknu kliknite **web-mjesta**.
    
2. Odaberite web-mjesto ili web-mjesta, a zatim na vrpci kliknite **Zajedničko korištenje**.
    
Za timsko web-mjesto koje pripada grupi Microsoft 365 ili komunikacijskom web-mjestu:
  
- Te nove vrste web-mjesta imaju istu postavku zajedničkog korištenja kao postavka na razini tvrtke ili ustanove, osim ako postavka na razini tvrtke ili ustanove omogućuje zajedničko korištenje datoteka pomoću veza koje ne zahtijevaju prijavu. U tom slučaju web-mjesta dopuštaju zajedničko korištenje s novim i postojećim vanjskim korisnicima koji se prijavljuju. Da biste promijenili postavku za određena web-mjesta, koristite novi centar za administratore sustava SharePoint ili PowerShell. [Saznajte više](https://go.microsoft.com/fwlink/?linkid=871863).
    
> [!NOTE]
> Postavka vanjskog zajedničkog korištenja za bilo koje web-mjesto može biti restriktivnija od postavke na razini vaše organizacije, ali ne i popustljivija od postavke na razini tvrtke ili ustanove. 
  

