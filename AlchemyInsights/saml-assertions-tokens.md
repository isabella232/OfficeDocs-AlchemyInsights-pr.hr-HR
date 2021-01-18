---
title: SAML tvrdnje (tokeni)
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004341"
- "7753"
ms.openlocfilehash: 557e23da09df3ab066c2ad7c0352f5fd904b5490
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 01/18/2021
ms.locfileid: "49884861"
---
# <a name="saml-assertions-tokens"></a>SAML tvrdnje (tokeni)

1. Tokeni za sigurnosne tvrdnje Markup Language (SAML) XML su prikazi potraživanja. Po zadanom, SAML tokeni Windows Communication Foundation (WCF) koristi se u vanjskim sigurnosnim scenarijima izdane su tokeni. Dodatne informacije potražite u članku [tokeni i tvrdnje o saml-](https://docs.microsoft.com/dotnet/framework/wcf/feature-details/saml-tokens-and-claims)u.
2. Microsoftova platforma identiteta emitira nekoliko vrsta sigurnosnih tokena u obradi svakog tijeka provjere autentičnosti. [Referenca zahtjeva za saml token](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens) opisuje oblikovanje, sigurnosne karakteristike i sadržaj žetona saml 2,0.
3. Slijedite upute u [konfiguracibilan token vijek u programu Microsoft Identity Platform](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes) da biste razumjeli kako konfigurisati životni vijek tokena.
4. Slijedite korake opisane u [ovom članku](https://docs.microsoft.com/azure/active-directory/manage-apps/howto-saml-token-encryption) da biste shvatili kako konfigurirati enkripciju tokena za Azure ad saml.
5. U servisu Azure AD možete postaviti mogućnosti potpisivanja certifikata i algoritam potpisivanja certifikata. Dodatne informacije potražite u članku dodatne [mogućnosti potpisivanja certifikata u Tokanu SAML-a za aplikacije Gallery u servisu Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).
