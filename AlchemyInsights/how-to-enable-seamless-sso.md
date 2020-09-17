---
title: Omogućivanje bešavnih SSO-a
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
- "628"
- "1300012"
ms.assetid: 80c88b2d-adb1-4e45-8eff-aaa80403b5b6
ms.openlocfilehash: f3581549823e1ec650a3717780bc07e9944d4c1c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47780519"
---
# <a name="how-to-enable-seamless-sso"></a>Omogućivanje bešavnih SSO-a

Omogućite bešavne SSO putem servisa [Azure ad Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect).
  
Ako koristite svježu instalaciju servisa Azure AD Connect, odaberite [prilagođeni put za instalaciju](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-get-started-custom). Na stranici **korisnik za prijavu** odaberite mogućnost **Omogući jedinstvenu prijavu** .
  
Da biste potvrdili da ste pravilno omogućili besprijekoran SSO:
  
1. Prijavite se u [administrativni centar za Azure Active Directory](https://aad.portal.azure.com) kao globalni administrator.

2. U levom oknu odaberite **Azure Active Directory** .

3. Provjerite je li **omogućena**neprekinutu jedinstvenu prijavu.

Dodatne informacije potražite u članku [neprimjetna jedinstvena prijava u servisu Azure Active Directory: brzi početak](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-sso-quick-start).
  