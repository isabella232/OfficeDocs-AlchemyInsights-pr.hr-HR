---
title: Privileged Identity Management uloga
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
ms.openlocfilehash: 358e446192e6b58ace81afa06e0d65ae3a207282351ffc3ec9975a24779951fb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53973221"
---
# <a name="privileged-identity-managementpim-role"></a>Privileged Identity Management(PIM) uloga

**Dozvole se ne dodjeljuju nakon aktivacije uloge**

Kada aktivirate ulogu u aplikaciji Azure AD Privileged Identity Management (PIM), aktivacija se možda neće odmah prenijeti na sve portale za koje je potrebna uloga s ovlastima. Ponekad, čak i ako se promjena propagira, web-predmemoriranje na portalu može dovesti do toga da promjena odmah ne utječe na snagu.

Ako je aktivacija odgođena, slijedite ove korake:

1. Odjavite se s portala Azure, a zatim se ponovno prijavite. Kada aktivirate ulogu azure AD ili ulogu resursa servisa Azure, vidjet ćete faze aktivacije. Kada sve faze dovrše, vidjet ćete vezu "Odjava". Tu vezu možete koristiti za odjavu. Time ćete riješiti većinu slučajeva kašnjenja aktivacije.
2. U programu PIM provjerite jeste li navedeni kao član uloge.
3. Ako aktivirate ulogu administratora Exchange, odjavite se i ponovno se prijavite. Ako se problem nastavi pojavljivati, otvorite kartu za podršku i podignite ga kao problem. Ako koristite ulogu administratora Exchange pristup centru za sigurnost i usklađenost, pogledajte sljedeći korak.
4. Ako aktivirate ulogu za pristup centru za sigurnost i usklađenost ili ako aktivirate ulogu administratora sustava SharePoint, doći će do kašnjenja aktivacije od nekoliko minuta do nekoliko sati. To je poznati problem i aktivno radimo s tim timovima na rješavanju tog problema što je prije moguće.

Dodatne informacije potražite u sljedećim člancima:

- [Aktivacija uloga servisa Azure AD u aplikaciji PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?wt.mc_id=portal-microsoft_azure_support")
- [Aktivacija uloga resursa na servisu Azure u aplikaciji PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?wt.mc_id=portal-microsoft_azure_support")

**Dozvole se ne uklanjaju nakon deaktiviranja uloge ili isteka aktivacije uloge**

Kada deaktivirate ulogu u aplikaciji Azure AD Privileged Identity Management ili kada razdoblje aktivacije uloga istekne, može biti kašnjenje u kojem i dalje imate pristup.

Ako je deaktivacija odgođena, slijedite ove korake:

1. Ako deaktivirate ulogu administratora sustava Exchange ili razdoblje aktivacije uloga istekne i primijetite značajno kašnjenje prije nego što se dozvole uklone, otvorite kartu za podršku i obavijestite inženjera za podršku da vam pomogne u prilaženju ulaznice timu za upravljanje pristupom s ovlastima u Office o tom problemu.
2. Ako je razdoblje aktivacije isteklo, ali i dalje imate otvorenu sesiju preglednika, zatvorite preglednik. Ulogu možete nastaviti koristiti dok ne zatvorite tu sesiju. To je poznati problem i tražimo mogući popravak radi aktivnog opoziva svake sesije nakon isteka aktivacije.

Ako se kašnjenje razlikuje od ova dva scenarija, otvorite kartu za podršku.
