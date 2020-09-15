---
title: Zajedničko korištenje s vanjskim korisnicima ne funkcionira
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: bd3a6c0d7206801ff76be121c4878b8343cc9886
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47691567"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a>Rješavanje problema s zajedničkim korištenjem sadržaja sustava SharePoint s vanjskim korisnicima

Provjerite je li za vašu tvrtku ili ustanovu uključena vanjsko zajedničko korištenje:
  
1. Idite na [ &amp; stranicu Dodaci servisa u centru za administratore sustava Microsoft 365](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), a zatim kliknite **web-mjesta**.
    
2. Provjerite je li postavka pretvorena u "uključeno". Ako je odabrana mogućnost "samo postojeći vanjski korisnici", provjerite je li vanjski korisnik naveden u centru za administratore sustava Microsoft 365.
    
Provjerite je li vanjsko zajedničko korištenje uključeno za web-mjesto. Za klasičnu zbirku web-mjesta:
  
1. U novom centru za administratore sustava SharePoint u desnom oknu kliknite **web-mjesta**.
    
2. Odaberite web-mjesto ili web-mjesta, a zatim na vrpci kliknite **zajedničko korištenje**.
    
Za timsko web-mjesto koje pripada grupi Microsoft 365 ili komunikacijskom web-mjestu:
  
- Te nove vrste web-mjesta imaju istu postavku zajedničkog korištenja kao postavke za cijelu tvrtku ili ustanovu, osim ako postavka u sklopu tvrtke ili ustanove ne dopušta zajedničko korištenje datoteka pomoću veza koje ne zahtijevaju prijavu. U ovom slučaju web-mjesta omogućuju zajedničko korištenje s novim i postojećim vanjskim korisnicima koji se prijavljuju. Da biste promijenili postavku za određena web-mjesta, koristite novi centar za administratore sustava SharePoint ili PowerShell. [Saznajte više](https://go.microsoft.com/fwlink/?linkid=871863).
    
> [!NOTE]
> Postavka vanjskog zajedničkog korištenja za bilo koje web-mjesto može biti restriktivniji od postavke za cijelu tvrtku ili ustanovu, ali ne i više nego što je postavka u cijelom tvrtki ili ustanovi. 
  

