---
title: Ikona kalendara ne prikazuje se u Microsoft Teams klijentu
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001219"
- "6794"
- "3403"
ms.openlocfilehash: edd6b4a2d94b03cf4ae7bf3a8d6332ed94a7e8263aba9df1f9588eecbd0ce05a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54119996"
---
# <a name="calendar-icon-isnt-showing-in-microsoft-teams-client"></a>Ikona kalendara ne prikazuje se u Microsoft Teams klijentu

Kartica **Kalendar** u aplikaciji Teams potreban je pristup poštanskom sandučiću Exchange putem Exchange web-servisa. Poštanski Exchange može biti na mreži ili lokalno. Za korisnike s interneta koji ne vide **karticu** Kalendar provjerite jesu li licencirani za poštanski Exchange Online i je li poštanski [sandučić omogućen](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes). Ako su vaši korisnici lokalno kod kuće, morate potvrditi je li hibridna konfiguracija zdrava. Otklanjanje poteškoća pomoću [Čarobnjaka za hibridne konfiguracije](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent). Imajte na umu da [sustav Teams zahtijeva Exchange 2016 CU3 ili napredniju verziju](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).

Dodatne informacije i upute za otklanjanje poteškoća potražite u članku [Otklanjanje poteškoća s Microsoft Teams i Exchange Server interakcije](https://docs.microsoft.com/microsoftteams/troubleshoot/known-issues/teams-exchange-interaction-issue).
