---
title: Saznajte tko je postavio prosljeđivanje na poštanskom sandučiću i kako
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: 7746e44a0ee5a4442051900985aab339b09652f08e412b02a02429c93cc7c107
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/11/2021
ms.locfileid: "57895171"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a>Saznajte tko je postavio prosljeđivanje na poštanskom sandučiću i kako

Ako je vanjsko prosljeđivanje postavljeno na poštanski sandučić, aktivnost se nadzirana obavlja u sklopu cmdleta **Set-Mailbox.** Evo kako pronaći aktivnost u zapisniku nadzora:

1. Učinite jednu od sljedećih akcija:
   - U Centar za usklađenost okruženja Microsoft 365 na <https://compliance.microsoft.com> idite na **Nadzor** \> **rješenja**. Možete i izravno pristupiti stranici **Nadzor** pomoću sustava <https://compliance.microsoft.com/auditlogsearch> .
   - Na portalu Microsoft 365 Defender idite <https://security.microsoft.com> na **Nadzor**. Možete i izravno pristupiti stranici **Nadzor** pomoću sustava <https://security.microsoft.com/auditlogsearch> .

   > [!NOTE]
   > Ako vidite obavijest da morate uključiti nadzor, odmah je uključite. Ako ta značajka nije uključena, rezultati pretraživanja neće moći povući podatke iz prethodnih datuma.

2. Na **stranici** Nadzor provjerite je li **odabrana** kartica Pretraživanje, a zatim konfigurirajte sljedeće postavke:
   - Odaberite raspon datuma/vremena u **okvirima Početak** **i** Kraj.
   - Provjerite sadrži **li okvir** Aktivnosti Prikaz rezultata za **sve aktivnosti**.

3. Kada završite, kliknite **Pretraživanje**. Aktivnosti se prikazuju na novoj stranici **pretraživanja nadzora.**

4. U rezultatima kliknite stupac **Aktivnost da biste** sortirati rezultate, a zatim potražite **unose za postavljanje poštanskog sandučića.**

5. Odaberite aktivnost u rezultatima da biste otvorili letak s detaljima. Da biste utvrdili je li aktivnost povezana s prosljeđivanjem e-pošte, morate pogledati pojedinosti o svakom zapisu nadzora:
   - **ObjectId**: vrijednost pseudonima izmijenjenog poštanskog sandučića.
   - **Parametri:** _ForwardingSmtpAddress označava_ odredišnu adresu e-pošte.
   - **UserId**: korisnik koji je konfigurirao prosljeđivanje e-pošte u poštanskom sandučiću u **polju ObjectId.**

Dodatne informacije potražite u članku [Određivanje tko je postavio prosljeđivanje e-pošte za poštanski sandučić.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox)
