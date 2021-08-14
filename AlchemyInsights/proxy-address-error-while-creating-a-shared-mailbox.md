---
title: Pogreška proxy adrese prilikom stvaranja zajedničkog poštanskog sandučića
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
ms.openlocfilehash: 7c15d5db5445fbe4c3ec22878f180f48d2da4f90369f2e6f223916646eb19c12
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54062900"
---
# <a name="proxy-address-error-while-creating-a-mailbox-or-other-email-enabled-object"></a>Pogreška proxy adrese prilikom stvaranja poštanskog sandučića ili nekog drugog objekta s omogućenom e-poštom

Ako ste pokušali stvoriti objekt s omogućenom e-poštom (poštanski sandučić, zajednički poštanski sandučić itd.) i primili ste pogrešku "Proxy adresa "SMTP:alias@domain.com" već se koristi...", adresu e-pošte koju ste odabrali već je preuzeo drugi objekt s omogućenom e-poštom u vašoj tvrtki ili ustanovi.
  
Morate pronaći korisnika, grupu, zajednički poštanski sandučić ili javnu mapu s tom adresom e-pošte i izbrisati je ili promijeniti njezinu adresu e-pošte. Zatim možete stvoriti novi objekt s omogućenom e-poštom s besplatnom adresom e-pošte. Pronađite ga pomoću pretraživanja na početnoj stranici. Da biste je potražili, možete Exchange Online sljedeću naredbu komponente PowerShell:

`
    Get-EXORecipient -Filter "EmailAddresses -eq 'email@contoso.onmicrosoft.com'"
`
  
Ako ne želite izbrisati postojeću adresu e-pošte, odaberite novu adresu e-pošte za novi objekt koji stvarate.
  