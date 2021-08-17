---
title: Tvrdnje o SAML-u (tokeni)
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
ms.openlocfilehash: 9c8ff0d4ff6da98ed6a5c42570d4a5fac80b00e93d1356b298528bd8d2c51a5f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54109232"
---
# <a name="saml-assertions-tokens"></a>Tvrdnje o SAML-u (tokeni)

1. Tokeni za označavanje sigurnosnih tvrdnji (SAML) XML su prikazi potraživanja. Prema zadanim postavkama, SAML tokeni Windows communication Foundation (WCF) u vanjskim sigurnosnim scenarijima izdaju tokene. Dodatne informacije potražite u članku [SAML tokeni i potraživanja](https://docs.microsoft.com/dotnet/framework/wcf/feature-details/saml-tokens-and-claims).
2. Program Microsoftova platforma za identitete nekoliko vrsta sigurnosnih tokena u obradi svakog tijeka provjere autentičnosti. [Referenca na tvrdnje SAML tokena](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens) opisuje oblik, sigurnosne karakteristike i sadržaj SAML 2.0 tokena.
3. Slijedite smjernice u [vijekovima tokena](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes) koji se mogu konfigurirati Microsoftova platforma za identitete biste razumjeli kako konfigurirati vijek trajanja tokena.
4. Slijedite korake navedene u ovom [članku da biste](https://docs.microsoft.com/azure/active-directory/manage-apps/howto-saml-token-encryption) razumjeli kako konfigurirati šifriranje tokena azure AD SAML.
5. Na servisu Azure AD možete postaviti mogućnosti potpisivanja certifikata i algoritam za potpisivanje certifikata. Dodatne informacije potražite u članku Dodatne [mogućnosti potpisivanja certifikata u SAML tokenu za aplikacije galerije u Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).
