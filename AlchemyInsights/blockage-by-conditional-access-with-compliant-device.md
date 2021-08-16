---
title: Uvjetni pristup blokira me sa kompatibilnim uređajem
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9835"
- "9003257"
ms.openlocfilehash: 709749b1a62f2d9cdabfb3fe4b7538c22101d7109204d9163f6059336b817bf8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54019140"
---
# <a name="im-getting-blocked-by-conditional-access-with-compliant-device"></a>Uvjetni pristup blokira me sa kompatibilnim uređajem

**Preporučeni alati**

- [Alat za otklanjanje poteškoća s registracijom](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) uređaja – sveobuhvatan alat koji olakšava otklanjanje najčešćih problema s registracijom uređaja.
- [Probna skripta za povezivanje s registracijom](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) uređaja – alat koji se koristi za pristup krajnjim točkama registracije uređaja na računu sustava.
- [Skripta za čišćenje uređaja azure AD](https://github.com/mzmaili/AzureADDeviceCleanup) – alat koji se koristi za traženje i upravljanje uređajima u zastojima u vašem okruženju.

Evo nekih uobičajenih razloga zbog kojih uvjetni pristup možda ne uspijeva  za kompatibilni uređaj ili zašto korisnici primaju Poruku ne možete dobiti iz ove poruke tijekom zahtjeva za prijavu u resurs tvrtke ili ustanove.

1. **Uređaj nije u stanju obaveznog uređaja s MDM-om:**

Provjerite je li uređaj prijavljen kod odobrenog davatelja MDM-a kao što je Intune i označen *kao usklađen*. Dodatne informacije o programu Intune potražite u ovom [dokumentu](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment). Da biste bolje razumjeli usklađenost uređaja i Intune, pogledajte korištenje pravilnika usklađenosti za [postavljanje pravila za uređaje kojima upravljate s programom Intune](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started). Ako imate problema s registracijom uređaja pomoću aplikacije Intune, pojedinosti o otklanjanju poteškoća potražite u otklanjanje [poteškoća s prijavom uređaja u Microsoft.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) Za dodatnu podršku za Intune stvorite zahtjev za podršku. Da biste to učiniti, posjetite stranicu Pomoć i podrška za [Intune](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/SupportMenu/helpSupport).

2. **Uređaj nije pridružen mreži tvrtki ili ustanova:**

Da biste pristupili resursima tvrtke ili ustanove, uređaj mora biti povezan s mrežom tvrtke ili ustanove putem izravne veze ili virtualne privatne mreže (VPN-a) i pridružiti se lokalnoj ili Azure Active Directory. Da biste se pridružili poslovnom uređaju u mrežu tvrtke ili ustanove, pogledajte u članku Pridruživanje [poslovnom uređaju u mrežu tvrtke ili ustanove](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network). Da biste registrirali osobni/BYOD uređaj, [pogledajte Registracija osobnog uređaja na mreži tvrtke ili ustanove.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network)

- Da biste provjerili je li uređaj spojen s mrežom, slijedite upute za registrirane uređaje [ovdje ili](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network#to-verify-that-youre-registered) radne [uređaje ovdje](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network#to-make-sure-youre-joined). Da biste obuhvatli problem s mrežnom vezom tvrtke ili e-aplikacije Org, slijedite smjernice u nastavku:

    1. Prijavite se da Windows pomoću računa za posao ili školu, primjerice alain@contoso.com.
    2. Povezivanje na mrežu tvrtke ili ustanove putem VPN-a ili DirectAccessa.
    3. Kada se povežete, pritisnite tipku **Windows + L da biste** zaključali uređaj.
    4. Otključajte uređaj pomoću računa za posao ili školu, a zatim pokušajte ponovno pristupiti problematičnoj aplikaciji ili servisu.

Ako vam se pojavi **poruka o pogrešci** Ne možete doći iz ove poruke o pogrešci, problem je vjerojatno negdje drugdje.

3. **Operacijski sustav nije podržan:**

Provjerite koristite li podržanu verziju operacijskog sustava, uključujući sljedeće:

- **Windows klijent**: Windows 7 ili novija

- **Windows Server**: Windows Server 2008 R2 ili noviji

- **macOS**: macOS X ili noviji

- **Android i iOS**: najnovija verzija mobilnih operacijskih sustava Android i iOS

4. **Web-preglednik nije podržan:**

U nastavku pronađite podržane preglednike. Za podršku za Chrome s Windows 1703 ili novijim verzijama potrebno je Windows 10 za račune. Za Edge 85+, korisnik mora biti prijavljen da bi pravilno prošao podatke o usklađenosti uređaja. Dodatne informacije potražite [ovdje](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support).

- **Windows 10**: Microsoft Edge, Internet Explorer, Chrome
- **Windows 8 / 8.1**: Internet Explorer, Chrome
- **Windows 7**: Internet Explorer, Chrome
- **iOS**: Microsoft Edge, Upravljani preglednik Intune, Safari
- **Android**: **Microsoft Edge**: Intune Managed Browser, Chrome
- **Windows Phone**: Microsoft Edge, Internet Explorer
- **Windows Server 2019**: Microsoft Edge, Internet Explorer, Chrome
- **Windows Server 2016**: Internet Explorer
- **Windows Server 2012 R2**: Internet Explorer
- **Windows Server 2008 R2**: Internet Explorer
- **macOS**: Chrome, Safari

Dodatne informacije o uputama **za otklanjanje poteškoća** potražite u nastavku. [](https://docs.microsoft.com/azure/active-directory/user-help/user-help-device-remediation)
