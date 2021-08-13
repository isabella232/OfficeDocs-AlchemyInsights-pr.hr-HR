---
title: Otklanjanje poteškoća s pristankom korisnika
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004353"
- "7785"
ms.openlocfilehash: db784c133fec554604ad09f5b27941879d97ff238f926ff6338d0f3b7c3c4105
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54007890"
---
# <a name="troubleshoot-user-consent"></a>Otklanjanje poteškoća s pristankom korisnika

1. Način pristanka krajnjih korisnika na aplikacije možete konfigurirati putem portala Azure ili ljuske PowerShell. Dodatne [informacije potražite u odjeljku](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) Postavke pristanka korisnika.
1. Administrator može koristiti i [MICROSOFTOV API Graph za](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) davanje pristanka na delegirane dozvole u ime jednog korisnika. Dodatne informacije potražite u [članku Pristup u ime korisnika](https://docs.microsoft.com/graph/auth-v2-user).
1. [Pogreške pri pristanku](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)korisnika : u ovom se članku razmatraju pogreške koje se mogu pojaviti tijekom postupka pristanka na aplikaciju. Ako otklanjate poteškoće s neočekivanim upitima za pristanak koji ne sadrže poruke o pogreškama, pogledajte [scenarije provjere autentičnosti za Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).