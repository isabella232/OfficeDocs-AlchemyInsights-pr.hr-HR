---
title: Otklanjanje poteškoća s hibridnim pridruživanjem servisa Azure AD
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/06/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6162"
- "6158"
- "9003244"
- "9003246"
ms.openlocfilehash: 23da360965a5972e328844d505698c91ece61788240d8fdb8909fff3a7ef0d7f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53939263"
---
# <a name="troubleshoot-hybrid-azure-ad-join"></a>Otklanjanje poteškoća s hibridnim pridruživanjem servisa Azure AD

Preporučuje se da uređaj može pristupati krajnjim točkama registracije uređaja u odjeljku računa sustava pomoću skripte [Test Device Registration Connectivity](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/).

1. Ako prvi put postavljate registracije uređaja, obavezno pregledajte[ntroduction](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) na upravljanje uređajima u aplikaciji Azure Active Directory da biste saznali kako nabaviti uređaje pod kontrolom platforme Azure AD.
1. Ako izravno registrirate uređaje na Azure AD i upisujete ih u Intune, provjerite jeste li [konfigurirali Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) i imate [li](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) prvo licencu.
1. Provjerite jeste li ovlašteni za izvođenje operacija na servisu Azure AD i lokalnom servisu AD. Samo globalni administrator na servisu Azure AD može upravljati postavkama za registracije uređaja. Osim toga, ako postavljate automatske registracije u lokalnom servisu Active Directory, morat ćete biti administrator servisa Active Directory i AD FS (ako je primjenjivo).

Dodatne informacije o rješavanju potencijalnih [](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current) problema s hibridnim pridruživanjem potražite u članku Otklanjanje poteškoća s hibridnim pridruživanjem za postavljanje hibridnih uređaja pridruženih servisu Azure AD i upravljanje uređajima pomoću portala Azure Ad, pogledajte postavljanje hibridnih uređaja pridruženih servisu [Azure AD (lokalno](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan?WT.mc_id=Portal-Microsoft_Azure_Support) pridruženim domenama) i Upravljanje uređajima pomoću [portala Azure](https://docs.microsoft.com/azure/active-directory/devices/device-management-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).

Da biste riješili uobičajene probleme s pridruživanjem hibridnih Azure Active Directory (AD), pogledajte najčešća pitanja o [hibridnom pridruživanju servisa Azure AD](https://docs.microsoft.com/azure/active-directory/devices/faq#hybrid-azure-ad-join-faq).
