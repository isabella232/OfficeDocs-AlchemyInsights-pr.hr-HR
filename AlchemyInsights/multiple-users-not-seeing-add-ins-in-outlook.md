---
title: Više korisnika ne vidi dodatke u Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.openlocfilehash: 850df2cb349f9a751def3d59fb665670e70e493daba56a88821afcef9c48ffa8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54011796"
---
# <a name="multiple-users-not-seeing-add-ins-in-outlook"></a>Više korisnika ne vidi dodatke u Outlook

Ako testirate Outlook i nijedan se ne prikazuje kao prvi korak za otklanjanje poteškoća, upotrijebite cmdlet **Get-OrganizationConfig** PowerShell da biste upitali _parametar AppsForOfficeEnabled._ Ako upit vraća vrijednost False **,** postavite taj parametar na **True** pomoću cmdleta **Set-OrganizationConfig,** pa će se dodaci prikazivati prema očekivanom.

Ne preporučujemo da je parametar _AppsForOfficeEnabled_ postavljen na **False**. Vrijednost False **nadjačava** sve gore navedene postavke uloge Administrator i Korisnik i onemogučava aktivaciju novih aplikacija od strane bilo kojeg korisnika u tvrtki ili ustanovi.

Dodatne informacije potražite u članku [Određivanje administratora i korisnika koji](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles)mogu instalirati dodatke i upravljati njima za Outlook .