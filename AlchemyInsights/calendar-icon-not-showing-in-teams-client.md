---
title: Ikona kalendara ne prikazuje se u klijentu sustava Teams
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001219"
- "4375"
ms.openlocfilehash: 7881d6837cb7d99180d2cc1b28d327ce12e4b836d33e4fca099569d4f72510fa
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53989583"
---
# <a name="calendar-icon-not-showing-in-teams-client"></a>Ikona kalendara ne prikazuje se u klijentu sustava Teams

Kartica kalendar u sustavu Teams zahtijeva pristup poštanskom sandučiću sustava Exchange pomoću web-servisa sustava Exchange. Poštanski sandučić sustava Exchange može biti mrežni ili lokalni. Za mrežne korisnike kojima se ne prikazuje kartica Kalendar provjerite jesu li [licencirani za poštanski sandučić sustava Exchange Online i je li poštanski sandučić omogućen](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).

Ako korisnik ima valjani poštanski sandučić u sustavu Exchange Online, no i dalje ne može vidjeti karticu Kalendar, možda nailazite na problem s mrežom. Koristite [Microsoftov analizator za daljinsko povezivanje](https://testconnectivity.microsoft.com/) i pokrenite **testiranja povezivanja sustava Microsoft Exchange Web Services** za zahvaćenog korisnika.

Napokon provjerite aplikacije [Teams – pravilnike o postavljanju aplikacija](https://admin.teams.microsoft.com/policies/app-setup) da biste osigurali da aplikacija Kalendar nije uklonjena iz pravilnika koji je primijenjen na korisnika (najvjerojatnije **Global (zadano na razini tvrtke ili ustanove)**.

Ako su vaši korisnici lokalni, morate provjeriti je li vaša hibridna konfiguracija zdrava. Otklanjanje poteškoća pomoću [Čarobnjaka za hibridne konfiguracije](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent).

Imajte na umu da [sustav Teams zahtijeva Exchange 2016 CU3 ili napredniju verziju](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).
