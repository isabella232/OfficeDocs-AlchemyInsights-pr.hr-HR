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
ms.openlocfilehash: 285535d6144825f0935bf72579a483260c2f2bd6
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43767241"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a>Rješavanje problema sa zajedničkim korištenjem sadržaja sustava SharePoint s vanjskim korisnicima

Provjerite je li vanjsko zajedničko korištenje uključeno za vašu tvrtku ili ustanovu:
  
1. Idite na [ &amp; stranicu Dodaci za usluge u centru za administratore sustava Microsoft 365](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), a zatim kliknite **Web-mjesta**.
    
2. Provjerite je li postavka uključena u "Uključeno". Ako je odabrano "Samo postojeći vanjski korisnici", provjerite je li vanjski korisnik naveden u centru za administratore sustava Microsoft 365.
    
Provjerite je li vanjsko zajedničko korištenje uključeno za web-mjesto. Za klasičnu zbirku web-mjesta:
  
1. U novom centru za administratore sustava SharePoint u lijevom oknu kliknite **web-mjesta**.
    
2. Odaberite web-mjesto ili web-mjesto, a zatim na vrpci kliknite **Zajedničko korištenje**.
    
Za timsko web-mjesto koje pripada grupi sustava Office 365 ili komunikacijskom web-mjestu:
  
- Te nove vrste web-mjesta imaju istu postavku zajedničkog korištenja kao i postavka na razini tvrtke ili ustanove, osim ako postavka na razini tvrtke ili ustanove dopušta zajedničko korištenje datoteka pomoću veza koje ne zahtijevaju prijavu. U tom slučaju web-mjesta omogućuju zajedničko korištenje s novim i postojećim vanjskim korisnicima koji se prijavljuju. Da biste promijenili postavku za određena web-mjesta, koristite novi centar za administratore sustava SharePoint ili PowerShell. [Saznajte više](https://go.microsoft.com/fwlink/?linkid=871863).
    
> [!NOTE]
> Postavka vanjskog zajedničkog korištenja za bilo koje web-mjesto može biti restriktivnija od postavke na razini tvrtke ili ustanove, ali ne i popustljivija od postavke na razini organizacije. 
  

