---
title: Dodavanje poddomenu
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
- "7"
- "13902"
ms.openlocfilehash: ea39984a54a15ae6167363eb5855943c8ab1120d
ms.sourcegitcommit: a097d1f8915a31ed8460b5b68dccc8d87e563cc0
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/22/2021
ms.locfileid: "59506253"
---
# <a name="adding-a-sub-domain"></a>Dodavanje poddomenu

Poddomenu je moguće dodati na isti ili drugi klijent od nadređene domene. U svakom slučaju morate upravljati vlastitim postavkama DNS-a na web-mjestu registrara. Ako ste Microsoftu dopustili upravljanje DNS postavkama pomoću NS zapisa ili ako ste kupili domenu od Microsofta, ne možete dodavati poddomene bez prethodne promjene.

Najprije dodajte nadređenu domenu, a zatim dodajte poddomenu. Ako se poddomena nalazi na istom klijentu, nije potrebna dodatna provjera. Ako dodate poddomenu zasebnom klijentu, dns txt zapis potreban je za provjeru vlasništva prije dodavanja domene i dodatnih DNS zapisa za odabrane servise.

- Da biste dodali domenu ili poddomenu, slijedite čarobnjak za dodavanje domene [ili](https://admin.microsoft.com/Adminportal#/Domains/Wizard)ručno dodajte domenu ili poddomenu tako da ode na **Postavljanje**  >  **domene**  >  **Dodaj domenu**.

Ako je potrebno:

- Da biste promijenili tko upravlja postavkama DNS-a za postojeću domenu, idite **na Postavke** Domene , potvrdite okvir uz domenu, a zatim  >  [](https://admin.microsoft.com/Adminportal/Home#/Domains)odaberite **Upravljanje DNS-om**. U čarobnjaku odaberite **Dodaj vlastite DNS zapise i** dovršite čarobnjak.
- Da biste dodali poddomenu u Microsoftovu kupljenu domenu, najprije prenesite domenu drugom registraru, a zatim unesite gornju promjenu da biste upravljali vlastitim DNS zapisima. Upute potražite u članku [Prijenos domene s Microsofta na drugo glavno računalo](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/transfer-a-domain-from-microsoft-to-another-host).
- Ako vam se pojavi pogreška da domenu već koriste drugi članovi ili osobe u vašoj tvrtki ili ustanovi, najprije morate preuzeti taj neupravljani račun prije korištenja domene. Upute potražite u članku [Preusmjeravani direktorij kao administrator u programu Azure Active Directory](https://docs.microsoft.com/azure/active-directory/enterprise-users/domains-admin-takeover).
