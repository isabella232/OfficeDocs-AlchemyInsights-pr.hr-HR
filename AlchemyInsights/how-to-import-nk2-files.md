---
title: how-to-import-nk2-files
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1800027"
- "1267"
ms.assetid: ''
ms.openlocfilehash: f2b034926ec165b819119b5c4e060f10022d6017ec5dba8794d18ee3e96c709a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54043198"
---
# <a name="how-to-import-nk2-files"></a>Uvoz .nk2 datoteka 

Kada prvi put pokrenete Microsoft Outlook 2013, Outlook 2016, Outlook 2019 ili Outlook za Microsoft 365, predmemorija nadimaka (pohranjena u datoteci *profilename*.nk2) uvozi se u skrivenu poruku u zadanom spremištu poruka.

Da biste uvezli .nk2 datoteke u Outlook 2013, Outlook 2016, Outlook 2019 ili Outlook za Microsoft 365, provjerite nalazi li se datoteka .nk2 u sljedećoj mapi: %appdata%\Microsoft\Outlook

**Napomena:** datoteka .nk2 mora imati isti naziv kao i trenutni Outlook 2013 ili Outlook 2016 profil. Naziv profila po zadanom je "Outlook". Da biste provjerili naziv profila, slijedite ove korake: 
1. Kliknite **Start**, a zatim **Upravljačka ploča**.
2. Dvokliknite **Pošta**.
3. U dijaloškom okviru Postavljanje pošte odaberite **Prikaži profile**.
4. Odaberite **Pokreni**  >  **pokreni**.
5. U okvir **Otvori** upišite *outlook.exe /importnk2*, a zatim odaberite U **redu**. 

Kada uvezete .nk2 datoteku, sadržaj datoteke spaja se u postojeću predmemoriju nadimaka pohranjenu u poštanskom sandučiću.

**Napomena:** datoteka .nk2 preimenovana je datotečnim nastavkom .old prilikom sljedećeg pokretanja programa Outlook 2013, Outlook 2016, Outlook 2019 ili Outlook za Microsoft 365. Ako želite ponovno uvesti .nk2 datoteku, najprije uklonite datotečni nastavak .old.

Dodatne informacije potražite u članku [Uvoz ili kopiranje popisa za samodovršetost na drugo računalo](https://support.microsoft.com/help/2806550/how-to-import-nk2-files-into-outlook%).