---
title: Nije moguće postaviti ili prikazati pravilnik AllowSelfServicePurchase
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: 255dbe35b808b3fe6b5707779251bf3f4a7e1c269c8b6f0ac2cb43ca03c469e9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54020184"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a>Nije moguće postaviti ili prikazati pravilnik AllowSelfServicePurchase

Kada pokušate postaviti ili prikazati pravilnik AllowSelfServicePurchase, primit ćete sljedeću poruku o pogrešci:

*HandleError : Nije uspjelo dohvaćanje pravilnika o proizvodu uz PolicyId 'AllowSelfServicePurchase', ErrorMessage – veza u podlozi je zatvorena: došlo je do neočekivane pogreške prilikom slanja.*

To može biti zbog starije verzije sigurnosti transportnog sloja (TLS). Da biste povezali servis MSCommerce, morate koristiti TLS 1.2 ili noviji.  

Isprobajte sljedeće korake da biste omogućili/postavili TLS protokol na 1.2, potvrdili i ponovno pokušali.
 1. U naredbeni redak komponente PowerShell (PS C: unesite sljedeću naredbu da biste \) protokol TLS postavili na verziju 1.2:

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. Provjerite protokole TLS koji se koriste pomoću sljedeće naredbe:

    `[Net.ServicePointManager]::SecurityProtocol` 

3. Po potrebi ponovno pokušajte s naredbama Get or Update.

