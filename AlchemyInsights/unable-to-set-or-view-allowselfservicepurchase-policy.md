---
title: Nije moguće postaviti ili pregledati pravila AllowSelfServicePurchase
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: 587a05cccbc71a970d4bd7723bff0df0c3b64ccc
ms.sourcegitcommit: 2a9d059262c07c33f9a740b3da4e6e3366b2f925
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 02/20/2020
ms.locfileid: "42158553"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a>Nije moguće postaviti ili pregledati pravila AllowSelfServicePurchase

Prilikom pokušaja postavljanja ili prikaza pravila AllowSelfServicePurchase dobivate sljedeću poruku o pogrešci:

*HandleError : Dohvaćanje pravila proizvoda s Pravilima Id 'AllowSelfServicePurchase', ErrorMessage - Veza u podlozi je zatvorena: Došlo je do neočekivane pogreške prilikom slanja.*

To može biti zbog starije verzije Transport Layer Security (TLS). Da biste povezali uslugu MSCommerce, morate koristiti TLS 1.2 ili noviji.  

Pokušajte sljedeće korake da biste omogućili/postavili TLS protokol na 1.2, provjerili i ponovno pokušali.
 1. U naredbeni redak PowerShell\) (PS C: unesite sljedeću naredbu da biste TLS protokol postavili na verziju 1.2:

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. Provjerite TLS protokole koji se koriste pomoću sljedeće naredbe:

    `[Net.ServicePointManager]::SecurityProtocol` 

3. Po potrebi ponovno pokušajte naredbe Get or Update.

