---
title: Dozvole i pristanak za API
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004343"
- "7756"
ms.openlocfilehash: c45bab67d414c8f0f2ca1c5275084d4ecce538c5256154292302080ba5bd8175
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53932089"
---
# <a name="api-permissions-and-consent"></a>Dozvole i pristanak za API

Aplikacije koje se integriraju Microsoftova platforma za identitete slijedite model autorizacije koji korisnicima i administratorima omogućuje kontrolu nad načinom pristupa podacima. Implementacija modela autorizacije ažurirana je na krajnjoj točki Microsoftova platforma za identitete autorizacije. Mijenja način na koji aplikacija mora stupiti u interakciju s Microsoftova platforma za identitete. [Dozvole i pristanak u krajnjoj Microsoftova platforma za identitete obuhvaća](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) osnovne koncepte ovog modela autorizacije, uključujući opsege, dozvole i pristanak.

Okvir [Azure Active Directory pristanak (Azure AD)](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) olakšava razvoj web-aplikacija s više klijenata i nativnih klijentskih aplikacija. Te aplikacije omogućuju prijavu korisničkih računa s klijenta servisa Azure AD koji se razlikuje od one u kojoj je aplikacija registrirana. Osim vlastitih API-ja na webu, možda će morati pristupati i web-API-jem kao što su API-je za Microsoft Graph (da bi pristupili servisima Azure AD, Intune i Microsoft 365) i drugim API-jem Microsoft services-ja.

