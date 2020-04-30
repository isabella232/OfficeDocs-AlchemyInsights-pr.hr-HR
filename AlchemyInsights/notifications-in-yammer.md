---
title: Obavijesti na servisu Yammer
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002878"
- "5480"
ms.openlocfilehash: ff4c13560b9cbf283e5c6b92a259debdf96cca62
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: HT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/27/2020
ms.locfileid: "43911895"
---
# <a name="notifications-in-yammer"></a>Obavijesti na servisu Yammer

Da bi vas upozorio na novu aktivnost u relevantnim razgovorima, [Yammer šalje obavijesti](https://support.microsoft.com/en-gb/office/enable-or-disable-yammer-email-and-phone-notifications-93e530e0-189f-4768-8f28-7683d48cc996) ili e-poštom ili s pomoću proslijeđenih obavijesti ako Yammer upotrebljavate na mobilnom uređaju. Yammer vam prema zadanim postavkama šalje obavijesti za mnogo vrsta aktivnosti u vašoj mreži. Korisnici mogu ažurirati postavke e-pošte putem web-mjesta servisa Yammer, a upute za proslijeđene obavijesti konfiguriraju se u mobilnoj aplikaciji. 

Yammer je dodao podršku za [interaktivne poruke e-pošte u programu Outlook](https://techcommunity.microsoft.com/t5/outlook-blog/interactive-yammer-emails-in-outlook-on-the-web-are-here/ba-p/1209420). Neke će poruke e-pošte (kopija poruke) postati interaktivne unutar programa Outlook na webu. Ta će se mogućnost u okviru budućih ažuriranja dodati u druge verzije programa Outlook.

**Vrste obavijesti na servisu Yammer**

- Poruke e-pošte (Ažuriranja iz grupe, netko vas poziva u grupu, primate poruku u ulaznoj pošti itd.)
- Proslijeđene obavijesti (Poslane su na mobilne uređaje kada se spominjete, primate poruku u ulaznoj pošti itd.)
- Skočni prozori na radnoj površini (Kada je instalirana aplikacija Yammer na radnoj površini, prikazat će se obavijesti za korisnike pod nazivom „skočna pločica”.)
- Obavijesti u obliku zvona (Korisnici će vidjeti obavijesti za različite događaje unutar web-mjesta servisa Yammer.) Ove obavijesti ne moraju uvijek imati povezanu poruku e-pošte ili proslijeđenu obavijest.

Dostupno je više [detaljnih informacija o obavijestima](https://support.microsoft.com/en-gb/office/enable-or-disable-yammer-email-and-phone-notifications-93e530e0-189f-4768-8f28-7683d48cc996).

**Upravljanje obavijestima**

Korisnici moraju upravljati vlastitim obavijestima. Informacije se nalaze na stranici [kako omogućiti i onemogućiti obavijesti e-poštom i mobilne obavijesti servisa Yammer](https://support.microsoft.com/en-gb/office/enable-or-disable-yammer-email-and-phone-notifications-93e530e0-189f-4768-8f28-7683d48cc996). 

Administratori ne mogu onemogućiti sve obavijesti ili upravljati obavijestima u ime korisnika. Administratori mogu [upravljati logotipom u porukama e-pošte i time trebaju li korisnici potvrditi poruke](https://docs.microsoft.com/yammer/configure-your-yammer-network/configure-email-and-yammer) poslane e-poštom.

**Obavijesti e-poštom poslane mnogim korisnicima u vašoj tvrtki ili ustanovi**

Yammer ponekad šalje samo jednu obavijest e-poštom, a prima je puno više korisnika u vašoj tvrtki ili ustanovi no što je očekivano. To se događa kada se u Yammer doda popis za raspodjelu ili druga vrsta nepojedinačne adrese e-pošte. Yammer ne zna u svim slučajevima pripada li adresa e-pošte jednom korisniku ili je riječ o adresi e-pošte preko koje će se jedna poruka e-pošte poslati mnogim primateljima. Kada se pojavi taj problem, morate poduzeti radnju da biste na servisu Yammer [suspendirali (deaktivirali) korisnika koji nije valjan s tom adresom e-pošte](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users). 

Da biste smanjili mogućnost pojavljivanja tog problema, trebali biste:

1. [primijeniti identitet sustava Office 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity) za Yammer.
2. Blokirajte vanjske pošiljatelje u slanju e-pošte u tvrtku ili ustanovu ili ograničite pošiljatelje na popis koji je odobren.

Ako se taj problem pojavi:

1. identificiranje primatelja e-pošte, koji bi trebao odgovarati korisniku na servisu Yammer. All-in-sales@fabrikam.com je, primjerice, DL za sve prodajne osobe. Taj bi se DL mogao prepoznati iz e-pošte servisa Yammer koju prime korisnici.
2. S pomoću značajke [deaktivacije (suspendiranja) u mrežnom administratoru](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users) suspendirajte korisnika s adresom e-pošte all-in-sales@fabrikam.com. Suspenziju je moguće poništiti pa je sigurnija nego brisanje. Korisnik se automatski briše nakon 90 dana.
3. Ako želite, pregledajte [Izvoz korisnika](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data#ExportUsers) da biste identificirali druge adrese e-pošte koje nisu korisničke i koje bi trebalo suspendirati.
