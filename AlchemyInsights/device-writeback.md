---
title: Pisanje na uređaju
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
- "9003257"
- "8279"
ms.openlocfilehash: 78af4dc8cfe38586dcec8d01b72170b56d98fa27860489bf2ca9544f32210c37
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54101942"
---
# <a name="device-writeback"></a>Pisanje na uređaju

Pisanje na uređaju koristi se u sljedećim scenarijima:

- Omogućivanje [Windows Hello za tvrtke pomoću hibridne implementacije pouzdanosti certifikata](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-cert-trust-prereqs#device-registration)
- Omogućivanje uvjetnog pristupa na temelju uređaja u ADFS (2012 R2 ili novije) zaštićene aplikacije (pouzdane strane)

    > [!NOTE]
    > Pretplata na Azure AD premium potrebna je za vraćanje na pisanje uređaja.

Time se pruža dodatna sigurnost i jamstvo da se pristup aplikacijama dodjeljuje samo pouzdanim uređajima. Dodatne informacije o uvjetnom pristupu potražite u članku [Upravljanje rizikom](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) uz uvjetni pristup i Postavljanje lokalnog [uvjetnog pristupa pomoću Azure Active Directory registracije uređaja](https://docs.microsoft.com/azure/active-directory/devices/overview).

Dodatne informacije o omogućivanju povratne informacije o uređaju za uređaje potražite u članku [Omogućivanje pisanja uređaja](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-device-writeback).
