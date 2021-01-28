---
title: Problemi s tvrdnjama i atributima tokena
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
- "9004347"
- "7761"
ms.openlocfilehash: 4c12f768ab4bf4547f48abc19736743fa555c477
ms.sourcegitcommit: c1c6047ec467853dc823a17b02c461a6a476406d
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 01/27/2021
ms.locfileid: "50035832"
---
# <a name="issues-with-token-claims-and-attributes"></a>Problemi s tvrdnjama i atributima tokena

**Ažuriranje, konfiguriranje i uklanjanje potraživanja od tokena**

1. Pomoću servisa Azure Active Directory (Azure AD) možete [prilagoditi vrstu potraživanja za zahtjev za ulogu](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) u toknu odaziva koji ste primili nakon autorizacija aplikacije.
2. Programeri aplikacija mogu koristiti neobavezne tvrdnje u svojim aplikacijama za Azure AD da bi naveli koje tvrdnje žele u tokene poslane u njihovu aplikaciju. Dodatne informacije potražite u članku [pružanje neobaveznih zahtjeva za aplikaciju](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims).
3. [Konfigurirajte grupne potraživanja za aplikacije pomoću servisa Azure Active Directory](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims).
4. Ako koristite neprekinutu jedinstvenu prijavu u aplikaciji, pročitajte članak [Prilagodba potraživanja izdanih u programu SAML token za Enterprise Applications](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization).

**Mapiranje atributa potraživanja**

1. Da biste konfigurirali pravilnik o preslikavanju potraživanja pomoću komponente PowerShell, pročitajte članak [Prilagodba potraživanja koje emitiraju tokeni za određenu aplikaciju u klijentu (pretpregled)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping).
2. Atributi proširenja sheme direktorija nude način spremanja dodatnih podataka u servisu Azure Active Directory na korisničke objekte i druge objekte direktorija, kao što su grupe, detalji o klijentu, ravnatelji servisa. Samo atributi proširenja na korisničke objekte mogu se koristiti za emitiranje potraživanja u aplikacije. [Pomoću atributa proširenja sheme direktorija u tvrdnjama](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) opisan je način korištenja atributa proširenja sheme direktorija za slanje korisničkih podataka u aplikacije u tvrdnjama tokena.

Dodatne informacije o tvrdnjama tokena potražite u članku:

- [Potraživanja u programu Access tokens](https://docs.microsoft.com/azure/active-directory/develop/access-tokens#claims-in-access-tokens)
- [Potraživanja u id_token](https://docs.microsoft.com/azure/active-directory/develop/id-tokens#claims-in-an-id_token)
- [Tvrdi](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) da možete očekivati u ID tokena i pristupne tokeni koje je izdala Azure ad B2C
- [Referenca za SAML token](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens)
