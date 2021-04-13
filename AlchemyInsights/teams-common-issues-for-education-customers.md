---
title: Česti problemi u aplikaciji Teams za korisnike u obrazovnim ustanovama
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000701"
- "3831"
- "3832"
ms.openlocfilehash: 893c8cacaf089932014ba7a3ea6122d17da38cdd
ms.sourcegitcommit: ef7ec42aba3c06aa8966dfac71cec18c08e7acf8
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/13/2021
ms.locfileid: "51692386"
---
# <a name="teams-common-issues-for-education-customers"></a>Česti problemi u aplikaciji Teams za korisnike u obrazovnim ustanovama

**Za korisnike u obrazovnim ustanovama**:

Ako vam je potrebna pomoć pri implementaciji timova za podršku daljinskom učenju, posjetite [FastTrack Center](https://www.microsoft.com/fasttrack) da biste poslali zahtjev. Pročitajte sljedeće česte probleme u aplikaciji Teams za korisnike u obrazovnim ustanovama:

- Vidite poruku „**Propuštate!**”? Pobrinite se da [omogućite aplikaciju Microsoft Teams za svoju školu](https://docs.microsoft.com/microsoft-365/education/intune-edu-trial/enable-microsoft-teams). U EDU klijentima aplikacija Microsoft Teams nije omogućena prema zadanim postavkama; najprije ćete je morati uključiti.

- **Novi ste korisnik aplikacije Teams?** Pogledajte [Daljinsko podučavanje i učenje u sustavu Office 365 Education](https://support.office.com/article/remote-teaching-and-learning-in-office-365-education-f651ccae-7b65-478b-8366-51bb884025c4) da biste naučili najnovije savjete o postavljanju svoje škole, planiranju lekcija, virtualnim sastancima i zajedničkom korištenju sadržaja sa studentima.

- Kada se uključi, korisnici mogu pokretati aplikaciju Teams ili instaliranjem [stolnog računala](https://docs.microsoft.com/MicrosoftTeams/get-clients#desktop-client) i [mobilnih klijenata](https://docs.microsoft.com/MicrosoftTeams/get-clients#mobile-clients) ili iz preglednika na https://teams.microsoft.com.

- **Omogućavanje pristupa aplikaciji Teams za goste:** pogledajte [kontrolni popis za pristup aplikaciji Teams za goste](https://docs.microsoft.com/microsoftteams/guest-access-checklist) i provjerite jesu li svi koraci dovršeni.
    - [Upoznavanje s pristupom gosta u aplikaciji Microsoft Teams](https://docs.microsoft.com/microsoftteams/guest-access)
    - [Postavljanje – kontrolni popis za pristup gosta u aplikaciji Microsoft Teams](https://docs.microsoft.com/microsoftteams/guest-access-checklist)
    - [Način na koji se gost uključuje u Teams](https://docs.microsoft.com/microsoftteams/guest-joins)

- **Sastanci i uključivanje biranjem u programu Teams**: trebate pomoć pri uključivanju ili postavljanju audiokonferencija u programu Microsoft Teams? Je li ovaj korisnik nedavno stvoren? Ako jest, trebat ćete pričekati 2 do 24 sata da bi se postavke primijenile. Da biste potvrdili da je korisnik licenciran za audio konferenciju i da ima zadani broj uz plaćanje:
    1. Idite na Aktivne korisnike i odaberite odgovarajućeg korisnika.
    2. Ovisno o verziji centra za administratore, odaberite ili **Licence i aplikacije** ili kliknite **Uređivanje** u odjeljku **Licence za proizvode**.
    3. Potvrdite da korisnik ima odabrane licence za audiokonferencije, Microsoft Teams i Skype za tvrtke online (Plan 2).
    4. U centrima za administratore kliknite **Prikaži sve**, a zatim **Teams**.
    5. U centru za administratore programa Microsoft Teams kliknite **Naslijeđeni portal**.
    6. U centru za administratore sustava Skype za tvrtke kliknite **Audiokonferencije**, a zatim **Korisnici**.
    7. Odaberite odgovarajućeg korisnika i potvrdite da korisnik ima zadani broj uz plaćanje.

    Dodatne informacije potražite u odjeljku [Tarife za pozivanje](https://docs.microsoft.com/microsoftteams/calling-plans-for-office-365) aplikacije Microsoft Teams ili nazovite tim za naplatu za Microsoft Commerce da biste saznali više o pitanjima povezanima s licenciranjem.

    Dodatni resursi

    - [Sastanci i konferencije u aplikaciji Microsoft Teams](https://docs.microsoft.com/microsoftteams/deploy-meetings-microsoft-teams-landing-page)
    - [Audiokonferencije](https://docs.microsoft.com/microsoftteams/audio-conferencing-in-office-365)

- **Pravilnici za sastanke**: pravilnici za sastanke služe za kontrolu značajki dostupnih sudionicima sastanaka koje zakažu korisnici iz vaše tvrtke ili ustanove. Kada stvorite pravilnik i napravite promjene, možete mu dodijeliti korisnike.

    - **Promjena ili stvaranje pravilnika za sastanke**: da biste promijenili ili stvorili pravilnik za sastanke, idite na odjeljak **Centar za administratore aplikacije Microsoft Teams > Sastanci > Pravilnici za sastanke**. Odaberite pravilnik s popisa ili kliknite **Dodaj**. Ako stvarate novi pravilnik, dodajte mu naziv i opis. Naziv ne može sadržavati posebne znakove ni biti dulji od 64 znaka. Odaberite postavke, a zatim kliknite **Spremi**. 
    
        Recimo, primjerice, da imate velik broj korisnika i da želite ograničiti propusnost koju bi njihov sastanak zahtijevao. Stvorili biste novi prilagođeni pravilnik pod nazivom „Ograničena propusnost” i onemogućili ove postavke:

        U odjeljku **Audio i video**:
        - Isključite **Dopusti snimanje u oblaku**.
        - Isključite **Dopusti IP videozapise**.

        U odjeljku **Zajedničko korištenje sadržaja**:

        - Onemogućite način rada sa zajedničkim korištenjem zaslona.
        - Isključite **Dopusti zaslonsku ploču**.
        - Isključite **Dopusti zajedničke bilješke**.

        Potom **dodijelite pravilnik korisnicima**:

    1. U lijevom navigacijskom oknu centra za administratore aplikacije Microsoft Teams idite na odjeljak **Korisnici**, a zatim kliknite korisnika.
    2. Odaberite korisnika tako da kliknete lijevo od njegovog imena, a zatim kliknete **Uređivanje postavki**.
    3. U odjeljku **Pravilnik za sastanke** odaberite pravilnik koji želite dodijeliti i kliknite **Primijeni**.

    Da biste pravilnik istodobno dodijelili većem broju korisnika, pročitajte odjeljak [Skupno uređivanje korisničkih postavki za Teams](https://docs.microsoft.com/microsoftteams/edit-user-settings-in-bulk).

    Možete učiniti i sljedeće:
    1. U lijevom navigacijskom oknu centra za administratore programa Microsoft Teams idite na odjeljak **Sastanci > Pravilnici za sastanke**.
    2. Odaberite pravilnik tako da kliknete lijevo od njegovog naziva.
    3. Kliknite **Upravljanje korisnicima**.
    4. U oknu **Upravljanje korisnicima** potražite korisnika prema zaslonskom nazivu ili korisničkom imenu, odaberite ime, a zatim kliknite **Dodaj**. Ponovite taj korak za svakog korisnika kojeg želite dodati.
    5. Kada završite s dodavanjem korisnika, kliknite **Spremi**.

- **Otklanjanje poteškoća s nedostajućom tipkovnicom**:
    - Provjerite ima li korisnik dodijeljenu [licencu za aplikaciju Teams](https://docs.microsoft.com/MicrosoftTeams/assign-teams-licenses).
    - Provjerite je li korisniku dodijeljena [tarifa za pozive](https://docs.microsoft.com/MicrosoftTeams/calling-plan-landing-page).
    - Omogućite korisnike za [korporacijski govorni servis](https://docs.microsoft.com/skypeforbusiness/skype-for-business-hybrid-solutions/plan-your-phone-system-cloud-pbx-solution/enable-users-for-enterprise-voice-online-and-phone-system-voicemail#to-enable-your-users-for-phone-system-in-office-365-voice-and-voicemail).

- **Otklanjanje poteškoća s prijavom u aplikaciju Teams**: najprije provjerite je li [aplikacija Microsoft Teams u dobrom stanju](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/servicehealth). Zatim provjerite postoje li uobičajeni kodovi pogrešaka i pogledajte odjeljak [Zašto imam problema s prijavom u aplikaciju Microsoft Teams?](https://support.office.com/article/a02f683b-61a3-4008-9447-ee60c5593b0f) Možda ćete također morati pogledati odjeljak [Modeli identiteta i provjera autentičnosti u aplikaciji Microsoft Teams](https://docs.microsoft.com/MicrosoftTeams/identify-models-authentication).
