---
title: Stvaranje web-mjesta na servisu SharePoint Online
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: eaf09aebad5568aab3a716ce28c8ce3357c9f43175e1b1458bfcd43fd95a71fa
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54057958"
---
# <a name="create-sharepoint-sites-using-templates"></a>Stvaranje SharePoint web-mjesta pomoću predložaka

Mogućnost spremanja web-mjesta u obliku predloška nije podržana za moderna web-mjesta za komunikaciju ili timove. Dodatne informacije o korištenju predložaka potražite u članku [Spremanje, preuzimanje i prenošenje web-mjesta sustava SharePoint u obliku predložaka](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).

Evo nekih uobičajenih problema/rješenja vezanih uz spremanje web-mjesta ili popisa kao predloška u sustavu Sharepoint Online. 

**Gumb Spremi predložak web-mjesta/popisa nije dostupan ili nedostaje**

Da bi omogućili značajke predložaka, administratori moraju omogućiti prilagođenu skriptu. Detaljne korake, primjere i razmatranja potražite u članku 

- [Dopuštanje ili sprječavanje prilagođene skripte](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- Naredba Spremi web-mjesto kao predložak nije podržana i može uzrokovati probleme na web-mjestima koja koriste infrastrukturu za objavljivanje u sustavu SharePoint Server.

**Predložak web-mjesta nije moguće stvoriti ili ne funkcionira pravilno**

Predlošku možda nedostaje značajka [i](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) neće se aktivirati. Ako značajka nije dostupna za aktivaciju u trenutnoj zbirci web-mjesta, ne možete koristiti predložak web-mjesta za stvaranje web-mjesta.

- Provjerite premašuju li neki popisi [](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) ili biblioteke prag ograničenja prikaza popisa od 5000 stavki jer to može blokirati stvaranje predloška web-mjesta.

- Web-mjesto možda koristi previše resursa i stoga predložak web-mjesta premašuje ograničenje od 50 MB.


- Postoje problemi s prikazom podataka s popisa koji koristi stupac s vrijednostima. Dodatne informacije potražite u članku Popis generiran predloškom ne prikazuje podatke s točnih [popisa pretraživanja u web-mjestu SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).

Detaljnije informacije o najčešćim problemima i rješenjima potražite u [web-mjestu Stvaranje i korištenje predložaka web-mjesta.](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989)



