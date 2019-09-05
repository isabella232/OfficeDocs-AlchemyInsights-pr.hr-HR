---
title: S/MIME u programu Outlook na webu
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 6915470655b85922f6f97e8ca6fac353224b1ae0
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36752852"
---
# <a name="encrypt-email-messages-in-outlook"></a>Šifriranje poruke e-pošte u programu Outlook

Šifriranje poruke Office 365 izgrađen na Microsoft Azure upravljanje pravima (Azure RMS), koji je dio Azure informacije zaštitu. Ako vaša pretplata uključuje Azure pravima ili zaštita Azure informacije **ne trebate poduzeti akcije ručno omogućiti ili aktivirati** uslugu upravljanja pravima.

Na temelju povratnih smo će više neće biti omogućavanje pravila toka pošte Exchange automatski šifrirati izlaznog e-pošta koja sadrži određene vrste osjetljive informacije u vašem klijentske po zadanom. Smo se umjesto toga pruža detaljne upute na kako to možete učiniti yourselves. Za dodatne pojedinosti o tome kako stvoriti pravilo prijevoza za šifriranje osjetljivih informacija, pogledajte [Ovaj članak](https://aka.ms/OmeEtr).

- Ako pomoću programa Outlook na webu (prije **OWA**): kada sastavljate poruku e-pošte, jednostavno kliknite **zaštiti** u programu OWA. To će se primijeniti dozvole "Ne prosljeđuj". Kliknite **Promijeni dozvole** i odaberite **Šifriraj** samo šifrirati poruke.

- Ako koristite **Outlook klijent**: poslati šifriranu poruku iz Outlook 2013 ili 2016 ili Outlook 2016 za Mac odaberite **Mogućnosti** > **dozvole**, a zatim odaberite mogućnost zaštite trebate.

- Da biste **automatski šifriranje sve e-pošte** šalju određene primatelje ili vanjski partner organizacijama, morate stvoriti pravilo toka prijevoza pošte u centru za administraciju sustava Exchange. U [ovom članku za podršku](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities)se daju detaljne upute.

