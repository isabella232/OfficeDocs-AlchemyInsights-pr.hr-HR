---
title: Otklanjanje poteškoća s korisničkim pitanjima
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7813"
- "9004358"
ms.openlocfilehash: d9964e50bdea0c41ac14ab3783b579034b5f2c8c
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 01/18/2021
ms.locfileid: "49900804"
---
# <a name="announcements"></a>Najave

Slijedite Googleove smjernice o kompatibilnosti testiranja da biste testirali utječu li na vaše aplikacije. Googleove smjernice dostupne su u programu https://docs.microsoft.com/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support .

Provjerite koristite li web-prikaz sustava ili sistemski preglednik prilikom prijave korisnika pomoću računa potrošača za Google. Dodatne informacije potražite u članku [Problemi s prijavom u aplikacije pomoću preglednika Chrome](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications).


**Ne mogu stvoriti novog korisnika u direktoriju Azure AD**

Da biste otklonili poteškoće s pitanjem da ne možete stvoriti novog korisnika u servisu Azure AD, slijedite sljedeće korake:

1. Provjerite jeste li ovlašteni za stvaranje novog standardnog korisnika. U servisu Azure Active Directory (AD) možete stvoriti novog standardnog korisnika samo za globalne administratore ili ulogu administratora korisnika. Ako niste u jednoj od tih uloga, zatražite od administratora da vas doda u neku od ovih uloga ili da stvori novi korisnički račun za vas.
2. Provjerite je li korisničko ime u domeni koja je potvrđena u servisu Azure AD. Ako nemate potvrđene prilagođene nazive domena u Azure AD-u, možete koristiti početnu domenu Azure AD, koja završava s *. onmicrosoft.com.
3. Provjerite je li korisničko ime u domeni koja se ne šalje na Azure AD iz lokalnog oglasa. Korisnici se ne mogu dodati u oblak s nazivima domena koji su na lokalnoj stranici.
4. Pobrinite se da nijedan drugi korisnik ili kontakt već ima korisničko ime koje želite dodijeliti novom korisniku. Korisnička imena moraju biti jedinstvena na servisu Azure AD.
5. Pogledajte [Azure ad uloge i administratore](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) za Azure AD.
6. Pogledajte [nazive domena](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Domains) za Azure AD.
7. Pregledajte [zapisnike nadzora](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Audit) da biste vidjeli detaljnije informacije o nedavno stvorenom ili izbrisanom korisniku kao što je taj koji je izvršio akciju i kada.
8. Dodatne informacije o dodavanju novih korisnika potražite u članku [Korištenje portala Azure za stvaranje novog korisnika u Azure ad-u](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory) .
9. Dodatne informacije o dozvolama administratorske uloge u servisu Azure AD potražite u članku [administrativne uloge za Azure](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference).
10. Pojedinosti o stvaranju korisnika pomoću servisa Azure AD PowerShell potražite u članku [Azure ad PowerShell za stvaranje novog korisnika](https://docs.microsoft.com/powershell/module/azuread/new-azureaduser).

**Problem s prijavom samoservisa**

Da biste otklonili poteškoće u vezi s prijavom samoservisiranja, učinite sljedeće:

1. Da biste koristili samoservisnu prijavu sa svojim aplikacijama, najprije omogućite prijavu samoservisa za svog stanara. 
2. Da biste aplikaciji omogućili podršku za samoposluživanje, dodajte ga u tijek korisnika. Kada sljedeći put odete na stranicu za prijavu za tu aplikaciju, prikazat će vam se mogućnost **_nema računa? Stvorite jedan!_* _. Time se započinje postupak prijave samoservisiranja.
3. Informacije o načinu korištenja samoposlužnog prijave radi popunjavanja tvrtke ili ustanove u servisu Azure AD potražite u članku [samoposluživanje prijavite se za Azure ad](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-self-service-signup).
4. Kada povežete korisnički tijek s jednom ili više aplikacija, korisnici koji posjećuju tu aplikaciju moći će se registrirati i dobiti račun za gosta pomoću mogućnosti konfiguriranih u protoku korisnika. Dodatne informacije o prijavi i dobivanju računa za gosta korisnici mogu vidjeti [samoposlužne prijave za goste korisnika](https://docs.microsoft.com/azure/active-directory/external-identities/self-service-sign-up-user-flow).

_ *Problem poziva vanjskog korisnika**

Da biste otklonili poteškoće koje se odnose na pozivanje vanjskog korisnika, izvedite sljedeći korak:

Provjerite šaljete li pozivnicu korisnika na adresu e-pošte koja odgovara nazivu s kojim se korisnik prijavljuje. Ako pozivnicu šaljete na korisnikovu proxy adresu e-pošte, korisnik je ne može otkupiti. Dodatne informacije potražite u članku [dokumentacija za Azure ad B2B](https://docs.microsoft.com/azure/active-directory/external-identities/).

**Ne mogu dodijeliti licence korisniku**

Da biste otklonili poteškoće u vezi s dodjeljivanjem licenci korisniku, učinite sljedeće:

1. Da biste upravljali korisničkim dozvolama, provjerite koristite li račun s jednom od potrebnih administratorskih uloga: globalni administrator, administrator licence ili administrator korisnika. Korisničku ulogu možete provjeriti na kartici **uloga direktorija** na korisničkom oštricu.
2. Ako koristite portal Azure, a dodjela licenci ne uspijeva, kliknite obavijest u gornjem desnom kutu. Time se otvara oštrica s detaljima o tome što je pošlo po zlu. U većini slučajeva to je dovoljno da biste razumjeli i riješili problem.
3. Prije nego što se licenci može dodijeliti korisniku, provjerite je li svojstvo **lokacije korištenja** postavljeno za korisnika. Provjerite je li korisnik taj objekt postavio prikazivanjem kartice **Profil** na popisu korisnika.
4. Provjerite ima li dovoljno dostupnih licenci za proizvod koji pokušavate dodijeliti. Na portalu Azure Active Directory možete vidjeti broj dostupnih licenci, a na servisu [Azure aktivni direktorij-> licence-> svi proizvodi](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/LicensesMenuBlade/Products).
5. Korisnik možda već ima neku drugu licencu čije se usluge sukobljavaju s onima u novoj licenci koju pokušavate dodijeliti. Ako korisnik, primjerice, ima omogućen servis Exchange Online (tarifa 1), nećete moći dodijeliti licencu za Exchange Online (plan 2). Onemogućite jedan od servisa da biste dopustili novi zadatak licence. Ako koristite portal za Azure ili komponente PowerShell, na stranici Detalji o **problemu** navedene su određene usluge koje uzrokuju sukob.
6. Ako pokušavate ukloniti licencu, a to ne uspijeva, korisnik može imati druge licence s servisima koje ovise o servisima koje pokušavate ukloniti. Ako koristite portal za Azure ili komponente PowerShell, poruka o pogrešci prikazat će popis određenih servisa koji imaju ovisnosti.
7. Ako želite razumjeti zašto je licenca dodana/uklonjena iz korisnika (primjerice, tko je još u vašoj tvrtki ili ustanovi mogao promijeniti), Provjerite zapisnike nadzora. Postavite filtar na **Licencne aktivnosti** da bi vam se prikazivale sve promjene, uključujući "glumca" koji ih je izveo.
8. Ako koristite Exchange Online, neki korisnici u vašem zakupcu možda su neispravno konfigurirani s istom vrijednošću Proxy adrese. U takvim slučajevima možda ćete vidjeti generičke poruke o pogreškama kada operacija licence ne uspije. U [ovom se članku](https://docs.microsoft.com/exchange/troubleshoot/administration/proxy-address-being-used) nalaze dodatne informacije o tom problemu, uključujući informacije o [povezivanju sa sustavom Exchange Online pomoću udaljene komponente PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell). Da biste odredili koji korisnici u vašem zakupcu sadrže istu proxy adresu, izvršite ovaj cmdlet sustava Exchange Online:

Pokretanje

Get-Recipient | Gdje je {$ _. Adrese e-pošte-Match <user principal name> } | fL name, RecipientType, adresa e-pošte





