---
title: Rješavanje uobičajenih problema s oblikovanjem DKIM zapisa
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/23/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: 5b3dc2338843906fbc7151322b82f304b4ed04b28d8ceb349f2705c309cdeae8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53930053"
---
# <a name="fix-common-problems-with-dkim-record-formatting"></a>Rješavanje uobičajenih problema s oblikovanjem DKIM zapisa

Većina problema s postavljanjem DKIM-a povezana je s netočnim DNS zapisima.

Da biste riješili probleme s postavljanjem DKIM-a, provjerite je li DKIM CNAME zapis (a ne TXT zapis) pravilno oblikovan. Dodatne informacije potražite u članku Što morate učiniti da biste ručno [postavili DKIM u programu Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email).

Ako vam je općenito potrebna pomoć za DNS zapise, pogledajte stvaranje DNS zapisa kod bilo kojeg [davatelja usluge hostiranja DNS-a za Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).

> [!NOTE]
> Kada stvorite ili ažurirate DKIM DNS zapise na servisu za hostiranje DNS-a za svoju domenu, morate pričekati širenje DNS zapisa.
