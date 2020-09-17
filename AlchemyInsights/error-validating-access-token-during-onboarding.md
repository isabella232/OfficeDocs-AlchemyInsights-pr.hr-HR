---
title: Došlo je do pogreške prilikom provjere pogrešaka programa Access token tijekom radne površine u analitici na dasci
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2536"
- "9000657"
ms.openlocfilehash: 45c6fb1a1632799a07c028c0791b6b8e77635293
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47783543"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a>"Došlo je do pogreške pri provjeri valjanosti programa Access token" prilikom korištenja analitičkih podataka za stolna računala

Ta se pogreška obično primjećuje kada istekne token za provjeru autentičnosti. Obično osvježavanjem stranice osvježava token. Međutim, taj problem može biti ustrajan ako postoje pravila uvjetnog pristupa koja se primjenjuju na račun koji se koristi za analitičke radne površine. Prijavite se u zapisnicima za Azure AD na portalu Azure da biste vidjeli postoje li neuspjele prijave za račun koji se koristi za analitiku za stolna računala.

Dodatne informacije o uvjetnom pristupu potražite u odjeljku [Planiranje implementacije uvjetnog pristupanja](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).