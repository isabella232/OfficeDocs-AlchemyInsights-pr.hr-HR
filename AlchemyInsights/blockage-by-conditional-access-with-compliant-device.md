---
title: Blokira me uvjetni pristup s kompatibilnim uređajem
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
ms.openlocfilehash: 240bd25f4d62505202c8cd7ceabe4c1cd3d5c0b5
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035057"
---
# <a name="im-getting-blocked-by-conditional-access-with-compliant-device"></a>Blokira me uvjetni pristup s kompatibilnim uređajem

**Visoko preporučeni Alati**

- [Alat za otklanjanje poteškoća s registracijom uređaja](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) – sveobuhvatan alat koji olakšava otklanjanje poteškoća s najčešćih problema s registriranjem uređaja.
- [Testna skripta za povezivanje s uređajima](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) – alat koji se koristi da bi uređaj mogao pristupiti krajnjim točkama registracije uređaja u odjeljku sistemski račun.
- [Skripta za čišćenje servisa Azure ad](https://github.com/mzmaili/AzureADDeviceCleanup) – alat koji se koristi za traženje ustajalih uređaja u vašem okruženju.

Evo nekoliko običnih razloga zbog kojih uvjetni pristup može biti neuspješan za kompatibilan uređaj ili zbog čega korisnici mogu primati **te poruke ne možete dobiti od ovdje kada** je zahtjev za prijavu namijenjen resursu tvrtke ili ustanove.

1. **Uređaj nije u obaveznom stanju uređaja s MDM**-om:

Provjerite je li uređaj upisan u ovlašteni MDM davatelj usluge kao što je Intune i *označen kao sukladan*. Dodatne informacije o Intune potražite u ovom [dokumentu](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment). Da biste bolje razumjeli usklađenost uređaja i Intune, pročitajte članak [Korištenje pravilnika o usklađenosti da biste postavili pravila za uređaje kojima upravljate Intune](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started). Ako imate problema s upisivanjem uređaja s programom Intune, pronađite pojedinosti o otklanjanju poteškoća pri [rješavanju problema s uvrštanjem uređaja u programu Microsoft](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune). Za daljnju podršku za Intune stvorite zahtjev za podršku. Da biste to učinili, posjetite [stranicu za pomoć i podršku u sustavu Intune](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/SupportMenu/helpSupport).

2. **Sprava nije povezana s mrežom tvrtke ili ustanove**:

Da bi pristup organizacijskim resursima, uređaj mora biti povezan s mrežom tvrtke ili ustanove, putem izravne veze ili virtualne privatne mreže (VPN-a), a također se pridružio i programu Active Directory na servisu Azure. Da biste se uključili u radni uređaj u mrežu tvrtke ili ustanove, pogledajte odjeljak [pridruživanje radnom uređaju u mrežu tvrtke ili ustanove](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network). Da biste registrirali osobni/BYOD uređaj, pročitajte članak [Registracija osobnog uređaja na mreži tvrtke ili ustanove](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network).

- Da biste provjerili je li se uređaj pridružio mreži, slijedite korake za registrirane uređaje [ovdje ili na radnim uređajima](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network#to-verify-that-youre-registered) [ovdje](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network#to-make-sure-youre-joined). Da biste razradili problem s mrežnom povezivanjem tvrtke org, slijedite upute u nastavku:

    1. Prijavite se u sustav Windows pomoću računa za rad ili obrazovne ustanove, na primjer, alain@contoso.com.
    2. Povežite se s mrežom tvrtke ili ustanove putem VPN-a ili programa DirectAccess.
    3. Kada se povežete, pritisnite tipku s **logotipom sustava Windows + L** da biste zaključali uređaj.
    4. Otključaj uređaj pomoću računa za rad ili obrazovne ustanove, a zatim ponovno pokušajte pristupiti problematičnoj aplikaciji ili servisu.

Ako se ponovno prikaže poruka o pogrešci, problem je vjerojatno **na** drugom mjestu.

3. **Operacijski sustav nije podržan**:

Provjerite koristite li podržanu verziju operacijskog sustava, uključujući sljedeće:

- **Klijent sustava Windows**: Windows 7 ili noviji

- **Windows Server**: windows Server 2008 R2 ili noviji

- **makro**: MacOS X ili noviji

- **Android i iOS**: najnovija verzija operacijskog sustava Android i iOS za mobilne uređaje

4. **Web-preglednik nije podržan**:

Potražite podržane preglednike u nastavku. Za podršku za Chrome sa sustavom Windows 1703 ili novijim verzijama potreban je produžetak računa za Windows 10. Za Edge 85 + korisnik mora biti potpisan da bi pravilno položio informacije o usklađenosti uređaja. Dodatne [informacije potražite u članku.](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support)

- **Windows 10**: Microsoft Edge, Internet Explorer, Chrome
- **Windows 8/8,1**: Internet Explorer, Chrome
- **Windows 7**: Internet Explorer, Chrome
- **iOS**: Microsoft Edge, Intune Managed browserima, Safari
- **Android**: **Microsoft Edge**: Intune upravljani preglednik, Chrome
- **Telefon sa sustavom Windows**: Microsoft Edge, Internet Explorer
- **Windows Server 2019**: Microsoft Edge, Internet Explorer, Chrome
- **Windows Server 2016**: Internet Explorer
- **Windows Server 2012 R2**: Internet Explorer
- **Windows Server 2008 R2**: Internet Explorer
- **MacOS**: Chrome, Safari

Dodatne informacije potražite u članku **poruka i otklanjanje poteškoća u nastavku** [.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-device-remediation)
