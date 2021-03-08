---
title: Automatsko premještanje poruka e-pošte u arhivski poštanski sandučić
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100008"
- "7217"
ms.openlocfilehash: 14ded561ee2b3c244fadbdab42fd0e833a1c66d5
ms.sourcegitcommit: 7fa9bf6f9fc7438791aa9241a440e5be817d4401
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/08/2021
ms.locfileid: "50524097"
---
# <a name="automatically-move-email-messages-to-the-archive-mailbox"></a>Automatsko premještanje poruka e-pošte u arhivski poštanski sandučić

Slijede upute za postavljanje pravilnika da bi se korisnikova stara e-pošta automatski pomakila u poštanski sandučić arhive:

1. Idite na [**sigurnosnu &**](https://go.microsoft.com/fwlink/p/?linkid=2077143)  >  **arhivu upravljanje podacima**  >   o usklađenosti da biste potvrdili da je za korisnika omogućen arhivski poštanski sandučić. Ako nije, kliknite **Omogući** **da** u okviru upozorenje.
2. Otvorite [**centar za administratore sustava Exchange > upravljanje usklađivanjem > oznake zadržavanja**](https://go.microsoft.com/fwlink/?linkid=2059104).
3. Odaberite ikonu +, a zatim odaberite **automatski primijeni na cijeli poštanski sandučić**.
4. Dodijelite naziv oznake zadržavanja, a zatim odaberite **Premjesti u arhivu**. Za razdoblje zadržavanja unesite željeno vrijeme, kao što je 90 days. Kliknite **Spremi**.
5. Sada stvorite pravilnik o zadržavanju: odaberite **pravila zadržavanja**, odaberite ikonu da biste dodali novo pravilo.
6. Dodijelite naziv pravilima zadržavanja, a zatim kliknite, a zatim se pomaknite da biste pronašli i dodali oznaku zadržavanja koju ste upravo stvorili. Kliknite **Spremi**.
7. Konačno, primijenite pravilnik o zadržavanju na korisnikov poštanski sandučić: još uvijek u centru za administratore sustava Exchange idite na  >  **poštanske sandučiće** primatelja. Odaberite sve korisnike na koje želite primijeniti pravilo, a zatim odaberite **Uređivanje** (ikona olovke).
8. U dijaloškom okviru kliknite **značajke poštanskog sandučića**. U odjeljku **pravilnik o zadržavanju** primijenite pravilo koje ste upravo stvorili > **Spremanje**.
9. Upute za primjenu Pravilnika na sve korisnike potražite u članku [Primjena pravilnika o zadržavanju na poštanske sandučiće](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy).
