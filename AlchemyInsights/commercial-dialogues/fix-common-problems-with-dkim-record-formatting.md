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
ms.openlocfilehash: e55175e7613d220eaf956d3c7fd02213dcd5803d
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58323982"
---
# <a name="fix-common-problems-with-dkim-record-formatting"></a>Rješavanje uobičajenih problema s oblikovanjem DKIM zapisa

Većina problema s postavljanjem DKIM-a povezana je s netočnim DNS zapisima.

Da biste riješili probleme s postavljanjem DKIM-a, provjerite je li DKIM CNAME zapis (a ne TXT zapis) pravilno oblikovan. Dodatne informacije potražite u članku Što morate učiniti da biste ručno postavili [DKIM u programu Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email).

Ako vam je općenito potrebna pomoć za DNS zapise, pogledajte stvaranje DNS zapisa kod bilo kojeg [davatelja usluge hostiranja DNS-a za Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).

**Napomena:** kada stvorite ili ažurirate DKIM DNS zapise na servisu za hostiranje DNS-a za svoju domenu, morate pričekati širenje DNS zapisa.
