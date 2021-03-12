---
title: U centru za sigurnost nije pronađena nijedna pretplata
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6028"
- "9001222"
ms.openlocfilehash: 01117bc535df14533e426fd2d31c336fccc75611
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/15/2020
ms.locfileid: "50713338"
---
# <a name="no-subscriptions-found-message-in-the-security-center"></a>U centru za sigurnost nije pronađena nijedna pretplata

Ako prilikom pristupanja centru za sigurnost programa Microsoft Defender dobijete poruku "nije pronađena pretplata", to znači da je Azure Active Directory (AAD) koji se koristi za prijavu korisnika na portal nema licencu za Microsoft Defender ATP.  

Licence za Windows E5 i Office E5 zasebne su licence.

Otvorite slučaj podrške ako je licenca kupljena, ali nije dodijeljena ovoj instanci AAD-a. Ili imate sljedeće: <br/>
-   Mogući problem dodjele licenci.<br/>
-   Nehotice ste dodijelili licencu drugim Microsoftovim AAD-ju od one koja se koristi za provjeru autentičnosti u servisu.