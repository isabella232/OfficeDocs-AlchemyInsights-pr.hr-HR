---
title: Zapisnici lozinki
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9361"
- "9003259"
ms.openlocfilehash: ed151b436fa2043c610931deeb74a202af88fcf4
ms.sourcegitcommit: 226fe97678b6be215eda0c278399f8be9be525c1
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/08/2021
ms.locfileid: "50524120"
---
# <a name="password-logs"></a>Zapisnici lozinki

**Imam problema s pristupom zapisnicima nadzora pri ponovnom postavljanju lozinki**

Da biste otklonili poteškoće vezane uz pristup zapisnicima nadzora pri ponovnom postavljanju lozinke, izvedite sljedeći korak:

Provjerite jeste li ovlašteni za prikaz zapisnika nadzora. 

Ovlašteni su samo sljedeće uloge:
 - Globalni administrator
 - Administrator sigurnosti
 - Čitač sigurnosnih tekstova

**Želim vidjeti sve izvorne postavke revizije za ponovno postavljanje lozinke od vremena kada sam se isprva raspoređen**

U izvješćima o posljednjih 30 dana spremaju se i događaji za vraćanje lozinke do 120.000. Ovo se maksimalno ograničenje primjenjuje na UI prilikom preuzimanja CSV-a. 1.000.000 događaji dostupni su pomoću komponente PowerShell.
Dodatne informacije potražite u odjeljku veze u nastavku:

- [Samoposlužni događaji za vraćanje izvorne lozinke iz izvješća Azure AD i eventa](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [Kako brzo preuzeti lozinke za upis na izvornu lozinku pomoću komponente PowerShell](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)

**Želim razumjeti više o mogućnostima izvješćivanja o ponovnom postavljanju lozinki**

Provjerite tko registrira ili ponovno postavljanje lozinki pomoću zapisnika nadzora za vraćanje izvornih postavki servisa Azure AD na portalu Azure u odjeljku **Korisnici i grupe**.
Dodatne informacije potražite u sljedećim vezama:

- [Pregled izvješća o ponovnom postavljanju lozinke](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [Prikaz izvješća o ponovnom postavljanju lozinki na portalu Azure](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [Samoposlužni događaji za vraćanje izvorne lozinke iz izvješća Azure AD i eventa](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [Kako brzo preuzeti lozinke za upis na izvornu lozinku pomoću komponente PowerShell](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)


