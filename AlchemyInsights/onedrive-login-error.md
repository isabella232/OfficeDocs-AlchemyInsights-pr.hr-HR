---
title: OneDrive pogreška prilikom prijave AADSTS50011
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
- "9003820"
- "6840"
ms.openlocfilehash: 80aafa2aee7213e1b77d274509a7eb9741c20b525ed97f473093ac8c6514f3c7
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54112904"
---
# <a name="onedrive-login-error-aadsts50011"></a>OneDrive pogreška prilikom prijave AADSTS50011

Ako vam se prikazuje pogreška "AADSTS50011: URL odgovora naveden u zahtjevu ne odgovara odgovoru" prilikom prijave u aplikaciju OneDrive, provjerite sljedeće:

Verzija OneDrive mora biti jednaka ili veća od verzije 20.052.XXXX.XXXX. Da biste provjerili svoju verziju, kliknite plavu OneDrive u području obavijesti, odaberite **Pomoć & Postavke > Postavke > O programu**.

Mreža može blokirati promet na **g.live.com** i **oneclient.sfx.ms**. Ako je taj promet blokiran, OneDrive se ne može ažurirati. Radite s mrežnim administratorom da biste bili sigurni da imate pristup tim URL-ovima. [Te bi krajnje točke](https://docs.microsoft.com/microsoft-365/enterprise/urls-and-ip-address-ranges?view=o365-worldwide) trebale biti takve za korisnike koji koriste Microsoft 365 tarife.

Ako morate ručno nabaviti trenutnu verziju programa OneDrive, posjetite [https://aka.ms/getonedrive](https://aka.ms/getonedrive) .
