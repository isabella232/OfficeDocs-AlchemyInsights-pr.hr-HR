---
title: U centru za sigurnost nije pronađena poruka o pretplatama
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
ms.openlocfilehash: 777fb9b09aa26d166f9971589bda464ccb90f4be
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: HT
ms.contentlocale: hr-HR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52544100"
---
# <a name="no-subscriptions-found-message-in-the-security-center"></a>U centru za sigurnost nije pronađena poruka o pretplatama

Ako prilikom pristupa Microsoft Defender Security Center poruku "Nema pronađenih pretplata", to znači da Azure Active Directory (AAD) koji se koristi za prijavu korisnika na portal nema licencu za Microsoft Defender ATP.  

Licence Windows E5 i Office E5 zasebne su licence.

Otvorite slučaj podrške ako je licenca kupljena, ali nije dodijeljena ovoj instanci AAD-a. Imate sljedeće: <br/>
-   Mogući problem s dodjelom licenci.<br/>
-   Nenamjerno ste licencu dodijeliti microsoftu AAD-u koji se razlikuje od one koja se koristi za provjeru autentičnosti u servis.