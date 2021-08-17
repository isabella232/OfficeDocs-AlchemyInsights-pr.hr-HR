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
ms.openlocfilehash: 57dbfd116bbae227f2288ce23edeaaa833fadf54ca3b10b95c49512758542e32
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54059218"
---
# <a name="automatically-move-email-messages-to-the-archive-mailbox"></a>Automatsko premještanje poruka e-pošte u arhivski poštanski sandučić

Evo kako postaviti pravilnik za automatsko premještanje korisnikova stare e-pošte u arhivski poštanski sandučić:

1. Idite [**na Arhiviranje & usklađenosti**](https://go.microsoft.com/fwlink/p/?linkid=2077143)podataka o usklađenosti da biste provjerili je li za korisnika  >    >   omogućen arhivski poštanski sandučić. Ako nije, u okviru s **upozorenjem** **kliknite** Omogući, a zatim Da.
2. Idite na [**Exchange centra za administratore > usklađenosti > oznaka zadržavanja**](https://go.microsoft.com/fwlink/?linkid=2059104).
3. Odaberite ikonu + pa odaberite **automatski primijeni na cijeli poštanski sandučić**.
4. Dodijelite naziv oznaci zadržavanja pa odaberite **Premjesti u arhiviranje.** Za razdoblje zadržavanja unesite vrijeme koje želite, primjerice 90 dana. Kliknite **Spremi**.
5. Sada stvorite pravilnik o zadržavanju: **odaberite pravilnike zadržavanja**, odaberite ikonu da biste dodali novi pravilnik.
6. Dodijelite naziv pravilniku zadržavanja, a zatim kliknite i pomaknite se da biste pronašli i dodali oznaku zadržavanja koju ste upravo stvorili. Kliknite **Spremi**.
7. Naposljetku primijenite pravilnik o zadržavanju na korisnikov poštanski sandučić: i dalje u centru Exchange za administratore idite **na poštanske sandučiće**  >  **primatelja**. Odaberite sve korisnike na koje želite primijeniti pravilnik, a zatim odaberite **Uređivanje** (ikona olovke).
8. U dijaloškom okviru kliknite Značajke **poštanskog sandučića**. U **odjeljku Pravilnik o** zadržavanju primijenite pravilnik koji ste upravo stvorili > **Spremi**.
9. Upute za primjenu pravilnika na sve korisnike potražite u članku [Primjena pravilnika o zadržavanju na poštanske sandučiće](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy).
