---
title: Pogreška prilikom prijave na OneDrive AADSTS50011
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
ms.openlocfilehash: 1f906f82e99c322ed953800d54fba5a073eacd10
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 11/09/2020
ms.locfileid: "48982430"
---
# <a name="onedrive-login-error-aadsts50011"></a>Pogreška prilikom prijave na OneDrive AADSTS50011

Ako vam se prikaže pogreška "AADSTS50011: URL za odgovor naveden u zahtjevu ne podudara se s odgovorom" prilikom prijave u aplikaciju OneDrive provjerite sljedeće:

Verzija servisa OneDrive mora biti jednaka ili veća od verzije 20.052. XXXX. XXXX. Da biste provjerili svoju verziju, kliknite plavu ikonu servisa OneDrive u području obavijesti, odaberite **Help & postavke > postavke >**.

Vaša mreža može blokirati promet na **g.Live.com** i **oneclient.SFX.MS**. Ako je promet blokiran, OneDrive se ne može ažurirati. Radite s mrežnim administratorom da biste bili sigurni da imate pristup tim URL-ovima. [Te krajnje točke](https://docs.microsoft.com/microsoft-365/enterprise/urls-and-ip-address-ranges?view=o365-worldwide) trebale bi biti dostupne korisnicima koji koriste planove za Microsoft 365.

Ako morate ručno nabaviti postojeću verziju servisa OneDrive, posjetite je [https://aka.ms/getonedrive](https://aka.ms/getonedrive) .
