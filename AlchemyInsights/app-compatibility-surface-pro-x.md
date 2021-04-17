---
title: Kompatibilnost aplikacija sa sustavom Microsoft Surface Pro X
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/14/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7009"
- "9003951"
ms.openlocfilehash: 085815982a3948a7853326541101d2ed21c1869e
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51837098"
---
# <a name="app-compatibility-with-microsoft-surface-pro-x"></a>Kompatibilnost aplikacija sa sustavom Microsoft Surface Pro X

Aplikacije se drugačije koriste na uređajima kao što je Surface Pro X. No većina aplikacija kompatibilna je s nekim ograničenjima. Evo popisa problema koje biste mogli imati prilikom pokretanja aplikacije: 

**Upravljački programi.** Upravljački će programi funkcionirati ako su namijenjeni PC-ju sa sustavom Windows 10 ARM. Ako upravljački program ne funkcionira, ni aplikacija ili hardver na koji se oslanja neće funkcionirati. Dodatnu podršku za uređaj potražite u članku Najčešća [pitanja o PC-jevima sa sustavom Windows 10 ARM](https://support.microsoft.com/windows/windows-10-arm-based-pcs-faq-477f51df-2e3b-f68f-31b0-06f5e4f8ebb5) ili se obratite proizvođaču hardvera.

**64-bitne (x64) aplikacije.** Aplikacije koje su 64-bitne (x64) neće funkcionirati. Potrebne su vam 64-bitne (ARM64) aplikacije, 32-bitne (ARM32) aplikacije ili 32-bitne (x86) aplikacije. Obično možete pronaći 32-bitne (x86) verzije aplikacija, ali neki razvojni inženjeri aplikacija nude samo 64-bitne (x64) aplikacije.

**Prilagođene aplikacije.** Aplikacije koje prilagođavaju doživljaj sustava Windows, kao što su pomoćne tehnologije ili aplikacije za pohranu u oblaku, mogu imati problema. Da biste saznali više, obratite se proizvođaču aplikacije.

**Antivirusni softver drugih proizvođača.** Neki antivirusni softver drugih proizvođača nije moguće instalirati. Sigurnost sustava Windows pridonosi zaštiti za podržani vijek trajanja uređaja sa sustavom Windows 10.

**Faksiranje i skeniranje u sustavu Windows.** Faksiranje i skeniranje sustava Windows nije dostupno na PC-ju sa sustavom Windows 10 ARM.

Ako naiđete na probleme prilikom instalacije, deinstalacije ili ponovne instalacije aplikacije, pogledajte pojedinosti [o otklanjanju poteškoća s aplikacijom](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-app-install#app-troubleshooting-details).

Osim u rijetkim slučajevima, sve ključne riječi moraju biti OR, a ne AND.