---
title: Spremi web-mjesto ili popis kao predložak
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: 627f49991aaef984f731412045351d7a1862b376
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 12/15/2019
ms.locfileid: "40048716"
---
# <a name="save-site-or-list-as-a-template"></a>Spremi web-mjesto ili popis kao predložak

Predlošci web-mjesta sustava SharePoint prethodno su ugrađene definicije koje su dizajnirane oko određene poslovne potrebe. Za dodatne informacije pogledajte [pomoću predložaka za stvaranje različitih vrsta SharePoint web-mjesta](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).

Evo nekih uobičajenih problema/rješenja vezanih uz spremanje web-mjesta ili popisa kao predloška u sustavu SharePoint online.

**Spremanje gumba predloška web-mjesta/popisa nije dostupno ili nedostaje**. 

- Administratori će morati dopustiti prilagođenoj skripti da omogući značajke predloška. Za detaljne korake primjeri i razmatranja vide [dopuštanje ili sprječavanje prilagođene skripte](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).


- Naredba Spremi web-mjesto kao predložak nije podržana i može uzrokovati probleme na web-lokacijama koje koriste SharePoint Server Publishing je infrastruktura.


**Predložak web-mjesta nije moguće stvoriti ili ne radi ispravno**

- Predlošku možda nedostaje [značajka](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) i neće se aktivirati. Ako značajka nije dostupna za aktivaciju u trenutnoj zbirci web-mjesta, ne možete koristiti predložak web-mjesta za stvaranje web-mjesta.


- Provjerite prelazi li neki popisi ili biblioteke prekoračiti [prag ograničenja prikaza popisa](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) od 5000 artikala jer to može blokirati stvaranje predloška web-mjesta.


- Web-mjesto možda koristi previše resursa i stoga predložak web-mjesta premašuje ograničenje od 50 megabajta (MB).


- Postoje problemi s prikazom podataka s popisa koji koristi stupac za pretraživanje. Dodatne informacije potražite [u prikazu popisa koji se generiraju predlošcima ne prikazuju se podaci s ispravnog popisa pretraživanja u sustavu SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).


Za detaljnije informacije o zajedničkim problemima i rješenjima molimo upućivanje, [Stvaranje i korištenje predložaka web-mjesta](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).

