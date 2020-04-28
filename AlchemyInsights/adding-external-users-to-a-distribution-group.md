---
title: Dodavanje vanjskih korisnika u grupu za raspodjelu
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: 7dbc69bced9ca800d3f95081b77dda5e49662579
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/27/2020
ms.locfileid: "43910924"
---
# <a name="add-external-users-to-a-distribution-group"></a>Dodavanje vanjskih korisnika u grupu za raspodjelu

Dodavanje vanjskog kontakta u grupu za raspodjelu (DG) postupak je u dva koraka:
  
1. Stvaranje kontakta e-pošte za vanjskog korisnika:
    
    1. U centru za administratore otvorite stranicu **Kontakti** > [korisnika.](https://admin.microsoft.com/adminportal/home#/Contact) 
    
    2. Odaberite **Dodaj kontakt**.
    
    3. Upišite podatke za svoj kontakt i odaberite **Dodaj**.
    
2. Dodajte kontakt e-pošte u dg:
    
    1. U centru za administratore idite na stranicu **Grupe grupa.** > [Groups](https://admin.microsoft.com/adminportal/home#/groups) 
    
    2. Pronađite GG kojem želite dodati vanjskog korisnika i odaberite je da biste otvorili dijaloški okvir za uređivanje.
    
    3. Na kartici **Članovi** odaberite **Prikaži sve i upravljaj članovima**. 
    
    4. Odaberite **Dodaj članove**.
    
    5. Odaberite kontakt pošte koji ste stvorili u prethodnom koraku, a zatim odaberite **Spremi**.
    
Ako nakon ovih koraka vanjski korisnici ne mogu slati e-poštu GU-u ili ne primaju poruke e-pošte od nje, moguće je da je GU označen tako da dopušta samo e-poštu od internih korisnika. Možete provjeriti ovu konfiguraciju i popraviti ga slijedeći upute [ovdje](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).
  
 **Napomena:** Te se upute ne primjenjuju ako je vrsta grupe "Grupa Microsoft 365" umjesto "Grupa za distribuciju". Ako je to slučaj, vanjski korisnik možete dodati izravno u grupu iz programa Outlook. Detaljne informacije o gostima grupa ci35 grupa kao i upute za dodavanje vanjskih gostiju možete pronaći u [ovom članku](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).
  