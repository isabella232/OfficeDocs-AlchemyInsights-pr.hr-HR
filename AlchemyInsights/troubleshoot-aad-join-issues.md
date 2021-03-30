---
title: Otklanjanje poteškoća s pridruživanjem servisa Azure AD
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003246"
- "6157"
ms.openlocfilehash: 0e9f7c95cf522340e9976f668c1d1a9eaff71910
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/29/2021
ms.locfileid: "51404381"
---
# <a name="troubleshoot-azure-ad-join-issues"></a>Otklanjanje poteškoća s pridruživanjem servisa Azure AD

1. Ako prvi put postavljate registracije uređaja, provjerite jeste li pregledali uvod u upravljanje uređajima na servisu [Azure Active Directory](https://docs.microsoft.com/azure/active-directory/devices/overview) koji će vas voditi o tome kako nabaviti uređaje pod kontrolu za Azure AD. 
1. Ako izravno registrirate uređaje na Azure AD i registrirate ih u Intune, morat [](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign) ćete biti sigurni da ste [konfigurirali Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment) i da ste prvo registrirali licencu.
1. Provjerite imate li ovlasti za izvođenje operacija na servisu Azure AD. Samo globalni administrator na servisu Azure AD može upravljati postavkama za registracije uređaja.
1. Da biste u implementaciju pridruživanja servisa Azure AD udružili, [pogledajte planiranje pridruživanja servisu Azure AD](https://docs.microsoft.com/azure/active-directory/devices/azureadjoin-plan).

Dodatne informacije o rješavanju uobičajenih problema s pridruživanjem servisa Azure AD potražite u članku [Najčešća](https://docs.microsoft.com/azure/active-directory/devices/faq#azure-ad-join-faq) pitanja o pridruživanju servisu Azure Ad i uređaju sa sustavom Windows 10 pro potražite u članku Nemogućnost pridruživanja računalu sa sustavom Windows 10 Pro na Azure AD – potrebno je nadograditi [na Microsoftovu zajednicu](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900)
