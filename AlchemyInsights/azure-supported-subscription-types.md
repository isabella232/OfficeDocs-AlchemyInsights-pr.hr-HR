---
title: Podržane vrste pretplate
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
- "9003560"
- "6675"
ms.openlocfilehash: 46bc60435c3f8477e9f274d90c39d0f1c6a523c6
ms.sourcegitcommit: f8b41ecda6db0b8f64fe0c51f1e8e6619f504d61
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 10/28/2020
ms.locfileid: "48807247"
---
# <a name="supported-subscription-types"></a>Podržane vrste pretplate

Pregledajte podržane vrste pretplata da biste nastavili dalje.

[Podržane vrste pretplate](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#supported-subscription-types)

**Prijenos vlasništva nad naplaćivanje**

Azure portal kao [administrator računa](https://ms.portal.azure.com/) za račun za naplatu s pretplatom koju želite prenijeti

- Pretraživanje za **Upravljanje troškovima + naplata** . Odaberite **pretplate** iz lijevog okna. Ovisno o pristupu, možda ćete morati odabrati opseg naplate, **a zatim pretplate** ili **Azure pretplate** .
- Odaberite prijenos vlasništva za naplatu za pretplatu koju želite prenijeti
- Unesite adresu e-pošte korisnika koji je administrator naplate računa koji će biti novi vlasnik pretplate, a zatim odaberite **Pošalji zahtjev za prijenos**
- Korisnik će dobiti poruku e-pošte s uputama za pregled vašeg zahtjeva za prijenos. Da biste odobrili zahtjev za prijenos, korisnik će odabrati vezu u poruci e-pošte i slijediti upute.

Pažnja: Ako prenesete vlasništvo nad pretplatom na korisnički račun u drugom servisu Azure AD, svi zadaci koji se [temelje na ulogama (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support) za upravljanje resursima u pretplati trajno se uklanjaju. Samo novi vlasnik imat će pristup resursima u pretplati. Dodatne informacije potražite u članku [prijenos pretplate na korisnika u nekom drugom klijentu za Azure ad](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).

**Prijenos vlasništva nad pretplatom**

Preduvjet za prijenos vlasništva na pretplatničkim ulogama (RBAC) za upravljanje resursima u pretplati gube pristup. Dodatne informacije o dodavanju postojeće pretplate na korisnika potražite u članku [pridruživanje i dodavanje pretplate Azure u servisu Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory?WT.mc_id=Portal-Microsoft_Azure_Support).

- Prijenos pretplate uz postojeći neplaćeni iznos iz tekućeg ciklusa naplate neće se prenijeti na novi instrument plaćanja u novom računu. Jedine informacije dostupne korisnicima u novom računu jesu troškovi posljednjeg mjeseca za vašu pretplatu. Ostatak povijesti upotrebe i naplate ne prenosi se pretplatom.
- Prijenos vlasništva nad pretplatom na Enterprise Agreement (EA) trenutno je podržan samo na portalu za Enterprise sporazum
- Prijenos pretplate orijentiranog na kredit kao što je Visual Studio, BizSpark, Microsoftova mrežna mreža za novog korisnika mora imati licencu za Visual Studio/Microsoftovu partnersku mrežu da bi prihvatio zahtjev za prijenos
- Svi resursi kao što su virtualni strojevi, diskovi i web-mjesta uspješno se prebacuju na novi račun. Sljedeći resursi mogu utjecati na prijenos pretplate na više korisnika:

**Usluge servisa Azure AD Domain**

Sefovi za Azure

- Moguće je utjecati na [korisnike i baze podataka vezanih uz SQL](https://docs.microsoft.com/azure/sql-database/sql-database-aad-authentication-configure?WT.mc_id=Portal-Microsoft_Azure_Support) , osobito ako klijent koristi provjeru autentičnosti povezanu s Azure Active Directory.
- **Aplikacijski servisi** konfigurirani uz provjeru autentičnosti servisa Azure Active Directory mogu se utjecati
- **Vizualni studijski tim** Računi servisa povezani s pretplatama na Azure mogu privremeno izgubiti Access kada se otkaže pretplata na Azure

**Preporučeni dokumenti**

Koraci nakon prihvaćanja vlasništva nad naplaćom:

- Da biste zadržali vlasništvo nad naplaćivanju, ali promijenite vrstu pretplate, pogledajte: [prebacivanje pretplate na Azure na drugu ponudu](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Prijenos Visual Studio, Microsoft partner Network (MPN) i pay kao što ste ići dev/test pretplate](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [Prijenos vlasništva nad pretplatama na Enterprise Agreement (EA)](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transfer-billing-ownership-of-enterprise-agreement-ea-subscriptions)
- [Najčešća pitanja o prijenosu vlasništva](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [Otklanjanje poteškoća s vlasničkim prijenosom](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)