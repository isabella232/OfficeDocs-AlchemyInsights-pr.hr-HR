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
ms.openlocfilehash: 03cfd2c576cb03cbefd524a4ab6f04e2ef1eebec
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663505"
---
# <a name="add-external-users-to-a-distribution-group"></a>Dodavanje vanjskih korisnika u grupu za raspodjelu

Dodavanje vanjskog kontakta u grupu za raspodjelu (DG) postupak je u dva koraka:
  
1. Stvaranje kontakta e-pošte za vanjskog korisnika:
    
    1. U centru za administratore otvorite stranicu kontakti **korisnika**  >  [Contacts](https://admin.microsoft.com/adminportal/home#/Contact) . 
    
    2. Odaberite **Dodaj kontakt**.
    
    3. Unesite podatke za kontakt i odaberite **Dodaj**.
    
2. Dodajte kontakt e-pošte u svoju DG:
    
    1. U centru za administratore otvorite stranicu **grupe**  >  [grupa](https://admin.microsoft.com/adminportal/home#/groups) . 
    
    2. Pronađite DG u koju želite dodati vanjskog korisnika, a zatim ga odaberite da biste otvorili dijaloški okvir Uređivanje.
    
    3. Na kartici **Članovi** odaberite **Prikaz svih članova i upravljanje njima**. 
    
    4. Odaberite **Dodaj članove**.
    
    5. Odaberite kontakt e-pošte koji ste stvorili u prethodnom koraku, a zatim odaberite **Spremi**.
    
Ako nakon sljedećih koraka vaši vanjski korisnici ne mogu slati poruke e-pošte upravi ili ne primaju poruke e-pošte s nje, moguće je da je DG označena samo da dopušta poruke e-pošte od internih korisnika. Tu konfiguraciju možete provjeriti i popraviti ga [uz upute za](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online)praćenje.
  
 **Upozorenje:** Ove se upute ne primjenjuju ako je vrsta grupe "Microsoft 365 Group" umjesto "grupa za raspodjelu". Ako je to slučaj, vanjski korisnik možete dodati izravno u grupu iz programa Outlook. Detaljne informacije o tvrtki Microsoft 365 Groups, kao i upute za dodavanje vanjskih gostiju možete pronaći u [ovom članku](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).
  