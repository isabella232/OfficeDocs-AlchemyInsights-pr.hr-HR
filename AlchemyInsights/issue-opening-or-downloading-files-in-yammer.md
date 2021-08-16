---
title: Problem s otvaranjem ili preuzimanjem datoteka u Yammer
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
ms.openlocfilehash: cb32085d13cbb5f609b887fc2b63e7af5ae056eb49c121a21722a147c67e30d8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028242"
---
# <a name="issue-opening-or-downloading-files-in-yammer"></a>Problem s otvaranjem ili preuzimanjem datoteka u Yammer

Klasični Yammer podržava više mogućnosti prijenosa datoteka u poruke i grupe. Ovisno o konfiguraciji mreže, datoteke su zadane za pohranu u SharePoint.

Odabir datoteke u novom Yammer još ne podržava sve mogućnosti dostupne u klasičnom Yammer. Buduće ažuriranje dodat će dodatne značajke. Dodatne informacije potražite u članku [Prilaganje datoteke ili slike u objavu Yammer razgovora](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-conversation-post-8d2d17f7-8f37-4535-961e-518d751be7e8).

**Nije moguće otvoriti ili preuzeti datoteku**  

Datoteka se može prenijeti na Yammer ali se povezuje i s datotekom u web-SharePoint Online. Da biste otklonili poteškoće, najprije morate odrediti mjesto datoteke. Ako je datoteka prenesena na Yammer, ona će imati URL yammer.com *.yammer.com. Provjerite jesu li obavezni URL-ovi i IP adrese deblokirani. Dodatne informacije potražite u članku Blog [Using hard coded IP addresses for Yammer not recommended](https://techcommunity.microsoft.com/t5/yammer-blog/using-hard-coded-ip-addresses-for-yammer-is-not-recommended/ba-p/276592).

Provjerite može li korisnik koji je i globalni administrator preuzeti datoteku. Ako je datoteka privatna, možda ćete morati koristiti način rada privatnog sadržaja. Dodatne informacije potražite u članku Praćenje [privatnog sadržaja u programu Yammer](https://docs.microsoft.com/yammer/manage-security-and-compliance/monitor-private-content).  

**Yammer mrežnih gostiju i datoteka na web-mjestu SharePoint Online**  

[Gosti na razini mreže u sustavu Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#invite-guests) ne koriste Azure AD B2B i interni su na servisu Yammer, pa ne mogu pristupati datotekama Yammer pohranjenim u SharePoint. Stvorite vanjskog AAD B2B korisnika koji može pristupati bibliotekama dokumenata u web-aplikaciji SharePoint Online pomoću tog identiteta. Informacije o budućoj podršci za goste servisa Azure AD B2B u aplikaciji Yammer potražite u članku Podrška za goste tvrtke [(B2B)](https://docs.microsoft.com/yammer/get-started-with-yammer/azure-ad-b2b-guests-yammer)u sustavu Yammer Preview – Korisničke odredbe i najčešća pitanja .