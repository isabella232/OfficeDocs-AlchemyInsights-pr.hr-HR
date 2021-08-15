---
title: Nije se moguće prijaviti u aplikaciju Teams zbog pogreške autologon.microsoftazuread-sso.com:443
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "9001686"
- "3750"
ms.openlocfilehash: 6671a63d97f24fadc9b34907d75600a3c0ad1c9990a4a8f8d32034c11e8a952e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54038392"
---
# <a name="unable-to-log-into-teams-due-to-error-autologonmicrosoftazuread-sso-dot-com443"></a>Nije se moguće prijaviti u aplikaciju Teams zbog pogreške autologon.microsoftazuread-sso dot com:443

Ako je kao provjera autentičnosti O365 omogućen besprijekorni SSO, možda će se na intranetska web-mjesta morati dodati URL "autologon.microsoftazuread-sso.com".  Ako je prethodno dodan na pouzdana web-mjesta, a u programu se koristi besprijekorni SSO, mora se ukloniti s pouzdanih web-mjesta.

Pregledajte [kontrolni popis za otklanjanje poteškoća s besprijekornim SSO](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso#troubleshooting-checklist).

Slijedite korake u nastavku da biste dodali URL na popis intranetskih web-mjesta:

1. Otvorite Internet Explorer tako da kliknete gumb **početak**. U okvir za pretraživanje unesite Internet Explorer, a zatim na popisu rezultata kliknite **Internet Explorer**.
2. Kliknite **Alati** pa odaberite **Internetske mogućnosti**.
3. Kliknite karticu **Sigurnost**.
4. Sada kliknite na **lokalna intranetska web-mjesta** a zatim kliknite gumb **web-mjesta**, te **gumb Napredno**.
5. Unesite URL web-mjesta, a zatim kliknite **dodajte**.
6. Kada završite, kliknite **Zatvori**.

Dodatne informacije potražite u članku [Dokumentacija za implementaciju besprijekornih SSO-a za O365](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start) (uključuje proces utemeljen na pravilniku da biste URL dodali na intranetska web-mjesta u koraku 3).
