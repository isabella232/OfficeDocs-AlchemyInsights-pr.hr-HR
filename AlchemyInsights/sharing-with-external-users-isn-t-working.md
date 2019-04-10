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
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 69e290e5a13f40ad045086791189a7d0af88240b
ms.sourcegitcommit: 228c986911ecf73217116a5d1fdcd2e89362774e
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/09/2019
ms.locfileid: "31747590"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a>Riješite probleme s vanjskim korisnicima dijeljenje SharePoint sadržaja

Provjerite je li vanjski je uključeno zajedničko korištenje vaše organizacije:
  
1. Idite na [Services &amp; stranici dodaci u centru za administraciju Microsoft 365](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), i kliknite **mjesta**.
    
2. Provjerite je li postavka uključena za "Na." Ako odabrano je "Samo postojeće vanjski korisnici", provjerite vanjskog korisnika navedene u centru za administraciju Microsoft 365.
    
Provjerite vanjske dijeljenja uključen za web-mjesto. Klasični zbirke stranica:
  
1. Novi centar admin SharePoint, u lijevom oknu kliknite **mjesta**.
    
2. Odaberite web-mjesta ili web-mjesta i na vrpci kliknite **zajedničko korištenje**.
    
Za web-mjesto tima koji pripada grupi Office 365 ili komunikacije web-mjesta:
  
- Ove nove vrste web-mjesta imaju na isti zajedničko korištenje postavljanje kao postavku nivou organizacije, osim ako postavka nivou organizacije omogućuje zajedničko korištenje datoteka pomoću veze koje ne zahtijevaju prijavu. U tom slučaju web-mjesta Dopusti zajedničko korištenje nove i postojeće vanjski korisnici koji se prijaviti. Da biste promijenili postavke za određena web-mjesta, koristite novi SharePoint administraciju centar ili PowerShell. [Saznajte više](https://go.microsoft.com/fwlink/?linkid=871863).
    
> [!NOTE]
> Vanjski zajedničko korištenje postavka za bilo koje web-mjesto može biti šira od postavku nivou organizacije, ali ne više čemu od postavke nivou organizacije. 
  

