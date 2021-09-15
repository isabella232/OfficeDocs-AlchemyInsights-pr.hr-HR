---
title: Izvješća u Centru za administratore okruženja Microsoft 365 ne prikazuju čitljivo korisničko ime
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/02/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13809"
- "13810"
- "13812"
- "9008619"
ms.openlocfilehash: ff8eac6487ef544277c5ce2c0c0b7068c9d400ca
ms.sourcegitcommit: b47c6d5e74819b73becaf1dc5eacc72eaf7c1055
ms.translationtype: HT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/15/2021
ms.locfileid: "59327806"
---
# <a name="reports-in-microsoft-365-admin-center-do-not-show-readable-username"></a>Izvješća u Centru za administratore okruženja Microsoft 365 ne prikazuju čitljivo korisničko ime

Izvješća u Centru za administratore okruženja Microsoft 365 ne prikazuju korisnička imena, već umjesto toga prikazuju alfanumeričke vrijednosti kao što su B2BC6C15BB9FCDEA71E5CD302D228CC8.

Ovo je očekivano ponašanje i komunicira se u centru za poruke (MC275344, objavljeno 3. kolovoza 2021.). 

Globalni administratori mogu vratiti tu promjenu za klijenta i prikazati korisničke podatke koji se mogu utvrditi ako to dopuštaju prakse zaštite privatnosti tvrtke ili ustanove. Da biste vratili promjenu za klijent:

1. U centru za administratore idite na **Postavke** > **Usluge** > [**Tvrtke ili ustanove**](https://admin.microsoft.com/Adminportal/Home#/Settings/Services ) pa odaberite **Izvješća**. 
1. U odjeljku **odaberite kako prikazati korisničke podatke**, odaberite **Prikaži korisničke podatke koji se mogu utvrditi u izvješćima**, a zatim ponovo pokrenite izvješće.