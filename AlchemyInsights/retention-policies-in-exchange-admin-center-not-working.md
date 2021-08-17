---
title: Pravila zadržavanja u Exchange centru za administratore ne rade
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 6652ad5fc1691e1d5a4293d81f3a649f23ec38f18c8ed9fe06665628a901d13e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54074924"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Pravila zadržavanja u centru Exchange administratora

Ako želite da pokrenemo automatske provjere postavki navedenih u nastavku, odaberite gumb natrag <– pri vrhu ove stranice, a zatim unesite adresu e-pošte korisnika koji ima problema s pravilima zadržavanja.

Ako imate problema s pravilnikom o zadržavanju u centru Exchange za administratore koji se ne primjenjuju na poštanske sandučiće ili stavke koje se ne premještaju u arhivski poštanski sandučić, provjerite sljedeće:

**Korijenski uzroci:**

- **Pomoćnik za upravljane** mape nije obradio korisnikov poštanski sandučić. Pomoćnik za upravljane mape pokušava obraditi svaki poštanski sandučić u tvrtki ili ustanovi u oblaku jedanput svakih sedam dana.

  **Rješenje:** Pokrenite pomoćnik za upravljane mape.

- **ZadržavanjeDržanje** je **omogućeno u** poštanskom sandučiću. Ako je poštanski sandučić postavljen na čuvanje, pravilnik o zadržavanju u poštanskom sandučiću neće se obraditi tijekom tog razdoblja.

  **Rješenje:** Provjerite status postavke čuvanja zadržavanja i ažurirajte po potrebi. Detalje potražite u članku Čuvanje [zadržavanja poštanskog sandučića](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).
 
**Napomena:** Ako je poštanski sandučić manji od 10 MB, pomoćnik za upravljane mape neće automatski obraditi poštanski sandučić.
 
Dodatne informacije o pravilima zadržavanja u centru Exchange za administratore potražite u sljedećem članku:

- [Oznake zadržavanja i pravilniki o zadržavanju](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)

- [Primjena pravilnika o zadržavanju na poštanske sandučiće](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) [ili Dodavanje ili uklanjanje oznaka zadržavanja](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)

- [Kako prepoznati vrstu zadržavanja koja se nalazi na poštanskom sandučiću](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
