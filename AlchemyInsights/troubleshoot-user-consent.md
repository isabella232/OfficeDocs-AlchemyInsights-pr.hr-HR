---
title: Otklanjanje poteškoća s korisničkim pristajanjem
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
ms.openlocfilehash: 7249bafe1b047c66d9351a79f1782cfcc1a936a1
ms.sourcegitcommit: 7b213fd5e8a3fdb5c602673dc194d576d372ac96
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 01/18/2021
ms.locfileid: "49900839"
---
# <a name="troubleshoot-user-consent"></a>Otklanjanje poteškoća s korisničkim pristajanjem

1. Možete konfigurirati način na koji krajnji korisnici mogu pristati na aplikacije putem portala Azure ili komponente PowerShell. Dodatne informacije potražite u članku [Postavke pristanka korisnika](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) .
1. Administrator može koristiti i [Microsoft Graph API](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) za odobravanje pristanka na delegirane dozvole u ime jednog korisnika. Dodatne informacije potražite u članku [dohvaćanje programa Access u ime korisnika](https://docs.microsoft.com/graph/auth-v2-user).
1. [Pogreške prilikom pristanka korisnika](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error): u ovom se članku opisuju pogreške koje se mogu pojaviti tijekom postupka pristanka na aplikaciju. Ako otklanjate poteškoće s neočekivanim odobrenjem koje ne sadrže poruke o pogrešci, pročitajte članak [scenariji provjere autentičnosti za Azure ad](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).