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
ms.openlocfilehash: a1c4c4d2fadaf75eda9b5b322aca35c32dfee8ea
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51792124"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a>Morate označiti domenu ili pošiljatelja e-pošte sigurnim?

- Korištenje popisa **sigurnih pošiljatelja ne preporučuje** se jer se u tvrtki ili ustanovi otvara neželjena pošta, fazani i lažni napadi.
- No ako postoji poslovni preduvjet, **preporučujemo** da za to koristite **[pravila tijeka](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** pošte. Naše smjernice osiguravaju provjeru autentičnosti pošiljatelja (potvrđuje da se domena pošiljatelja ne može smućiti). **Napomena:** ne preporučujemo upravljanje lažnim pozitivnim vrijednostima pomoću popisa sigurnih pošiljatelja jer iznimke od filtriranja neželjene pošte mogu otvoriti vašu organizaciju za sigurnosne napade. Ako vaši korisnici primaju poruke koje su pogrešno označene kao neželjena ili bezvrijedna e-pošta, **[prijavite poruke i datoteke Microsoftu.](https://protection.office.com/reportsubmission)**
- Sigurni pošiljatelji u programu Outlook, popis dopuštenih pošiljatelja  ili popis dopuštenih domena u pravilima za zaštitu od neželjene pošte moraju se izbjegavati jer pošiljatelji zaobilaze svu neželjenu poštu, podvala i phish zaštitu te provjeru autentičnosti pošiljatelja (SPF, DKIM, DMARC). Ta se metoda najbolje koristi samo za privremeno testiranje.
