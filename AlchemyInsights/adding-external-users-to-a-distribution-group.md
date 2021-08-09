---
title: Dodavanje vanjskih korisnika u grupu za raspodjelu
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: d8c06c81ecc66df0fbaa4cac9908178cdc1d9c6bdc38d19010c7b55e9bca8776
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53934825"
---
# <a name="add-external-users-to-a-distribution-group"></a>Dodavanje vanjskih korisnika u grupu za raspodjelu

Dodavanje vanjskog kontakta u grupu za raspodjelu (DG) postupak je u dva koraka:
  
1. Stvaranje kontakta e-pošte za vanjskog korisnika:
    
    1. U centru za administratore idite na stranicu  >  [Kontakti korisnika.](https://admin.microsoft.com/adminportal/home#/Contact) 
    
    2. Odaberite **Dodaj kontakt**.
    
    3. Upišite podatke za kontakt i odaberite **Dodaj**.
    
2. Dodajte kontakt e-pošte glavnoj upravi:
    
    1. U centru za administratore idite na **stranicu**  >  [Grupe](https://admin.microsoft.com/adminportal/home#/groups) grupa. 
    
    2. Pronađite GLAVNU upravu u koju želite dodati vanjskog korisnika, a zatim ga odaberite da biste otvorili dijaloški okvir za uređivanje.
    
    3. Na kartici **Članovi odaberite** Prikaz **svih članova i upravljanje njima.** 
    
    4. Odaberite **Dodaj članove**.
    
    5. Odaberite kontakt e-pošte koji ste stvorili u prethodnom koraku, a zatim **Odaberite Spremi**.
    
Ako nakon sljedećih koraka vanjski korisnici ne mogu slati poruke e-pošte glavnoj upravi ili ne primaju poruke e-pošte od njega, možda je glavna uprava označena tako da dopušta samo poruke e-pošte internih korisnika. Tu konfiguraciju možete provjeriti i popraviti prema [uputama](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online)ovdje .
  
 **Napomena:** Ove se upute ne primjenjuju ako je vrsta grupe "Microsoft 365 grupa" umjesto "Grupa za raspodjelu". U tom slučaju vanjski korisnik možete dodati izravno u grupu iz Outlook. Detaljne informacije o Microsoft 365 grupama te upute za dodavanje vanjskih gostiju potražite u [ovom članku](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).
  