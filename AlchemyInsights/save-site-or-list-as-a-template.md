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
ms.openlocfilehash: 31cb294be6b72be313cf63ed5ed2af0ef041dcf6efb7a7a2af4e1b6a9a149c43
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54109196"
---
# <a name="save-site-or-list-as-a-template"></a>Spremanje web-mjesta ili popisa kao predloška

SharePoint web-mjesta unaprijed su izrađene definicije dizajnirane oko određene poslovne potrebe. Dodatne informacije potražite u članku Stvaranje različitih vrsta web-mjesta pomoću [predložaka SharePoint web-mjesta](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).

Evo nekih uobičajenih problema/rješenja vezana uz spremanje web-mjesta ili popisa kao predloška u web-SharePoint mreži.

**Gumb Spremi predložak web-mjesta/popisa nije dostupan ili nedostaje**. 

- Da bi omogućili značajke predložaka, administratori moraju omogućiti prilagođenu skriptu. Detaljne korake, primjere i napomene potražite u članku [Dopuštanje ili sprječavanje prilagođene skripte](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).


- Naredba Spremi web-mjesto kao predložak nije podržana i može uzrokovati probleme na web-mjestima koja koriste infrastrukturu za objavljivanje u sustavu SharePoint Server.


**Predložak web-mjesta nije moguće stvoriti ili ne funkcionira pravilno**

- Predlošku možda nedostaje značajka [i](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) neće se aktivirati. Ako značajka nije dostupna za aktivaciju u trenutnoj zbirci web-mjesta, ne možete koristiti predložak web-mjesta za stvaranje web-mjesta.


- Provjerite premašuju li neki popisi [](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) ili biblioteke prag ograničenja prikaza popisa od 5000 stavki jer to može blokirati stvaranje predloška web-mjesta.


- Web-mjesto možda koristi previše resursa i stoga predložak web-mjesta premašuje ograničenje od 50 megabajta (MB).


- Postoje problemi s prikazom podataka s popisa koji koristi stupac s vrijednostima. Dodatne informacije potražite u članku Popis generiran predloškom ne prikazuje podatke s točnih [popisa pretraživanja u web-mjestu SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).


Detaljnije informacije o najčešćim problemima i rješenjima potražite u web-mjestu Stvaranje [i korištenje predložaka web-mjesta.](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989)

