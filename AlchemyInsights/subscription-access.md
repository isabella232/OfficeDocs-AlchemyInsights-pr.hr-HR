---
title: Pristup pretplatama
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
- "9003799"
- "6805"
ms.openlocfilehash: 166380cff09f2a2bd9b7e8914d5db4071b6c3f12
ms.sourcegitcommit: bec3554bf061ef28a009f460fb9d0a661b4fc008
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 10/27/2020
ms.locfileid: "48807223"
---
# <a name="unable-to-sign-in-azure-due-to-browser-issues-browser-hangs-keeps-spinning-does-not-load-etc"></a>Nije moguće prijaviti Azure zbog problema s preglednikom (ako se preglednik objesi, nastavlja se vrtjeti, ne učitava se, itd.)

Nakon toga će vas možda utjecati Prekoračeno vrijeme. Provjerite postoji li trenutna nevremena: [status stanja Azure](https://status.azure.com/status/history/).

Odjavite se od svih aktivnih sesija servisa Azure. Započnite privatni ili anonimni način web-preglednika.

Možete i pokušati osvježiti preglednik, koristiti neki drugi preglednik, izbrisati predmemorirane kolačiće ako više ne funkcionira.

Dodatne informacije: [Otklanjanje poteškoća s prijavom](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)

**Nije moguće pristupiti pretplatama**

Na [portalu Azure](https://portal.azure.com/)provjerite je li odabran ispravan direktorij Azure s računa u gornjem desnom kutu.

U [centru za račun Azure](https://account.windowsazure.com/Subscriptions)provjerite je li korišten račun administrator računa.

Dodatne informacije: [Otklanjanje poteškoća koje su pronađene pretplate](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)

**Nije moguće pristupiti povijesti naplate**

Administrator računa mora osigurati da korisnik koji pristupi podacima za naplatu bude dodan u servisu Azure Active Directory kao gost: [Dodajte ili izbrišite novog korisnika](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support).

Korisniku mora biti dodijeljena uloga globalnog administratora: [Dodjela uloge korisnicima](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).

Objavite to, korisniku se može dodijeliti pristup naplati pomoću RBAC pravilnika: [Dodijeli pristup naplati](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support).

**Preporučeni dokumenti**

-   [Ne mogu se prijaviti za upravljanje pretplatom na Azure](https://docs.microsoft.com/azure/billing-cannot-login-subscription?WT.mc_id=Portal-Microsoft_Azure_Support)