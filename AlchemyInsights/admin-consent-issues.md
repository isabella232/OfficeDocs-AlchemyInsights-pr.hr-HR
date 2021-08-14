---
title: Problemi s pristankom administratora
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
ms.openlocfilehash: 08d3bfa84fd5ab31d7165090c392866d863898545ade7631e820a100eef89dea
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53952565"
---
# <a name="admin-consent-issues"></a>Problemi s pristankom administratora

1. Omogućite tijek [rada za pristanak administratora](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-admin-consent-workflow) da biste korisnicima omogućili da od administratora zatraži odobrenje izravno s zaslona za pristanak.

1. Ako vi ili korisnici aplikacije tijekom postupka pristanka vidite neočekivane pogreške, upute za otklanjanje poteškoća potražite u ovom članku: Neočekivana pogreška prilikom [izvršavanja pristanka na aplikaciju.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)

1. Saznajte više o [](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent) [pristanku administratora na Microsoftova platforma za identitete,](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent)kako funkcionira upit za pristanak i kako procijeniti zahtjev za pristanak administratora na razini [klijenta](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent).

1. Aplikacije koje se integriraju Microsoftova platforma za identitete slijedite model autorizacije koji korisnicima i administratorima omogućuje kontrolu nad načinom pristupa podacima. Implementacija modela autorizacije ažurirana je na krajnjoj Microsoftova platforma za identitete i mijenja način na koji aplikacija mora stupiti u interakciju s Microsoftova platforma za identitete. Pogledajte [dozvole i pristanak u krajnjoj Microsoftova platforma za identitete za](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent) pregled ovog modela autorizacije, uključujući opsege, dozvole i pristanak.