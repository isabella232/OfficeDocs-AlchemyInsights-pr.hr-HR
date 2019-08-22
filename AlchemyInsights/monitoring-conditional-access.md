---
title: Nadzor uvjetno pristup
ms.author: pebaum
author: pebaum
ms.date: 8/1/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 374814f4eabd61433a15876ebf7f351819933c21
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36538733"
---
# <a name="monitoring-conditional-access-for-exchange"></a>Nadzor uvjetno pristup za Exchange

Ciljane uvjetno access korisnici će primiti obavijest e-pošte ako ne udovoljava zahtjevima pristupa vašoj organizaciji. Da biste riješili, preporučujemo da jedno ili više od sljedećih rješenja:
  
- Ako uređaj presumed da se upisani, savjeta korisnik Idi na Portal tvrtke app i provjerite pojavljuje se Portal tvrtke. Ako ne, korisnik treba uvrstili uređaj.
    
- Azure portal idite na **Intune \> usklađenosti uređaj**. Ispod **monitora** kliknite **uređaj usklađenosti**. Prikaz izvještaja usklađenosti uređaj da biste provjerili korisnički uređaj je označena kao sa standardom. 
    
- Azure portal idite na **Intune \> usklađenosti uređaj**. U odjeljku **Upravljanje**kliknite **pravila**. Na popisu pravila usklađenosti provjerite profil je dodijeljena svoj korisnički uređaj. Ako je dodijeljen nijedan profil, zatim Intune nećete moći potvrditi statusom usklađenosti na uređaj. 
    
- Uređivanje korisnika uvjetno access dodjele.
    
1. Azure portal idite na **Intune \> uvjetno access \> pravila**
    
2. Odaberite pravilo s popisa
    
3. Kliknite **korisnici i grupe**
    
4. Ciljne određena pravila na netko, dodajte ih na popis za **Uvrštavanje** . Da biste osigurali osoba izostavljen iz pravila, dodajte ih na popis za **izostavljanje** . 
    
Pročitajte više: [Kako Access uvjetno Monitor uređaji](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)
  

