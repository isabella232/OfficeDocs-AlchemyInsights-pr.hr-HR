---
title: DataProtection - Bitlocker
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1802"
- "9000220"
ms.openlocfilehash: 3f6e48b9d2f7562d74d60c2901759a7ab359e5c67bd4aa2d556d941a41ab680c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54118566"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Omogućivanje bitlocker šifriranja pomoću aplikacije Intune

Intune Endpoint Protection Policy može se koristiti za konfiguriranje postavki bitlocker šifriranja za Windows uređaje. Dodatne informacije potražite u [članku Windows 10 (i novije) postavke za zaštitu uređaja pomoću aplikacije Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).

Uz pravilnik o zaštiti krajnjih točaka nalazi se i izvješće o šifriranju koje pruža detaljniji prikaz statusa šifriranja za uređaje. Ovom se izvješću može pristupiti s mem portala u odjeljku **Uređaji > Monitor**, a zatim u odjeljku Konfiguracija **odaberite** [Izvješće šifriranja](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/DevicesMonitorMenu/encryptionReport).

Ako otkrijete da Bitlocker ne uspijeva biti omogućen na očekivani način ili da je profil koji se koristi za omogućivanje značajke Bitlocker u stanju pogreške, pregledajte izvješće o šifriranju da biste bolje razumjeli zašto se ponašanje odvija.

Detalje o tumačenju izvješća, uključujući različite vrijednosti statusa šifriranja, potražite u članku [Praćenje šifriranja uređaja pomoću uređaja Intune](https://docs.microsoft.com/mem/intune/protect/encryption-monitor).

Imajte na umu da mnogi noviji uređaji sa sustavom Windows 10 podržavaju automatsko bitlocker šifriranje, koje se pokreće bez primjene pravilnika MDM-a. To može utjecati na primjenu pravilnika ako nisu zadane postavke konfigurirane. Dodatne pojedinosti potražite u sljedećim najčešćim pitanjima.

Informacije o otklanjanju poteškoća sa značajkom bitlocker potražite u [članku Otklanjanje poteškoća s pravilnikom](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies)značajke BitLocker Microsoft Intune .
 
 
**Najčešća pitanja**

P: Koja izdanja Windows podržavaju šifriranje uređaja pomoću pravilnika za zaštitu krajnjih točaka?<br>
O: Postavke u pravilniku o zaštiti krajnjih točaka u aplikaciji Intune implementira se pomoću [bitlocker CSP-a.](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp) Ne podržavaju sva izdanja ni međuverzije Windows bitlocker CSP. <br><br>

P: Kako se Bitlocker može omogućiti na uređajima bez potrebe za interakciji krajnjih korisnika?<br>
O: Ako su ispunjeni potrebni preduvjeti, bitlocker "Silent Encryption" možete omogućiti putem aplikacije Intune. Pogledajte pojedinosti o preduvjetima uređaja i o primjeru postavki pravilnika za omogućivanje tihog šifriranja u sljedećem dokumentu: [Tiho Omogući bitlocker šifriranje](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#silently-enable-bitlocker-on-devices). <br><br>

P: Ako je uređaj već šifriran pomoću bitlockera pomoću zadanih postavki operacijskog sustava za način šifriranja i jačinu šifriranja (XTS-AES-128), primijenit će pravilnik s različitim postavkama automatski pokreće ponovno šifriranje pogona novim postavkama?<br>
O: Ne. Da biste primijenili nove postavke šifriranja, pogon najprije morate dešifrirati.<br><br>
**Napomena:** Za uređaje koji se registriraju pomoću autopilota automatsko šifriranje koje bi se odvijalo tijekom OOBE-a ne pokreće se dok se ne procijeni Pravilnik o sustavu Intune, što omogućuje korištenje postavki utemeljenih na pravilniku na mjestu zadanih postavki operacijskog sustava.
 
P: Ako je uređaj šifriran kao rezultat primjene pravilnika intune, hoće li se dešifrirati kada se taj pravilnik ukloni?<br>
O: Uklanjanje pravilnika povezanog s šifriranjem NE rezultira dešifriranje konfiguriranih pogona.
 
P: Zašto Pravilnik o usklađenosti aplikacije Intune pokazuje da na mom uređaju nije omogućen Bitlocker, čak i ako jest?<br>
O: Postavka "Bitlocker enabled" u pravilniku o usklađenosti aplikacije Intune koristi klijent Windows DHA (Device Health Attestation). Taj klijent mjeri samo stanje uređaja u vrijeme pokretanja. Dakle, ako se uređaj nije ponovno pokrenuo od dovršetka bitlocker šifriranja, klijentski servis DHA neće prijaviti Bitlocker kao aktivan.
 
 