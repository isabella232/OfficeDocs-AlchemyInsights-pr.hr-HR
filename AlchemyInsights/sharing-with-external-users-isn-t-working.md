---
title: Zajedničko korištenje s vanjskim korisnicima ne radi
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 5/18/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 20b538846997c021b6e88596a1e8aff401ea935b
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 02/12/2019
ms.locfileid: "29900856"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a>Riješite probleme s vanjskim korisnicima dijeljenje SharePoint sadržaja

Provjerite je li vanjski je uključeno zajedničko korištenje vaše organizacije:
  
1. Idite na [Services &amp; stranicu dodaci u centru za administraciju sistema Office 365](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), i kliknite **mjesta**.
    
2. Provjerite je li postavka uključena za "Na." Ako odabrano je "Samo postojeće vanjski korisnici", provjerite vanjskog korisnika navedene u centru za administraciju sistema Office 365.
    
Provjerite vanjske dijeljenja uključen za web-mjesto. Klasični zbirke stranica:
  
1. Klasični center admin SharePoint, u lijevom oknu kliknite **zbirki web-mjesta**.
    
2. Odaberite web-mjesta ili web-mjesta i na vrpci kliknite **zajedničko korištenje**.
    
Za web-mjesto tima koji pripada grupi Office 365 ili komunikacije web-mjesta:
  
- Ove nove vrste web-mjesta imaju na isti zajedničko korištenje postavljanje kao postavku nivou organizacije, osim ako postavka nivou organizacije omogućuje zajedničko korištenje datoteka pomoću veze koje ne zahtijevaju prijavu. U tom slučaju web-mjesta Dopusti zajedničko korištenje nove i postojeće vanjski korisnici koji se prijaviti. Da biste promijenili postavke za određena web-mjesta, koristite novi SharePoint administraciju centar (pretpregled) ili PowerShell. [Saznajte više](https://go.microsoft.com/fwlink/?linkid=871863).
    
> [!NOTE]
> Vanjski zajedničko korištenje postavka za bilo koje web-mjesto može biti šira od postavku nivou organizacije, ali ne više čemu od postavke nivou organizacije. 
  

