---
title: Pristup pretplati
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
ms.openlocfilehash: b138c05e87e70c18bb6528819a34f8a9501446d57dcf4dbac0734f70fbc3466b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53999232"
---
# <a name="unable-to-sign-in-azure-due-to-browser-issues-browser-hangs-keeps-spinning-does-not-load-etc"></a>Nije moguće prijaviti Azure zbog problema s preglednikom (preglednik se prekida, vrti se, ne učitava se itd.)

Na vas može utjecati neusiljedstvo. Provjerite je li došlo do odlaznog stanja: [stanje stanja sustava Azure](https://status.azure.com/status/history/).

Odjavite se iz svih aktivnih sesija servisa Azure. Pokrenite privatni ili anonimni način rada web-preglednika.

Možete i pokušati osvježiti preglednik, koristiti neki drugi preglednik, izbrisati kolačiće predmemorije ako gore ne funkcionira.

Dodatne informacije: [Otklanjanje poteškoća s prijavom](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)

**Nije moguće pristupiti pretplatama**

Na [portalu Azure](https://portal.azure.com/)provjerite je li odabran odgovarajući direktorij servisa Azure s računa u gornjem desnom mjestu.

U centru [za račun za Azure](https://account.windowsazure.com/Subscriptions)provjerite je li korišteni račun administrator računa.

Dodatne informacije: Otklanjanje [poteškoća s nenađenim pretplatama](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)

**Nije moguće pristupiti povijesti naplate**

Administrator računa mora biti siguran da se korisnik koji pristupa podacima za naplatu doda u direktorij Servisa Azure Active kao gost: [Dodavanje ili brisanje novog korisnika.](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support)

Korisniku se zatim mora dodijeliti uloga globalnog administratora: [Dodjela uloge korisnicima](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).

Objavite to, korisniku se može dodijeliti pristup naplati pomoću pravilnika RBAC: [Odobravanje pristupa naplati](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support).

**Preporučeni dokumenti**

-   [Ne mogu se prijaviti da bih upravljao pretplatom na Azure](https://docs.microsoft.com/azure/billing-cannot-login-subscription?WT.mc_id=Portal-Microsoft_Azure_Support)