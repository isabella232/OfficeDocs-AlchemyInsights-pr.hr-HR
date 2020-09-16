---
title: Više korisnika koji ne vide dodatke u programu Outlook
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
ms.openlocfilehash: a0c272f40044795754ed8630e88e00ed14ea6ad7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47729863"
---
# <a name="multiple-users-not-seeing-add-ins-in-outlook"></a>Više korisnika koji ne vide dodatke u programu Outlook

Ako isprobate dodatke programa Outlook, a nijedna se ne prikaže, kao prvi korak otklanjanja poteškoća, pomoću cmdleta **Get-OrganizationConfig** PowerShell zatražite upit za parametar _Appsforofficeenabled_ . Ako upit vraća vrijednost **False**, postavite ovaj parametar na **True** pomoću cmdleta **set-OrganizationConfig** , pa se dodaci prikazuju kao što je očekivano.

Ne preporučujemo da parametar _Appsforofficeenabled_ bude postavljen na **False**. Vrijednost **lažnih** prekoračenja svih navedenih postavki administrativne i korisničke uloge i onemogućuje aktiviranje novih aplikacija od strane bilo kojeg korisnika u tvrtki ili ustanovi.

Dodatne informacije potražite u članku [određivanje administratora i korisnika koji mogu instalirati dodatke za Outlook i upravljati njima](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles).