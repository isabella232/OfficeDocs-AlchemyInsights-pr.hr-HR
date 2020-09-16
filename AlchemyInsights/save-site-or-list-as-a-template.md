---
title: Spremanje web-mjesta ili popisa kao predloška
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: 37ae727aa6dd6af94d0d833ce972aec413d90194
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727523"
---
# <a name="save-site-or-list-as-a-template"></a>Spremanje web-mjesta ili popisa kao predloška

Predlošci web-mjesta sustava SharePoint pretizgrađene su definicije dizajnirane oko određene poslovne potrebe. Dodatne informacije potražite u članku [Korištenje predložaka za stvaranje različitih vrsta web-mjesta sustava SharePoint](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).

Slijede neki Česti problemi/rješenja vezana uz spremanje web-mjesta ili popisa kao predloška u sustavu SharePoint online.

**Gumb Spremi predložak web-mjesta/popisa nije dostupan ili nedostaje**. 

- Administratorima će biti potrebno omogućiti prilagođenu skriptu za omogućivanje značajki predložaka. Detaljne upute, primjeri i razmatranja potražite u članku [Omogućivanje i onemogućivanje prilagođene skripte](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).


- Naredba Spremi web-mjesto kao predložak nije podržana i može uzrokovati probleme na web-mjestima koja koriste infrastrukturu za objavljivanje sustava SharePoint Server.


**Predložak web-mjesta nije moguće stvoriti ili ne funkcionira pravilno**

- Predložak možda nema [značajku](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) i neće se aktivirati. Ako značajka nije dostupna za aktivaciju u aktualnoj zbirci web-mjesta, ne možete stvoriti web-mjesto pomoću predloška web-mjesta.


- Provjerite prelazi li neki popisi ili biblioteke iznad [praga ograničenja prikaza popisa](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) od 5000 stavki jer to može blokirati stvaranje predloška web-mjesta.


- Web-mjesto možda koristi previše resursa, a predložak web-mjesta premašuje ograničenje od 50 megabajta (MB).


- Postoje problemi s prikazom podataka s popisa koji koristi stupac za pretraživanje. Dodatne informacije potražite u članku [popis generirani predložak ne prikazuje podatke s odgovarajućeg popisa pretraživanja u sustavu SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).


Detaljne informacije o uobičajenim problemima i rješenjima potražite u odjeljku [Stvaranje i korištenje predložaka web-mjesta](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).

