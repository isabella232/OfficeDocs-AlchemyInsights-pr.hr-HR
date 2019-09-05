---
title: Dodavanje vanjskog korisnika grupe raspodjele
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: e84a5b04d6fc805deaa47cb10c91081f37411e5b
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36737865"
---
# <a name="add-external-users-to-a-distribution-group"></a>Dodavanje vanjski korisnici grupe raspodjele

Dodavanje vanjskog kontakta za na raspodjele grupe (DG) je postupak u dva koraka:
  
1. Stvaranje pošte kontaktu za vanjske korisnika:
    
    1. U centru za administraciju Idi **korisnici** > stranica[kontakata](https://admin.microsoft.com/adminportal/home#/Contact) . 
    
    2. Odaberite **Dodaj kontakt**.
    
    3. Unesite informacije za vaš kontakt i odaberite **Dodaj**.
    
2. Dodavanje kontakta pošte vaše DG:
    
    1. U centru za administraciju Idi **grupe** > [grupe](https://admin.microsoft.com/adminportal/home#/groups) stranica. 
    
    2. Traži DG želite dodati vanjskog korisnika i odaberite ga da biste otvorili dijaloški okvir Uređivanje.
    
    3. Na kartici **Članovi** odaberite **Prikaz svih i upravljanje članovima**. 
    
    4. Odaberite **Dodaj članove**.
    
    5. Odaberite kontakt pošte stvorena na prethodni korak i odaberite **Spremi**.
    
Ako nakon ovih koraka vanjski korisnici pošta nije moguće poslati na DG ili ne primate pošta iz nje, to može biti u DG označen samo iz internim korisnicima dopustiti pošta. Provjerite konfiguraciju i popravite slijedeći upute [ovdje](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).
  
 **Napomena:** Te se upute ne primijenite ako je vaša grupa Vrsta "Office 365 grupa" umjesto "Grupu raspodjele." Ako je to slučaj, možete dodati vanjskog korisnika izravno na grupe iz programa Outlook. Detaljne informacije o Office 365 grupe Gosti i upute za dodavanje vanjskog Gosti mogu pronaći u [ovom članku](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).
  