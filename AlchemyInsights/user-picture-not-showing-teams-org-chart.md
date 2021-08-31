---
title: Korisnička slika koja se ne prikazuje Microsoft Teams organizacijskom grafikonu
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/23/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12620"
- "9007457"
ms.openlocfilehash: 661b04913581ddd6650316298134ff9835ef3a90
ms.sourcegitcommit: 3986fa5377895cfc9fd98aca0739e599ebafb712
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/23/2021
ms.locfileid: "58792658"
---
# <a name="user-picture-not-showing-in-microsoft-teams-organization-chart"></a>Korisnička slika koja se ne prikazuje Microsoft Teams organizacijskom grafikonu

Ako jednoj ili više pojedinaca u vašoj tvrtki ili ustanovi nedostaje njihova profilna fotografija na organizacijskom grafikonu, **postavka ShowInAddressLists** postavljena je na **False:**

1. Idite na Centar za administratore okruženja Microsoft 365 > [**aktivni korisnici**](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users), a zatim odaberite korisnika s fotografijom koja nedostaje. 
1. Odaberite **karticu Pošta** i provjerite je li popis Pokaži na **globalnoj adresi** postavljen na **Da**. 

Ako **postavka ShowInAddressLists** na **Da** ne funkcionira, provjerite sljedeće:

- Korisnik je možda skriven s popisa primatelja u Exchange. Dodatne informacije potražite u članku [Upravljanje popisima adresa u programu Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#use-the-eac-to-hide-recipients-from-address-lists). 
- Korisnik je možda skriven s popisa adresa u Azure Active Directory. Dodatne informacije potražite u članku [Set-AzureADUser](https://docs.microsoft.com/powershell/module/azuread/set-azureaduser?view=azureadps-2.0). 
