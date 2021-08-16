---
title: Podržane vrste pretplata
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003560"
- "6675"
ms.openlocfilehash: f11eabdc18f708e34a6a10c67bc3e7416330cbf34aec20209b42252ffa0ab018
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54072152"
---
# <a name="supported-subscription-types"></a>Podržane vrste pretplata

Da biste nastavili, pregledajte podržane vrste pretplata.

[Podržane vrste pretplata](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#supported-subscription-types)

**Prijenos vlasništva nad naplatom**

Prijavite se na portal platforme Microsoft Azure kao [administrator](https://ms.portal.azure.com/) računa za naplatu koji sadrži pretplatu koju želite prenijeti

- Potražite **Upravljanje troškovima + naplata**. Odaberite **Pretplate** u lijevom oknu. Ovisno o pristupu, možda ćete morati odabrati opseg naplate, a zatim **Pretplate** ili **pretplate na Azure**.
- Odaberite Prijenos vlasništva nad naplatom za pretplatu koju želite prenijeti.
- Unesite adresu e-pošte korisnika koji je administrator za naplatu računa koji će biti novi vlasnik pretplate, a zatim odaberite **pošalji zahtjev za prijenos**
- Korisnik prima poruku e-pošte s uputama da bi pregledao vaš zahtjev za prijenos. Da bi se odobrio zahtjev za prijenos, korisnik odabire vezu u poruci e-pošte i prati upute.

Napomena: ako prenosite vlasništvo nad naplatom pretplate na korisnički račun drugog klijenta servisa Azure AD, svi [zadaci koji se temelje na ulogama kontrole pristupa (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support) za upravljanje resursima u pretplati trajno se uklanjaju. Samo će novi vlasnik imati pristup upravljanju resursima u pretplati. Dodatne informacije potražite u članku [Prijenos pretplate na korisnika u drugom klijentu servisa Azure AD](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).

**Prijenos vlasništva nad pretplatom**

Posljedica prijenosa vlasništva nad pretplatom jest ta što će pristup na temelju uloga (RBAC) za upravljanje resursima u pretplati izgubiti pristup. Dodatne informacije o dodavanju postojeće pretplate klijentu potražite u članku [Povezivanje ili dodavanje pretplate na Azure u Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory?WT.mc_id=Portal-Microsoft_Azure_Support).

- Prijenos pretplate uz postojeći dugovani iznos iz trenutačnog ciklusa naplate neće biti prenesen na novo sredstvo plaćanja na novom računu. Jedini podaci koji će korisnicima na novom računi biti dostupni jest prošlomjesečna cijena vaše pretplate. Ostatak povijesti upotrebe i naplate ne prenosi se s pretplatom.
- Prijenos vlasništva nad naplatom za pretplate uz Enterprise Agreement (Ugovor Enterprise) (EA) trenutačno su podržane samo na portalu Enterprise Agreement (Ugovor Enterprise)
- Za prijenos pretplate usmjerene na kredit kao što je Visual Studio, BizSpark i Microsoftova partnerska mreža na novog korisnika potrebno je imati licencu za Visual Studio / Microsoftovu partnersku mrežu za prihvaćanje zahtjeva za prijenos
- Svi resursi kao što su virtualni uređaji, diskovi i web-mjesta uspješno se prenose na novi račun. Sljedeći bi resursi mogli biti pogođeni tijekom prijenosa pretplate za sve klijente:

**usluge domene Azure AD**

sefovi za ključeve platforme Azure

- [korisnici i baze podataka povezani sa SQL-om](https://docs.microsoft.com/azure/sql-database/sql-database-aad-authentication-configure?WT.mc_id=Portal-Microsoft_Azure_Support) mogli bi biti pogođeni, posebno ako korisnik provjeru autentičnosti povezanu sa sustavom Azure Active Directory
- **usluge aplikacija** konfigurirane uz provjeru autentičnosti za Azure Active Directory mogle bi biti pogođene
- servisni računi za **tim Visual Studio** povezani s pretplatama na Azure mogli bi privremeno izgubiti pristup kada se otkaže povezana pretplata na Azure.

**Preporučeni dokumenti**

Koraci nakon prihvaćanja vlasništva nad naplatom:

- Da biste zadržali vlasništvo nad naplatom, no promijenili vrstu pretplate, pročitajte članak: [Promjena pretplate na Azure na drugu ponudu](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Prijenos pretplata na alat Visual Studio, Microsoftove mreže partnera (MPN) i plaćanja prema potrošnji](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [Prijenos vlasništva nad naplatom za pretplate uz Enterprise Agreement (Ugovor Enterprise)](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transfer-billing-ownership-of-enterprise-agreement-ea-subscriptions)
- [Najčešća pitanja o prijenosu vlasništva](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [Otklanjanje poteškoća s prijenosom vlasništva](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)