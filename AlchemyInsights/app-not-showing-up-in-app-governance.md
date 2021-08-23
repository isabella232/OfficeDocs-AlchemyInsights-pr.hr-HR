---
title: Aplikacija se ne prikazuje u upravljanju aplikacijama
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 8/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9007647"
- "12734"
ms.openlocfilehash: a8d176fdee073e41b61de6f53c728601da955aaa
ms.sourcegitcommit: 2be4a0352cb84a703ebf12966e1c17b64df07364
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/16/2021
ms.locfileid: "58454468"
---
# <a name="my-app-isnt-showing-up-in-app-governance"></a>Aplikacija se ne prikazuje u upravljanju aplikacijama

Ako se aplikacija ne prikazuje u upravljanju aplikacijama, provjerite sljedeće:

1. Idite [na Azure AD](https://aad.portal.azure.com/) i pronađite ID aplikacije za aplikaciju tako da na gornjoj traci na stranici Pregled pronađete naziv aplikacije.

1. Pristupite Graph Exploreru i potražite ID aplikacije unutar upravitelja servisa pomoću tog upita i zamijenite odgovarajućim <appId> ID-om aplikacije: < https://graph.microsoft.com/v1.0/servicePrincipals? $search= "appId: <appId> ">

1. Ako nema rezultata, potražite ID aplikacije u aplikaciji pomoću tog upita i zamijenite ga <appId> odgovarajućim ID-om aplikacije: < https://graph.microsoft.com/v1.0/applications? $search= "appId: <appId> ">

Ako imate problema s upitom, pogledajte [pomoć](https://docs.microsoft.com/microsoft-365/business-video/get-help-support). 

Dodatne informacije ili uvid u aplikacije u upravljanju aplikacijama potražite u [članku Saznajte više o vidljivosti i uvidima](https://docs.microsoft.com/microsoft-365/compliance/app-governance-visibility-insights-overview).

Dodatne informacije o prikazu aplikacija potražite u članku [Prikaz aplikacija](https://docs.microsoft.com/microsoft-365/compliance/app-governance-visibility-insights-view-apps).
