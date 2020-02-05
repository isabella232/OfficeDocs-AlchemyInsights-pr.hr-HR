---
title: Stvaranje web-mjesta u sustavu SharePoint Online
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: b9009fdbdc2a5e7443151446daade1685d2f5d45
ms.sourcegitcommit: 317eeed39c7777a922442992d67733726c41d9e1
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 02/04/2020
ms.locfileid: "41770415"
---
# <a name="create-sharepoint-sites-using-templates"></a>Stvaranje SharePoint web-mjesta pomoću predložaka

Mogućnost spremanja web-mjesta kao predloška nije podržana s modernom komunikacijom ili tim web-lokacijama. Dodatne informacije o korištenju predložaka potražite u okviru [Spremi, Preuzmite i prenesite SharePoint web-mjesto kao predložak](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).

Evo nekih uobičajenih problema/rješenja vezanih uz spremanje web-mjesta ili popisa kao predloška u sustavu SharePoint online. 

**Spremanje gumba predloška web-mjesta/popisa nije dostupno ili nedostaje**

Administratori će morati dopustiti prilagođenoj skripti da omogući značajke predloška. Za detaljne korake, primjeri i razmatranja vide 

- [Dopusti ili spriječi prilagođenu skriptu](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- Naredba Spremi web-mjesto kao predložak nije podržana i može uzrokovati probleme na web-lokacijama koje koriste SharePoint Server Publishing je infrastruktura.

**Predložak web-mjesta nije moguće stvoriti ili ne radi ispravno**

Predlošku možda nedostaje [značajka](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) i neće se aktivirati. Ako značajka nije dostupna za aktivaciju u trenutnoj zbirci web-mjesta, ne možete koristiti predložak web-mjesta za stvaranje web-mjesta.

- Provjerite prelazi li neki popisi ili biblioteke prekoračiti [prag ograničenja prikaza popisa](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) od 5000 artikala jer to može blokirati stvaranje predloška web-mjesta.

- Web-mjesto možda koristi previše resursa i stoga predložak web-mjesta premašuje ograničenje od 50 MB.


- Postoje problemi s prikazom podataka s popisa koji koristi stupac za pretraživanje. Dodatne informacije potražite [u prikazu popisa koji se generiraju predlošcima ne prikazuju se podaci s ispravnog popisa pretraživanja u sustavu SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).

Za detaljnije informacije o zajedničkim problemima i rješenjima, provjerite [stvorite i koristite predloške web-mjesta](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).



