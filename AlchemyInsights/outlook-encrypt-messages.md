---
title: S/MIME u Outlook na webu
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
ms.openlocfilehash: bef87baafdbaf9346f99f1ff54aaa83bc9173c70f1412ea00afb717c15a8014c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54010716"
---
# <a name="encrypt-email-messages-in-outlook"></a>Šifriranje poruka e-pošte u Outlook

Microsoft 365 Šifriranje poruka temelji se na upravljanju pravima na Microsoft Azure (Azure RMS), koji je dio platforme Azure Information Protection. Ako vaša pretplata obuhvaća Azure Rights Management ili Azure Information Protection, ne morate ništa poduzeti da biste ručno **omogućili ili aktivirali** servis za upravljanje pravima.

Na temelju povratnih informacija klijenata više nećemo Exchange pravila tijeka pošte automatski šifrirati odlaznu e-poštu koja po zadanom sadrži određene vrste osjetljivih podataka u klijentu. Umjesto toga, nudimo detaljne upute o tome kako to možete učiniti sami. Dodatne informacije o stvaranju pravila prijenosa radi šifriranja osjetljivih podataka potražite u [ovom članku](https://aka.ms/OmeEtr).

- Ako koristite Outlook na webu (prijašnji **OWA):** Prilikom sastavljanja poruke e-pošte jednostavno **kliknite Zaštiti u** aplikaciji OWA. Na to će se primijeniti dozvola "Ne prosljeđuj". Kliknite **Promijeni dozvolu i** odaberite **Šifriraj** da biste šifrirali samo poruku.

- Ako **koristite Outlook**: da biste poslali šifriranu poruku iz programa Outlook 2013 ili 2016 ili Outlook 2016 za Mac, odaberite **Mogućnosti** Dozvole , a zatim odaberite  >  željenu mogućnost zaštite.

- Da **biste automatski šifrirali sve** poruke e-pošte poslane određenim primateljima ili vanjskim partnerskim tvrtkama ili ustanovama, morate stvoriti pravilo prijenosa tijeka pošte u centru Exchange administratora. Detaljne upute navedene su u [ovom članku za podršku](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities).

