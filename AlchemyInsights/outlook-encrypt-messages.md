---
title: S / MIME u programu Outlook na webu
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 6bbbf8722dacb8b7d5191d57ce1055a48dcb4dd0
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511500"
---
# <a name="encrypt-email-messages-in-outlook"></a>Šifriranje poruka e-pošte u programu Outlook

Microsoft 365 Šifriranje poruka izgrađen je na Microsoft Azure prava management (Azure RMS), koji je dio Azure Information Protection. Ako vaša pretplata uključuje upravljanje pravima na Azure ili zaštitu informacija o platformi Azure, **ne morate poduzimati nikakve radnje da biste ručno omogućili ili aktivirali** uslugu upravljanja pravima.

Na temelju povratnih informacija korisnika više nećemo omogućiti pravilima tijeka pošte sustava Exchange da automatski šifriraju odlaznu e-poštu koja sadrži određenu vrstu osjetljivih podataka na klijentu prema zadanim postavkama. Umjesto toga, pružamo detaljne upute o tome kako to možete učiniti sami. Dodatne pojedinosti o stvaranju pravila prijenosa za šifriranje osjetljivih informacija potražite u [ovom članku](https://aka.ms/OmeEtr).

- Ako koristite Outlook na webu (bivši **OWA):** Prilikom sastavljanja poruke e-pošte jednostavno kliknite **Zaštiti** u OWA. To će primijeniti dozvolu "Ne prosljeđujte". Kliknite **Promijeni dozvolu,** a zatim odaberite **Šifriraj** da biste šifrirali samo poruku.

- Ako koristite **klijent programa Outlook**: Da biste poslali šifriranu poruku iz programa Outlook 2013 ili 2016 ili Outlook 2016 za Mac, odaberite **Dozvole za mogućnosti**, a zatim odaberite  >  **Permissions**željenu mogućnost zaštite.

- Da biste **automatski šifrirali svu e-poštu** poslanu određenim primateljima ili vanjskim partnerskim organizacijama, morate stvoriti pravilo prijenosa tijeka pošte u centru za administratore sustava Exchange. Detaljne upute navedene su u [ovom članku podrške](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities).

