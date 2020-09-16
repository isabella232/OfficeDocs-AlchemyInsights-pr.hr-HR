---
title: S/MIME u programu Outlook na webu
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 052149d1f11387246bc1ff24ba48c45b944ba52c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47772254"
---
# <a name="encrypt-email-messages-in-outlook"></a>Šifriranje poruka e-pošte u programu Outlook

Šifriranje poruka u sustavu Microsoft 365 izgrađeno je na servisu Microsoft Azure Rights Management (Azure RMS), koji je dio zaštite informacija za Azure. Ako vaša pretplata obuhvaća upravljanje pravima na Azure i Azure, ne **morate poduzeti nikakve akcije da biste ručno omogućili ili aktivirali** servis za upravljanje pravima.

Na temelju povratnih informacija o klijentu više neće biti omogućeno automatsko šifriranje odlaznih poruka e-pošte koja sadrži određene vrste osjetljivih podataka u zakupcu. Umjesto toga dajemo detaljne upute o tome kako to sami možete učiniti. Dodatne informacije o stvaranju pravila prijenosa radi šifriranja osjetljivih informacija potražite u [ovom članku](https://aka.ms/OmeEtr).

- Ako koristite Outlook na webu (bivši **OWA**): prilikom skladanja poruke e-pošte jednostavno kliknite **zaštiti** u aplikaciji OWA. Time će se primijeniti dozvola "Ne prosljeđuj". Kliknite **Promijeni dozvolu** , a zatim **Šifriraj** samo da biste šifrirali poruku.

- Ako koristite **klijent programa Outlook**: da biste slali šifriranu poruku iz programa Outlook 2013 ili 2016 ili Outlook 2016 za Mac, odaberite **mogućnosti**  >  **dozvole**, a zatim odaberite mogućnost zaštite koja vam je potrebna.

- Da biste **automatski šifrirali sve poruke e-pošte** poslane određenim primateljima ili vanjskim partnerskim organizacijama, morate stvoriti pravilo prijenosa tijeka pošte u centru za administratore sustava Exchange. Detaljne upute navedene su u [ovom članku podrške](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities).

