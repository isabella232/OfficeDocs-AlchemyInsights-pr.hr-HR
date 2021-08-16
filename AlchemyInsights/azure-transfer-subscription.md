---
title: Prijenos vlasništva nad naplatom servisa Azure
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
- "6849"
ms.openlocfilehash: 803d0105ad2bbaf2b18cea6aa556b6af5e09cb2d41812d4747aa703e6e7d7780
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54036088"
---
# <a name="transfer-azure-billing-ownership"></a>Prijenos vlasništva nad naplatom servisa Azure

Prijavite se na [portal platforme Microsoft Azure](https://portal.azure.com/) kao administrator računa za naplatu koji sadrži pretplatu koju želite prenijeti. Ako niste sigurni jeste li administrator ili ako morate odrediti tko jest, pročitajte odjeljak [Određivanje administratora za naplatu računa](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa).

1. Potražite _Upravljanje troškovima + naplata_.
1. Odaberite **Pretplate** u lijevom oknu. Ovisno o pristupu, možda ćete morati odabrati opseg naplate, a zatim **Pretplate** ili **pretplate na Azure**.
1. Odaberite **Prijenos vlasništva nad naplatom** za pretplatu koju želite prenijeti.
1. Unesite adresu e-pošte korisnika koji je administrator za naplatu računa koji će biti novi vlasnik pretplate, a zatim odaberite **pošalji zahtjev za prijenos**.
1. Korisnik prima poruku e-pošte s uputama da bi pregledao vaš zahtjev za prijenos. Da bi se odobrio zahtjev za prijenos, korisnik odabire vezu u poruci e-pošte i prati upute.

Imajte na umu da ako prenosite vlasništvo nad naplatom pretplate na korisnički račun drugog klijenta servisa Azure AD, svi [zadaci koji se temelje na ulogama kontrole pristupa (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support) za upravljanje resursima u pretplati trajno se uklanjaju. Samo će novi vlasnik imati pristup upravljanju resursima u pretplati. Dodatne informacije o promjeni imenika za pretplatu potražite u članku [Prijenos pretplate na korisnika u drugom klijentu servisa Azure AD](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).

_**Važan utjecaj na vaše fakture**_: ako ste prenijeli vlasništvo nad naplatom pretplate na Azure, vaše će naknade biti u obrocima. Moći ćete pristupati fakturama kako slijedi:  

1. Odaberite pretplatu na stranici [Pretplate](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) na portalu platforme Microsoft Azure kao [korisnik s pristupom fakturama](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support), a zatim odaberite **Računi**.
1. Kliknite **Preuzmi fakturu** da biste prikazali kopiju PDF računa. Ako piše _Nije dostupno_, pročitajte odjeljak [Zašto ne vidim fakturu za zadnje razdoblje naplate?](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice).
1. Svakodnevno korištenje možete pogledati i tako da kliknete **razdoblje naplate** kako biste dobili PDF računa i kopiju detaljnog dnevnog korištenja datoteke (. CSV). Dodatne informacije potražite u članku [Dohvatite podatke o fakturi i korištenju](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support).

**Preporučeni dokumenti**

- [Prijenos vlasništva nad naplatom pretplate na Azure na drugi račun](https://docs.microsoft.com/azure/cost-management-billing/manage/billing-subscription-transfer)
- [O prijenosu vlasničkog računa za pretplatu na Azure](https://docs.microsoft.com//azure/cost-management-billing/understand/subscription-transfer)
- [Prijenos pretplata na alat Visual Studio, Microsoftove mreže partnera (MPN) i plaćanja prema potrošnji](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [Najčešća pitanja o prijenosu vlasništva](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [Otklanjanje poteškoća s prijenosom vlasništva](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)
