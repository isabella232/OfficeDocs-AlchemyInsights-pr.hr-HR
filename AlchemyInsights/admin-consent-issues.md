---
title: Problemi s pristankom za administratore
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004354"
- "7786"
ms.openlocfilehash: 6154b4b9cce51be3271cb25132f409319d8da14b
ms.sourcegitcommit: 113b802081101de70810fc73938ea92f7518d8c6
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 01/18/2021
ms.locfileid: "49900822"
---
# <a name="admin-consent-issues"></a>Problemi s pristankom za administratore

1. Omogući [tijek rada pristanka](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-admin-consent-workflow) administratora da biste korisnicima dopustili zahtjev za administratorom izravno na zaslonu pristanak.

1. Ako vam se u postupku pristanka prikazuje neočekivana pogreška, u ovom se članku radi otklanjanja poteškoća: [neočekivano pogreške prilikom izvođenja pristanka na aplikaciju](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).

1. Saznajte više o [pristanku za administratore na Microsoftovoj platformi identiteta](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent), kako funkcionira [upit za suglasnost](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent) i kako [procijeniti zahtjev za pristanak administratora na razini korisnika](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent).

1. Aplikacije koje se integriraju sa platformom Microsoftova identiteta slijede model autorizacije koji korisnicima i administratorima omogućuje kontrolu nad načinom pristupa podacima. Implementacija modela autorizacije ažurirana je na krajnjoj točki platforme Microsoftova identiteta i mijenja način interakcije aplikacije s Microsoftovu platformom Identity. Pogledajte [dozvole i pristanak u krajnjoj točki platforme Microsoftova identiteta](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent) za pregled ovog modela autorizacije, uključujući dosege, dozvole i pristanak.