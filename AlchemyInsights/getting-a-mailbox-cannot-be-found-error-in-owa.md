---
title: 126 Pogreška pri dobivanju poštanskog sandučića nije pronađena u aplikaciji OWA?
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "126"
- "1600020"
ms.assetid: e85bffec-e5ad-418a-8561-dab6257e1864
ms.openlocfilehash: 6bab821aaa3b50c365ef5d25a61bca195c76d7ce
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/30/2021
ms.locfileid: "51426654"
---
# <a name="getting-a-mailbox-not-found-error-in-outlook-on-the-web"></a>Nije pronađena pogreška poštanskog sandučića u programu Outlook na webu?

Ako koristite Outlook na webu i  ne možete pronaći poštanski sandučić radi pogreške, račun koji ste koristili za povezivanje s programom Outlook na webu nema licencu za Exchange Online i stoga s računom nije povezan nijedan poštanski sandučić. Administrator može dodijeliti licencu vašem računu na sljedeći način:

1. Otvorite centar za administratore sustava [Microsoft 365](https://portal.office.com/adminportal/home#/homepage) i otvorite **odjeljak** Aktivni korisnici u odjeljku Korisnici, a zatim odaberite korisnika koji vidi pogrešku. 

2. Na stranici korisnika koja će  se otvoriti idite na  odjeljak Licence i aplikacije, odaberite odgovarajuću vrijednost Lokacije i dodijelite licencu koja sadrži Exchange Online (proširite licencu da biste vidjeli pojedinosti o njemu). Kada završite, kliknite **Spremi promjene**.

U nekim slučajevima, ako je licenca već dodijeljena korisničkom računu, uklanjanje i ponovno dodjeljivanje licence pridonosi rješavanju problema i pravilnom dodjeljivanju resursa u sustavu: 

- Provjerite jesu li vaše pretplate na M365 Exchange Online (i druge, ako imate neku) trenutnu i nisu nedavno istekle.

Kada provjerite nije li vaša pretplata istekla i dodijeljena mu je valjana licenca, može biti potrebno do 24 sata da se licenca dodijeli, pa ćete možda morati pričekati da se problem riješi. Dodatne informacije potražite u članku [Dodjela licenci i upravljanje njima.](https://docs.microsoft.com/deployoffice/overview-licensing-activation-microsoft-365-apps#assign-and-manage-licenses)