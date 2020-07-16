---
title: Problem s otvaranjem ili preuzimanjem datoteka na sustavu Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6041"
- "9003112"
ms.openlocfilehash: 6dfcbe9abfc23219a61e81785d31c11f7a0fa95c
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148184"
---
# <a name="issue-opening-or-downloading-files-in-yammer"></a>Problem s otvaranjem ili preuzimanjem datoteka na sustavu Yammer

Klasični Yammer podržava više mogućnosti za prijenos datoteka u poruke i grupe. Ovisno o konfiguraciji mreže, datoteke zadane za pohranu u sustavu SharePoint.

Birač datoteka u novom programu Yammer još ne podržava sve mogućnosti dostupne u klasičnom programu Yammer. Buduće ažuriranje dodat će dodatne značajke. Dodatne informacije potražite u [odjeljku Prilaganje datoteke ili slike objavi razgovora na yammeru](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-conversation-post-8d2d17f7-8f37-4535-961e-518d751be7e8).

**Nije moguće otvoriti ili preuzeti datoteku**  

Datoteka se može prenijeti na Yammer, ali se povezuje i s datotekom u sustavu SharePoint Online. Da biste otklonili poteškoće, najprije morate odrediti mjesto datoteke. Ako je datoteka prenesena na Yammer, imat će *.yammer.com URL. Provjerite jesu li potrebni URL-ovi i IP adrese deblokirani. Dodatne informacije potražite u članku na blogu [Korištenje tvrdih kodiranih IP adresa za Yammer ne preporučuje se](https://techcommunity.microsoft.com/t5/yammer-blog/using-hard-coded-ip-addresses-for-yammer-is-not-recommended/ba-p/276592).

Provjerite može li korisnik koji je također globalni administrator preuzeti datoteku. Ako je datoteka privatna, možda ćete morati koristiti način privatnog sadržaja. Dodatne informacije potražite [u odjeljku Nadzor privatnog sadržaja na web-mjestu Yammer](https://docs.microsoft.com/yammer/manage-security-and-compliance/monitor-private-content).  

**Gosti i datoteke na razini mreže servisa Yammer u sustavu SharePoint Online**  

[Gosti na razini mreže na servisu Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#invite-guests) ne koriste Azure AD B2B i interni su za servis Servisa Yammer pa ne mogu pristupiti datotekama servisa Yammer pohranjenima u sustavu SharePoint. Pomoću tog identiteta stvorite vanjskog korisnika AAD B2B koji može pristupiti bibliotekama dokumenata u sustavu SharePoint Online pomoću tog identiteta. Informacije o budućoj podršci za goste za Azure AD B2B na servisu Yammer potražite u članku [Podrška za korisnike između tvrtke (B2B) u pretpregledu servisa Yammer – Uvjeti i najčešća pitanja o klijentima](https://docs.microsoft.com/yammer/get-started-with-yammer/azure-ad-b2b-guests-yammer).