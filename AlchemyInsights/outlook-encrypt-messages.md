---
title: S/ MIME u programu Outlook na webu
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 7184ffd68f56639a8bcb87e9c6cab88388868103
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43764864"
---
# <a name="encrypt-email-messages-in-outlook"></a>Šifriranje poruka e-pošte u programu Outlook

Šifriranje poruka sustava Microsoft 365 izgrađeno je na servisu Microsoft Azure Rights Management (Azure RMS), koje je dio zaštite podataka usluge Azure. Ako vaša pretplata uključuje upravljanje pravima na Azure ili Azure Information Protection, **ne morate poduzimati nikakve radnje da biste ručno omogućili ili aktivirali** uslugu upravljanja pravima.

Na temelju povratnih informacija korisnika više nećemo moći omogućiti pravila tijeka pošte sustava Exchange da automatski šifriraju izlaznu e-poštu koja sadrži određenu vrstu osjetljivih podataka u klijentu prema zadanim postavkama. Umjesto toga, dajemo detaljne upute o tome kako to možete učiniti sami. Dodatne pojedinosti o stvaranju pravila prijenosa za šifriranje osjetljivih podataka potražite [u ovom članku](https://aka.ms/OmeEtr).

- Ako koristite Outlook na webu (bivši **OWA):** Prilikom sastavljanja poruke e-pošte jednostavno kliknite **Zaštiti** u programu OWA. To će primijeniti dozvolu "Ne prosljeđuj". Kliknite **Promijeni dozvolu** i odaberite **Šifriraj** da biste šifrirali samo poruku.

- Ako koristite **klijent programa Outlook**: Za slanje šifrirane poruke iz programa Outlook 2013 ili 2016 ili Outlook 2016 za Mac odaberite **Dozvole** > **mogućnosti**, a zatim odaberite željenu mogućnost zaštite.

- Da biste **automatski šifrirali svu e-poštu** poslanu određenim primateljima ili vanjskim partnerskim organizacijama, morate stvoriti pravilo prijenosa tijeka pošte u centru za administratore sustava Exchange. Detaljne upute navedene su u [ovom članku podrške](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities).

