---
title: Problemi s uređajima za ukrcavanje
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6023"
- "9002913"
ms.openlocfilehash: c3203ed68eb19d5f6d75eb2269094bb0422b14cc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47676874"
---
# <a name="issues-with-onboarding-machines"></a>Problemi s uređajima za ukrcavanje

Možda imate problema s uređajima za ukrcavanje na servisu MDATP. Ako možete pristupiti stroju krajnjeg korisnika, slijedite ove korake:

1. Preuzmite dijagnostički alat za [analizu povezivanja s klijentom](https://aka.ms/mdatpanalyzer) .
2. Ekstrakt i trčanje MDATPAnalyzer. cmd.
3. Pronađite Dijagnostički zapisnik u mapi Mdatpclientanalyzer, istoj mapi u kojoj je preuzeta alat za analizu.
4. Pregledajte datoteku zapisnika, MDATPClientAnalyzer.txt i potražite probleme s postavkama internetske veze.