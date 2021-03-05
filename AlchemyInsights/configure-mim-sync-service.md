---
title: Konfiguracija servisa MIM sync
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8472"
- "9004688"
ms.openlocfilehash: 48e9a0e8c26088b690092bfaedfba641841739f6
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50480964"
---
# <a name="configure-mim-sync-service"></a>Konfiguracija servisa MIM sync

Servis za sinkronizaciju programa Microsoft Identity Manager (MIM) komponenta je MIM. To je središnji lokalni servis koji pohranjuje i integrira informacije za tvrtke ili ustanove koje imaju više lokalnih direktorija i baza podataka. Problem možete riješiti i uz MIM sync ako je problem upućen nedavnim ažuriranjem na MIM ili je jedan od ostalih problema navedenih u odjeljku u nastavku.

**Preporučeni koraci**

1. Provjerite koristite li nedavno ažuriran broj MIM sinkronizacijom i provjerite je li na [bilješkama o objavama izdanja Mim sinkronizirajte](https://docs.microsoft.com/microsoft-identity-manager/reference/version-history) problem riješen u ažuriranju.
2. Ako je problem s generičkim LDAP, Generic SQL, Lotus Domino ili Web Services Connector, provjerite koristite li nedavno ažuriranje [generičkih konektora](https://docs.microsoft.com/microsoft-identity-manager/reference/microsoft-identity-manager-2016-connector-version-history).
3. Ako se MIM sinkronizira s pogreškom, obratite se u tablici [kodova pogrešaka](https://docs.microsoft.com/microsoft-identity-manager/reference/maerrorcodes) radi utvrđivanja mogućih uzroka.
4. Ako se pokretanje prestane stvarati uz **iznimku Extension-DLL**, kliknite te riječi da biste otvorili prozor **Svojstva prostora konektora** , a zatim kliknite na gumb **Trace...** da biste vidjeli dodatne informacije o temeljnim uzroku, kao što je opisano u odjeljku [protezanje-DLL – iznimka](https://social.technet.microsoft.com/wiki/contents/articles/7515.fim-troubleshooting-extension-dll-exception.aspx).
5. Ako je u zapisniku događaja prilikom sinkronizacije lozinke servisa za obavješćivanje o promjeni lozinke (PCN-a) **došlo do pogreške 6025** , provjerite vodič za otklanjanje poteškoća s [prijavom na poruku o pogrešci 6025](https://social.technet.microsoft.com/wiki/contents/articles/4159.pcns-troubleshooting-event-id-6025.aspx).
6. Ako je potpuna sinkronizacija s agentom za upravljanje servisom FIM spor, provjerite postavku **automatskog rasta** za tempdb, kao što je opisano u odjeljku [Otklanjanje poteškoća s usporenim ili visećim punim sinkronizacijom](https://social.technet.microsoft.com/wiki/contents/articles/14713.troubleshooting-fim-performance-slow-or-hanging-full-synchronization.aspx).
7. Ako naijete na pogrešku zaustavnog poslužitelja s neuspjelih-stvaranje-Via-web-servisima pomoću agenta za upravljanje servisom FIM, pročitajte članak [Podrška-informacije: nije uspjelo-stvaranje-Via-Web-Services](https://docs.microsoft.com/archive/blogs/iamsupport/support-info-fimma-failed-creation-via-web-services) za pregled uzroka.

