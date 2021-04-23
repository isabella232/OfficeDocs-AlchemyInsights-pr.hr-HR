---
title: Pravila zadržavanja u centru za administratore sustava Exchange ne rade
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
ms.openlocfilehash: bb2ce7ce2405be575dfdb79d304fef690e863a4e
ms.sourcegitcommit: e9206b7bb1bf2efd2471edbf4c60c00c3607bc41
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2021
ms.locfileid: "51952220"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Pravila zadržavanja u centru za administratore sustava Exchange

Ako želite da pokrenemo automatske provjere postavki navedenih u nastavku, odaberite gumb natrag <– pri vrhu ove stranice, a zatim unesite adresu e-pošte korisnika koji ima problema s pravilima zadržavanja.

Ako imate problema s pravilima zadržavanja u centru za administratore sustava Exchange koji se ne primjenjuju na poštanske sandučiće ili stavke koje se ne premještaju u arhivski poštanski sandučić, provjerite sljedeće:

**Korijenski uzroci:**

- **Pomoćnik za upravljane** mape nije obradio korisnikov poštanski sandučić. Pomoćnik za upravljane mape pokušava obraditi svaki poštanski sandučić u tvrtki ili ustanovi u oblaku jedanput svakih sedam dana.

  **Rješenje:** Pokrenite pomoćnik za upravljane mape.

- **ZadržavanjeDržanje** je **omogućeno u** poštanskom sandučiću. Ako je poštanski sandučić postavljen na čuvanje, pravilnik o zadržavanju u poštanskom sandučiću neće se obraditi tijekom tog razdoblja.

  **Rješenje:** Provjerite status postavke čuvanja zadržavanja i ažurirajte po potrebi. Detalje potražite u članku Čuvanje [zadržavanja poštanskog sandučića](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).
 
**Napomena:** Ako je poštanski sandučić manji od 10 MB, pomoćnik za upravljane mape neće automatski obraditi poštanski sandučić.
 
Dodatne informacije o pravilima zadržavanja u centru za administratore sustava Exchange potražite u članku:

- [Oznake zadržavanja i pravilniki o zadržavanju](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)

- [Primjena pravilnika o zadržavanju na poštanske sandučiće](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) [ili Dodavanje ili uklanjanje oznaka zadržavanja](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)

- [Kako prepoznati vrstu zadržavanja koja se nalazi na poštanskom sandučiću](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
