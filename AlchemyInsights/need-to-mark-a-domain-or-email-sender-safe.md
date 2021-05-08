---
title: Morate označiti domenu ili pošiljatelja e-pošte sigurnim?
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002921"
- "5673"
ms.openlocfilehash: 57d1e2d696a8be42b5f868f021d829bf019349bf
ms.sourcegitcommit: 3994cece80410371330b39f7b79b1b1c1bfcf648
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 05/08/2021
ms.locfileid: "52286672"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a>Morate označiti domenu ili pošiljatelja e-pošte sigurnim?

- Korištenje popisa **sigurnih pošiljatelja ne preporučuje** se jer se u tvrtki ili ustanovi otvara neželjena pošta, fazani i lažni napadi.
- No ako postoji poslovni preduvjet, **preporučujemo** da za to Flow pravila aplikacije **[Mail.](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** Naše smjernice osiguravaju provjeru autentičnosti pošiljatelja (potvrđuje da se domena pošiljatelja ne može smućiti). **Napomena:** ne preporučujemo upravljanje lažnim pozitivnim vrijednostima pomoću popisa sigurnih pošiljatelja jer iznimke od filtriranja neželjene pošte mogu otvoriti vašu organizaciju za sigurnosne napade. Ako vaši korisnici primaju poruke koje su pogrešno označene kao neželjena ili bezvrijedna e-pošta, **[prijavite poruke i datoteke Microsoftu.](https://protection.office.com/reportsubmission)**
- Sef Pošiljatelje u Outlook, popisu dopuštenih pošiljatelja ili popisu  dopuštenih domena u pravilnikima o zaštiti od neželjene pošte potrebno je izbjegavati jer pošiljatelji zaobilaze svu neželjenu poštu, podvala i phish zaštitu te provjeru autentičnosti pošiljatelja (SPF, DKIM, DMARC). Ta se metoda najbolje koristi samo za privremeno testiranje.
- Provjera valjanosti da je određena e-pošta zaobišla procjenu antispama može se obaviti provjerom zaglavlja poruke "X-Forefront-Antispam-Report" (SFV:SFE, SFV:SKA, SFV:SKN), pogledajte zaglavlja poruka o **[neželjenoj pošti](https://docs.microsoft.com/microsoft-365/security/office-365-security/anti-spam-message-headers)**.
- Budući da Microsoft po zadanom želi zaštiti naše [korisnike](https://docs.microsoft.com/microsoft-365/security/office-365-security/secure-by-default#exceptions), neka nadjačavanja klijenata ne primjenjuju se na zlonamjerni softver i krađu identiteta visoke pouzdanosti. Ta nadjačavanja obuhvaćaju sljedeće: o Dopuštene popise pošiljatelja ili dopuštene popise domena (pravilnike o neželjenoj pošti) o Outlook Sef Senders o IP Allow List (filtriranje veze) 
- Jedino nadjačavanje koje omogućuje da poruka o krađi identiteta radi zaobilaženje filtriranja Exchange pravila tijeka pošte (poznata i kao pravila prijenosa). Da biste zaobišli filtriranje pomoću pravila tijeka pošte, pogledajte korištenje pravila tijeka pošte da biste postavili razinu **[pouzdanosti neželjene pošte (SCL) u porukama](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-mail-flow-rules-to-set-the-spam-confidence-level-scl-in-messages)**.