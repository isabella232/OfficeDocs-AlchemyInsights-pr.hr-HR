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
ms.openlocfilehash: 02d79c1b1e112eb41e8c60ffa2ef28e429f76ada
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58304361"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a>Rješavanje problema sa zajedničkim SharePoint sadržaja s vanjskim korisnicima

Provjerite je li za vašu organizaciju uključeno vanjsko zajedničko korištenje:
  
1. Idite na stranicu Dodaci servisa u Centar za administratore okruženja Microsoft 365 pa kliknite [ &amp; Web-mjesta](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns). 
    
2. Provjerite je li postavka uključena u "Uključeno". Ako je odabrano "Samo postojeći vanjski korisnici", provjerite je li vanjski korisnik naveden u Centar za administratore okruženja Microsoft 365.
    
Provjerite je li za web-mjesto uključeno zajedničko korištenje s vanjskim korisnicima. Za klasičnu zbirku web-mjesta:
  
1. U novom centru SharePoint administratora u lijevom oknu kliknite **web-mjesta**.
    
2. Odaberite web-mjesto ili web-mjesta, a zatim na vrpci kliknite **Zajedničko korištenje**.
    
Za timski web-mjesto koje pripada grupi Microsoft 365 ili komunikacijskom web-mjestu:
  
- Te nove vrste web-mjesta imaju istu postavku zajedničkog korištenja kao i postavka na razini tvrtke ili ustanove, osim ako postavka na razini tvrtke ili ustanove omogućuje zajedničko korištenje datoteka pomoću veza koje ne zahtijevaju prijavu. U tom slučaju web-mjesta omogućuju zajedničko korištenje s novim i postojećim vanjskim korisnicima koji se prijave. Da biste promijenili postavku za određena web-mjesta, koristite novi centar za administratore SharePoint PowerShell. [Saznajte više](https://go.microsoft.com/fwlink/?linkid=871863).
    
**Napomena:** postavka vanjskog zajedničkog korištenja za bilo koje web-mjesto može biti restriktivniji od postavki na razini tvrtke ili ustanove, ali ne i više dopuštena od postavke na razini tvrtke ili ustanove. 
  

