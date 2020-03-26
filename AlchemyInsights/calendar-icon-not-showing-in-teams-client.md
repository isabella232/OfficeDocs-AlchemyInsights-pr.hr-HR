---
title: Ikona kalendara ne prikazuje se u klijentu sustava Teams
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001219"
- "4375"
ms.openlocfilehash: 21692639fb746b2e5aab3dfc8894293d5dc890ac
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931874"
---
# <a name="calendar-icon-not-showing-in-teams-client"></a>Ikona kalendara ne prikazuje se u klijentu sustava Teams

Kartica kalendar u sustavu Teams zahtijeva pristup poštanskom sandučiću sustava Exchange pomoću web-servisa sustava Exchange. Poštanski sandučić sustava Exchange može biti mrežni ili lokalni. Za mrežne korisnike kojima se ne prikazuje kartica Kalendar provjerite jesu li [licencirani za poštanski sandučić sustava Exchange Online i je li poštanski sandučić omogućen](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).

Ako korisnik ima valjani poštanski sandučić u sustavu Exchange Online, no i dalje ne može vidjeti karticu Kalendar, možda nailazite na problem s mrežom. Koristite [Microsoftov analizator za daljinsko povezivanje](https://testconnectivity.microsoft.com/) i pokrenite **testiranja povezivanja sustava Microsoft Exchange Web Services** za zahvaćenog korisnika.

Napokon provjerite aplikacije [Teams – pravilnike o postavljanju aplikacija](https://admin.teams.microsoft.com/policies/app-setup) da biste osigurali da aplikacija Kalendar nije uklonjena iz pravilnika koji je primijenjen na korisnika (najvjerojatnije **Global (zadano na razini tvrtke ili ustanove)**.

Ako su vaši korisnici lokalni, morate provjeriti je li vaša hibridna konfiguracija zdrava. Otklanjanje poteškoća pomoću [Čarobnjaka za hibridne konfiguracije](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent).

Imajte na umu da [sustav Teams zahtijeva Exchange 2016 CU3 ili napredniju verziju](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).
