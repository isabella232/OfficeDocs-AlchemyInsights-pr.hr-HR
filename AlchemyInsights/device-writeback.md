---
title: Uređaj writeback
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
ms.openlocfilehash: f1a8dba19d220e1154549507801c813f56fe5cdd
ms.sourcegitcommit: 0470a728d184ceb89d1419f7ed57166e07bb778b
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 02/15/2021
ms.locfileid: "50256702"
---
# <a name="device-writeback"></a>Uređaj writeback

Writeback uređaja koristi se u sljedećim scenarijima:

- Omogućavanje [servisa Windows Hello za tvrtke pomoću hibridnog certificiranja pouzdanih certifikata](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-cert-trust-prereqs#device-registration)
- Omogućivanje uvjetnog pristupa na temelju uređaja na ADMINISTRATARE (2012 R2 ili novije) zaštićene aplikacije (Trust strana)

    > [!NOTE]
    > Za writeback uređaja potrebna je pretplata na Azure AD Premium.

Time se omogućuje dodatna sigurnost i garancija da se pristup aplikacijama dodjeljuje samo pouzdanim uređajima. Dodatne informacije o uvjetnom pristupu potražite u članku [Upravljanje rizikom uz uvjetni pristup](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) i [Postavljanje lokalnog uvjetnog pristupa pomoću servisa Azure Active Directory registracija uređaja](https://docs.microsoft.com/azure/active-directory/devices/overview).

Dodatne informacije o omogućivanju uređaja writeback za uređaje potražite u članku [Omogućivanje programa writeback uređaja](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-device-writeback).
