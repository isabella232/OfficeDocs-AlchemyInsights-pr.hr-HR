---
title: S/MIME u programu Outlook na webu
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 33e94eac6a2982b8036e13d17bf60015f244f2cb
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 12/15/2019
ms.locfileid: "40053217"
---
# <a name="encrypt-email-messages-in-outlook"></a>Šifriranje poruka e-pošte u programu Outlook

Office 365 šifriranje poruka izgrađeno je na servisu Microsoft Azure Rights Management (Azure RMS), koja je dio usluge Azure Information Protection. Ako vaša pretplata uključuje upravljanje pravima na Azure ili zaštitu informacija za Azure, **ne morate poduzeti nikakve radnje kako biste ručno omogućili ili aktivirali** uslugu upravljanja pravima.

Na temelju povratnih informacija kupaca više nećemo omogućiti Exchange pravila tijeka pošte za automatsko šifriranje izlazne e-pošte koja sadrži određenu vrstu osjetljivih podataka u vašem klijentu po zadanim postavkama. Umjesto toga, pružamo detaljne upute o tome kako to možete učiniti sami. Dodatne pojedinosti o stvaranju pravila prijevoza za šifriranje osjetljivih podataka potražite u [ovom članku](https://aka.ms/OmeEtr).

- Ako koristite Outlook na webu (nekadašnji **OWA**): prilikom sastavljanja poruke e-pošte, jednostavno kliknite **Zaštitite** u OWI. To će primijeniti dopuštenje "ne prosljeđivati". Kliknite **Promijeni dozvolu** i odaberite **Šifriraj** da biste šifrirali poruku.

- Ako koristite **Outlook Client**: za slanje šifrirane poruke iz programa Outlook 2013 ili 2016 ili Outlook 2016 za Mac, odaberite **opcije** > **dozvole**, a zatim odaberite mogućnost zaštite koja vam je potrebna.

- Da biste **automatski šifrirali svu e-poštu** poslanu određenim primateljima ili vanjskim partnerskim organizacijama, morate stvoriti pravilo transporta prijenosa pošte u centru za administraciju sustava Exchange. Detaljne upute navedene su u [ovom članku podrške](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities).

