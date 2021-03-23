---
title: Blokira mi se uvjetni pristup pomoću uređaja za priključene domene
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/20/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9834"
- "9003257"
ms.openlocfilehash: 052311ffe71bcb65de2b5c2a964932b1fb99c373
ms.sourcegitcommit: c34ba92e19419dcb2d251b8a1afe4d180a939617
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/20/2021
ms.locfileid: "51035233"
---
# <a name="im-getting-blocked-by-conditional-access-with-domain-joined-device"></a>Blokira mi se uvjetni pristup pomoću uređaja za priključene domene

**Visoko preporučeni Alati**

[Alat za otklanjanje poteškoća s registracijom uređaja](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) – alat koji olakšava otklanjanje poteškoća s najčešćih problema s registracijom uređaja.

[Testna skripta za povezivanje s uređajem za registraciju](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) – skripta koja omogućuje pristup krajnjim točkama registracije uređaja u odjeljku sistemski račun.

[Skripta za čišćenje servisa Azure ad](https://github.com/mzmaili/AzureADDeviceCleanup) -skripta koja omogućuje traženje i upravljanje ustajalim uređajima u vašem okruženju.

Evo nekoliko običnih razloga zbog kojih uvjetni pristup možda ne uspijeva na uređaju koji se pridružio domeni (Hybrid Azure AD).

1. **Na uređaju nema servisa Azure ad PRT** , morate osigurati da uređaj ima token za primarni osvježavanje za Azure AD (prt). Dodatne informacije o PRT-u potražite u ovom [dokumentu](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).

Da biste provjerili imate li Azure AD PRT, možete pokrenuti `dsregcmd/status` naredbu na uređaju i provjeriti je li "AzureAdPrt" jednako "da".

Ako je "AzureAdPrt" "ne", provjerite sljedeće:

- Bez obzira na to imate li **udruženu okolinu sa programom AD FS, a nedostupna je iz kućnih mreža vaših korisnika**: u ovom slučaju provjerite jesu li krajnje točke "usernazivno" podijeljene u programu extranet dostupne. Ako je vaš AD FS iza VPN-a, pobrinite se da se korisnici povezuju s VPN-om i ponovno se prijave na uređaj. Dodatne informacije potražite u ovom [dokumentu](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains).

- **Bez obzira na to je li TPM neispravan i time ne može potvrditi autentičnost uređaja**: Potvrdite "TPM. msc" da biste provjerili je li stanje TPM-a "spremno". Ako ne, pokrenite `dsregcmd/leave` i pustite da se uređaj ponovno pridruži Azure ad-u. Zatim pokušajte ponovno. Dodatne informacije potražite u ovom [dokumentu](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).

- **Koristite davatelja usluge trećih strana, koji ne podržava WS-Trust Protocol**. Kao što je opisano u našim dokumentima, Hybrid Azure AD-pridruženi uređaji ne mogu raditi u ovom slučaju. Suradite s pružateljem identiteta radi podrške.

2. **Korisnici koriste preglednik Chrome bez računa sustava Windows 10** ili **ekstenzije sustava Office Chrome ne koristi automatski prt na AAD-u ili HIBRIDNU-AAD-kompatibilnim uređajima**: to dovodi do neuspjeha bilo koje pravilnike o uvjetnom pristupu utemeljenoj na uređaju, s prikazanim porukama o pogrešci "neregistrirani uređaj". Da biste ispravno koristili preglednik Chrome, morate instalirati "računi u sustavu Windows 10" ili "ekstenziju sustava Office u pregledniku Chrome" Via SCCM ili Intune. Dodatne informacije potražite u ovom [dokumentu](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support).

Ako nije moguće pritisnuti daljinsko proširenje, obavijestite korisnike da ručno instaliraju neku od navedenih proširenja da bi pristupili aplikacijama iza uvjetnog pristupa utemeljenog na uređaju. Dodatne informacije potražite u ovom [dokumentu](https://docs.microsoft.com/azure/active-directory/conditional-access/require-managed-devices#prerequisites).

3. **Uređaj je ispravno spojen hibridni Azure AD, ali je nehotice izbrisano ili onemogućeno, bilo zbog sinkronizacije promjena u servisu Azure ad Connect ili s portala Azure**: ako se to dogodi, objekt Device više nije prepoznat kao potpuno spojeni uređaj, iako se status "Azureadconnector" i "prt" prikazuje kao valjano na uređaju.

Da biste riješili taj problem, pokrenite se `dsregcmd/leave` na pogođenim uređajima i pustite ih da se vrate u Azure AD. Dodatne informacije potražite u ovom [dokumentu](https://docs.microsoft.com/azure/active-directory/devices/faq#q-why-do-my-users-see-an-error-message-saying-your-organization-has-deleted-the-device-or-your-organization-has-disabled-the-device-on-their-windows-10-devices).

> [!NOTE]
> Ako su vaši uređaji u sustavu Windows 10, 1809 Update, uz VPN/Cloud proxy i pogledajte probleme s stanjem "AzureAdPrt" ili bilo kojom aplikacijom sa sustavom SSO (Outlook ne povezuje se s poštanskim sandučićem iako ste imali PRT), provjerite imate li tu zakrpu [KB4554354](https://support.microsoft.com/topic/march-30-2020-kb4554354-os-build-17763-1132-deaba49b-4b29-55b9-caee-3e2d87dd75a2) ili Travanj Kumulativno ažuriranje [KB4549949](https://support.microsoft.com/topic/april-14-2020-kb4549949-os-build-17763-1158-76d9a3af-b20b-8996-bd4d-7b50c505fda6) da biste spriječili pogreške prt-a na tim uređajima.

















