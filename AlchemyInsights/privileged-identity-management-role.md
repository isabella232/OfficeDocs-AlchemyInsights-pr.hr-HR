---
title: Povlaštena uloga upravljanja identitetom
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003230"
- "6825"
ms.openlocfilehash: 726511d016462f56c48a4272b57abc3e9f0cbc3d
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 11/17/2020
ms.locfileid: "49088569"
---
# <a name="privileged-identity-managementpim-role"></a>Povlaštene uloge za upravljanje identitetom (PIM)

**Dozvole se ne dodjeljuju nakon aktiviranja uloge**

Kada aktivirate ulogu u povlaštenom upravljanju identitetom servisa Azure AD (PIM), aktivacija se možda neće odmah proširiti na sve portale koje zahtijevaju privilegiranu ulogu. Ponekad se, čak i ako se promjena proširi, web-predmemoriranje na portalu može rezultirati promjenom netrenutačne efekte.

Ako aktivacija kasni, slijedite ove korake:

1. Odjavite se s portala Azure, a zatim se ponovno prijavite. Kada aktivirate ulogu Azure AD ili ulogu resursa Azure, prikazat će vam se faze aktivacije. Kada završite sa svim fazama, prikazat će se veza za odjavu. Ovu vezu možete koristiti za odjavu. To će riješiti većinu slučajeva za kašnjenje aktivacije.
2. U servisu PIM provjerite jeste li navedeni kao član uloge.
3. Ako aktivirate ulogu administratora sustava Exchange, provjerite jeste li se odjavili i ponovno prijavili. Ako se problem ne riješi, otvorite karticu za podršku i Podignimo ovo kao problem. Ako koristite ulogu administratora sustava Exchange za pristup centru za sigurnost i usklađenost, pročitajte sljedeći korak.
4. Ako aktivirate ulogu za pristup centru za sigurnost i usklađenost ili ako aktivirate ulogu administratora sustava SharePoint, za nekoliko minuta doživjet ćete odgodu aktivacije do nekoliko sati. To je poznat problem i aktivno radimo s tim timovima radi rješavanja tog problema što je prije moguće.

Dodatne informacije potražite u članku:

- [Aktiviranje uloga Azure oglasa u servisu PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?wt.mc_id=portal-microsoft_azure_support")
- [Aktivacija uloga resursa za Azure u servisu PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?wt.mc_id=portal-microsoft_azure_support")

**Dozvole se ne uklanjaju Nakon deaktivacije uloge ili isteka aktivacije uloge**

Kada deaktivirate ulogu u povlaštenom upravljanju identitetu ili kada istekne razdoblje aktivacije uloga, možda će biti odgoda gdje ćete i dalje imati pristup.

Ako vaša deaktivacija kasni, slijedite ove korake:

1. Ako deaktivirate ulogu administratora sustava Exchange ili razdoblje aktivacije uloga, a primjetite značajno kašnjenje prije uklanjanja dozvola, otvorite karticu za podršku i obavijestite inženjera za podršku da vam pomogne podnijeti prijavu karte pomoću tima za upravljanje povlaštenim pristupom (PAM) u sustavu Office u vezi s tim problemom.
2. Ako je razdoblje aktivacije isteklo, ali i dalje imate otvorenu sesiju preglednika, zatvori preglednik. Ulogu možete nastaviti koristiti sve dok ne zatvoriš tu sesiju. To je poznat problem i tražimo potencijalno rješenje za aktivno ukidanje svake sesije kada je aktivacija istekla.

Ako vam se kašnjenje razlikuje od ovih dvaju scenarija, otvorite karticu za podršku.
