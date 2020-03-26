---
title: Nije se moguće prijaviti u aplikaciju Teams zbog pogreške autologon.microsoftazuread-sso.com:443
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "9001686"
- "3750"
ms.openlocfilehash: 77049153939989d1c63789adfec0b494d047a6e4
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931831"
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
