---
title: Otvaranje i preuzimanje datoteka u servisu Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6041"
- "9003112"
ms.openlocfilehash: de335e27624caf5a91bdc2913570eba92f627282
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695641"
---
# <a name="issue-opening-or-downloading-files-in-yammer"></a>Otvaranje i preuzimanje datoteka u servisu Yammer

Klasični Yammer podržava više mogućnosti za prijenos datoteka na poruke i grupe. Ovisno o konfiguraciji mreže, datoteke će biti zadane za pohranu u sustavu SharePoint.

Birač datoteka u novom Yammeru još ne podržava sve mogućnosti dostupne u klasičnom Yammeru. Ubuduće će se ažurirati dodavanjem dodatnih značajki. Dodatne informacije potražite u članku [prilaganje datoteke ili slike u objavu razgovora u servisu Yammer](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-conversation-post-8d2d17f7-8f37-4535-961e-518d751be7e8).

**Nije moguće otvoriti ili preuzeti datoteku**  

Datoteka se može prenijeti na Yammer, ali i povezati se s datotekom u sustavu SharePoint online. Da biste otklonili poteškoće, najprije morate odrediti mjesto datoteke. Ako je datoteka prenesena na Yammer, imat će URL *. yammer.com. Provjerite jesu li obavezni URL-ovi i IP adrese neblokirani. Dodatne informacije potražite u članku objava bloga [pomoću tvrdih kodirane IP adrese za Yammer](https://techcommunity.microsoft.com/t5/yammer-blog/using-hard-coded-ip-addresses-for-yammer-is-not-recommended/ba-p/276592).

Provjerite je li korisnik koji je također globalni administrator mogao preuzeti datoteku. Ako je datoteka privatna, možda ćete morati koristiti način osobnog sadržaja. Dodatne informacije potražite [u članku praćenje privatnog sadržaja u servisu Yammer](https://docs.microsoft.com/yammer/manage-security-and-compliance/monitor-private-content).  

**Gosti i datoteke na razini servisa Yammer u sustavu SharePoint Online**  

[Gosti na razini mreže u servisu Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#invite-guests) ne koriste tvrtke Azure ad B2B i interni su za servis servisa Yammer, tako da ne mogu pristupiti datotekama servisa Yammer pohranjenima u sustavu SharePoint. Stvaranje vanjskog servisa AAD B2B korisnika koji može pristupati bibliotekama dokumenata u sustavu SharePoint Online pomoću tog identiteta. Informacije o budućoj podršci za podršku za Azure AD B2B u servisu Yammer potražite [u članku Podrška za tvrtke – poslovno (B2B) u pretpregledu servisa Yammer – uvjeti kupaca i najčešća pitanja](https://docs.microsoft.com/yammer/get-started-with-yammer/azure-ad-b2b-guests-yammer).