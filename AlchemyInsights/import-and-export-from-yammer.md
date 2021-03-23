---
title: Uvoz i izvoz iz servisa Yammer
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
- "9735"
- "9003224"
ms.openlocfilehash: dcdf569f96e51a62899761589ef6f9f317517c3a
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035092"
---
# <a name="import-and-export-from-yammer"></a>Uvoz i izvoz iz servisa Yammer

**Uvoz**

Mogućnosti uvoza korisnika razlikuju se ovisno o tome je li mreža servisa Yammer u [izvornom načinu rada za Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/overview-native-mode)ili ne.

- **Način koji nije urođenik**: korisnici se mogu uvesti u grupe pomoću značajke [Dodaj iz adresara](https://support.microsoft.com/office/manage-yammer-community-members-75253554-d0f3-4148-b835-e6a9a8a0c294) (ograničenje na 100 korisnika) unutar postavki grupe ili na mrežu pomoću [skupnog ažuriranja](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users) unutar administratora mreže.
- **Izvorni način rada**: članstvo u grupama i mreža za članstvo moraju se izvoditi na servisu [Microsoft 365 admin portal](https://docs.microsoft.com/microsoft-365/admin/add-users), [Azure ad portal](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)ili pomoću druge mogućnosti Azure AD. Mreže u izvornom načinu više ne sadrže pristup masovnim ažuriranjem i drugim naslijeđenim značajkama.

> [!IMPORTANT]
> Yammer nikada nije podržao Uvoz sadržaja iz mrežnog administratora čak ni kada je značajka izvoza podataka korištena u drugoj mreži. Sadržaj se može ponovno knjižiti putem partnerskih rješenja ili API-ja za odmor u servisu Yammer.

**Izvoz**

[Izvoz mrežnih podataka unutar mrežnog administratora](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data) dopušta izvoz sadržaja iz mreža servisa Yammer, uključujući poruke i datoteke. Privici mogu biti izuzetno veliki i prouzroci da će izvoz poduzeti značajno vrijeme za dovršetak. Preporučujemo da se aktivne mreže izvoze pomoću API-ja za [Izvoz podataka](https://developer.yammer.com/docs/data-export-api) u komadima za dan ili tjedan. Microsoftova podrška ne nudi prilagođene skripte za tu svrhu.

Za izvoz sadržaja za pojedinačnog korisnika postoji zasebni [Izvoz u Gdpr](https://docs.microsoft.com/yammer/manage-security-and-compliance/gdpr-requests-in-yammer-enterprise) -u.