---
title: Uklanjanje pozadinskog servisa za Microsoft Search u programu Bing
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/12/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9214"
- "9005302"
ms.openlocfilehash: 6447137fca9b2d48508f4e240a438c7f851c103c
ms.sourcegitcommit: 3fb39a080cc8680d960b8468ac9355389a3e2df4
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50816090"
---
# <a name="remove-the-background-service-for-microsoft-search-in-bing"></a>Uklanjanje pozadinskog servisa za Microsoft Search u programu Bing

Da biste uklonili pozadinski servis za Microsoft Search u programu Bing, isprobajte sljedeće lijekove:

1. Da biste se vratili na izvorne postavke tražilice, učinite sljedeće:

    je. Promijenite gumb **koristi Bing kao zadanu postavku isključivanja tražilice [](https://docs.microsoft.com/deployoffice/microsoft-search-bing#change-whether-bing-is-the-default-search-engine-for-google-chrome)**.

    b. [Otvorite centar za administratore sustava Microsoft 365](https://docs.microsoft.com/deployoffice/microsoft-search-bing#configure-the-setting-in-the-microsoft-365-admin-center-to-allow-the-extension-to-be-installed) i poništite postavku koja utječe na sve korisnike u tvrtki ili ustanovi.

2. Da biste uklonili pozadinski servis s pojedinog uređaja, učinite sljedeće:

    je. Odaberite **Upravljačka ploča > programe > programe i značajke**.

    b. Desnom tipkom miša kliknite **Microsoft Search u programu Bing na** popisu instaliranih programa, a zatim kliknite **Deinstaliraj**.

3. Da biste uklonili poslužitelj pozadine s više uređaja u tvrtki ili ustanovi, prijavite se kao administrator i pokrenite sljedeću naredbu u skripti: 

`"%ProgramFiles(x86)%\Microsoft\DefaultPackMSI\MainBootStrap.exe" uninstallAll`
