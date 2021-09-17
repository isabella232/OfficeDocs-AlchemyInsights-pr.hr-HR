---
title: Korisnička slika i dalje se prikazuje na Microsoft Teams organizacijskom grafikonu
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/13/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13834"
- "9007457"
ms.openlocfilehash: be4c6feb55e6b7c4667566946d8d3640cc0ffb1d
ms.sourcegitcommit: b47c6d5e74819b73becaf1dc5eacc72eaf7c1055
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/15/2021
ms.locfileid: "59422194"
---
# <a name="user-picture-still-appears-in-the-microsoft-teams-organization-chart"></a>Korisnička slika i dalje se prikazuje na Microsoft Teams organizacijskom grafikonu

Ako je jedna ili više pojedinaca u vašoj tvrtki ili ustanovi onemogućeno ili uklonjeno, a njihova se fotografija profila i dalje prikazuje na organizacijskom grafikonu, **postavka ShowInAddressLists postavljena** je na False: 

1. Idite na Centar za administratore okruženja Microsoft 365 > [aktivni korisnici](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users) i odaberite korisnika s fotografijom koja se i dalje prikazuje. 
1. Odaberite **karticu Pošta** i provjerite je li popis Pokaži na **globalnoj adresi** postavljen na **Ne**.

Ako **postavka ShowInAddressLists** na **Ne** ne funkcionira, provjerite sljedeće: 

- Korisnik se može prikazati s popisa primatelja u Exchange. Dodatne informacije potražite u članku [Upravljanje popisima adresa u programu Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#use-the-eac-to-hide-recipients-from-address-lists). 
- Korisnik se može prikazati s popisa adresa u Azure Active Directory. Dodatne informacije potražite u članku [Set-AzureADUser](https://docs.microsoft.com/powershell/module/azuread/set-azureaduser?view=azureadps-2.0). 