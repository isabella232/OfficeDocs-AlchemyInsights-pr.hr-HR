---
title: Postavljanje preglednika Microsoft Edge kao zadanog preglednika na uređaju sa sustavom macOS
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10362"
- "9006005"
ms.openlocfilehash: 5318c7d20ee7091e162e566cd2b4ebf5d255915b
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/30/2021
ms.locfileid: "51491360"
---
# <a name="set-microsoft-edge-as-the-default-browser-on-a-macos-device"></a>Postavljanje preglednika Microsoft Edge kao zadanog preglednika na uređaju sa sustavom macOS

Pomoću jedne od ova dva načina postavite Microsoft Edge kao zadani preglednik:

Prvi način: flash uređaj sa slikom sustava macOS na kojoj je Microsoft Edge već postavljen kao zadani preglednik.

Drugi način: postavite pravilnik DefaultBrowserSettingEnabled tako da od korisnika zatraži postavljanje preglednika Microsoft Edge kao zadanog preglednika.

Oba načina korisniku omogućuju promjenu zadanog preglednika. Zato preporučujemo implementaciju pravilnika DefaultBrowserSettingEnabled čak i ako ste koristili 1. metodu. Ako korisnik promijeni zadani preglednik nakon primjene pravilnika, pravilnik će od korisnika zatražiti da vrati zadani preglednik na Microsoft Edge.
