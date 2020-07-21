---
title: Više korisnika koji ne vide dodatke u programu Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.openlocfilehash: 18d3fa535a88af18d8c4b02a5371d0a81c8d28c0
ms.sourcegitcommit: a05276bd623466ad211e1f8d9f0c616672dd3640
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 07/16/2020
ms.locfileid: "45197771"
---
# <a name="multiple-users-not-seeing-add-ins-in-outlook"></a>Više korisnika koji ne vide dodatke u programu Outlook

Ako testirate dodatke programa Outlook i ništa se ne prikazuje, kao prvi korak za otklanjanje poteškoća, upotrijebite cmdlet **Get-OrganizationConfig** PowerShell da biste upitali parametar _AppsForOfficeEnabled._ Ako upit vraća vrijednost **False**, postavite ovaj parametar na **True** pomoću cmdleta **Set-OrganizationConfig,** tako da se dodaci pojavljuju prema očekivanjima.

Ne preporučujemo da parametar _AppsForOfficeEnabled_ postavljen na **False**. Vrijednost **False** nadjačava sve gore navedene postavke uloge administrativne i korisničke uloge i sprječava bilo koje nove aplikacije da budu aktivirane od strane bilo kojeg korisnika u tvrtki ili ustanovi.

Dodatne informacije [potražite u odjeljku Određivanje administratora i korisnika koji mogu instalirati dodatke za Outlook i upravljati njima](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles).