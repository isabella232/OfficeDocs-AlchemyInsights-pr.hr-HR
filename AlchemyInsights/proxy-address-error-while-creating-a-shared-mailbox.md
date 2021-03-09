---
title: Pogreška Proxy adrese prilikom stvaranja zajedničkog poštanskog sandučića
ms.author: pebaum
author: CrystalThomasMS
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ece4bcce-1053-4ed3-a194-9d0af8f73c6f
ms.custom:
- "19"
- "6"
ms.openlocfilehash: ab491e883ab294f08d0b5d2e686dc059b468d29f
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/09/2021
ms.locfileid: "50568282"
---
# <a name="proxy-address-error-while-creating-a-mailbox-or-other-email-enabled-object"></a>Pogreška Proxy adrese prilikom stvaranja poštanskog sandučića ili drugog objekta koji je omogućen za e-poštu

Ako ste pokušali stvoriti objekt omogućen za e-poštu (poštanski sandučić, zajednički poštanski sandučić itd.) i primili pogrešku "proxy adresa" SMTP:alias@domain.com "već se koristi...", adresa e-pošte koju ste odabrali već je uzeo neki drugi objekt omogućen za e-poštu u vašoj tvrtki ili ustanovi.
  
Morate pronaći korisnika, grupu, zajednički poštanski sandučić ili javnu mapu koja sadrži ovu adresu e-pošte i izbrisati je ili promijeniti adresu e-pošte. Zatim možete stvoriti novi objekt omogućen za e-poštu s oslobođenom adresom e-pošte. Pronađite ga pomoću pretraživanja na početnoj stranici. Da biste ga potražili, možete koristiti i sljedeću naredbu sustava Exchange Online PowerShell:

`
    Get-EXORecipient -Filter "EmailAddresses -eq 'email@contoso.onmicrosoft.com'"
`
  
Ako ne želite izbrisati postojeću adresu e-pošte, odaberite novu adresu e-pošte za novi objekt koji stvarate.
  