---
title: 646 kako konfigurirati AADConnect
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: dd6d6986b23c8adcc98fe713bacf32fb5bf8b4b6
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 02/12/2019
ms.locfileid: "29915556"
---
# <a name="configure-sync-features"></a>Konfiguriranje značajke sinkronizacije

Povezivanje Azure AD uključuje nekoliko značajki koje su omogućena po zadanom ili koje kasnije možete omogućiti. Neke značajke zahtijevaju dodatnu konfiguraciju u određenim okruženjima.
  
- [Filtriranje](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) ograničenja objekata se sinkroniziraju Azure AD. Po zadanom, sve korisnici, kontakti, grupe i Windows 10 sinkroniziraju se računi na računalu. Možete uključiti ili isključiti na temelju domene, organizacijske jedinice ili druge atribute objekata. 
    
- [Lozinka raspršivanja sinkronizacije](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) sinkronizira raspršivanja lozinku iz lokalno servisa Active Directory za Azure AD. To omogućuje upravljanje lozinkom na jedno mjesto, ali koristi istu lozinku u oba lokalno i oblak okruženjima. Jer je Active Directory mjerodavne izvora, možete koristiti vlastite pravila lozinke. 
    
- [(SSPR) za vraćanje izvorne lozinke samoposlužno](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) omogućava korisnicima da Vrati svoje vlastite lozinke oblak dok još uvijek se primjenjuju pravila za lozinke lokalno. 
    
- [Writeback uređaj](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) dopušta registrirani uređaji u Azure AD budu napisani natrag na lokalno Active Directory pa se može koristiti za uvjetno pristup. 
    
- [Briše spriječi slučajnog](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) po zadanom je omogućena za sprečavanje brisanja previše istodobnih objekt (više od 500 objekata po sinkronizacije). Možete promijeniti ovu postavku potrebama vaše organizacije. 
    
- [Automatske nadogradnje](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) omogućena je po zadanom express instalacijama i osigurava vaša verzija Azure AD povezivanje uvijek je trenutni. 
    

