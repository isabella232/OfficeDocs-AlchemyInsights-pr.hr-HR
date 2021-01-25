---
title: API dozvole i pristanak
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
ms.openlocfilehash: c99e5e2e8fb9bcc88e5221890ed9c28ed9e7d0c8
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974259"
---
# <a name="api-permissions-and-consent"></a>API dozvole i pristanak

Aplikacije koje se integriraju sa platformom Microsoftova identiteta slijede model autorizacije koji korisnicima i administratorima omogućuje kontrolu nad načinom pristupa podacima. Implementacija modela autorizacije ažurirana je na krajnjoj točki Microsoftove identifikacijske platforme. Mijenja način interakcije aplikacije s Microsoftovu platformom Identity. [Dozvole i pristanak u krajnjoj točki platforme Microsoft Identity](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) obuhvaća osnovne koncepte ovog modela autorizacije, uključujući dosege, dozvole i pristanak.

[Okvir za suglasnost servisa Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) olakšava razvijanje web-mjesta i izvornih klijentskih aplikacija za više korisnika. Te aplikacije omogućuju prijavu za korisničke račune iz stanara Azure AD koji se razlikuje od onog u kojem je aplikacija registrirana. Možda će morati pristupati i web-API-Jima, kao što je Microsoft Graph API (da biste pristupili Azure AD, Intune i Services u programu Microsoft 365) i drugim API-Jima sustava Microsoft Services, uz vlastite web-API-je.

