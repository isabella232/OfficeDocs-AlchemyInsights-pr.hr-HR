---
title: Otklanjanje poteškoća s sigurnosnim vrhom za provjeru otkrivanja prijevara
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: e42b498070bf5d9bfc36110667da8cc0fd431524
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658402"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>Otklanjanje poteškoća s sigurnosnim vrhom za provjeru otkrivanja prijevara

Ako dobivate sigurnosnu dojavu na kojoj piše: "pošiljatelj nije uspeo da otkrije provjeru prijevara i možda neće biti ono što izgleda", onda Pošiljatelj nije prošao ni DKIM ni SPF provjere autentičnosti. Najbolji način za rješavanje toga jest da se pošiljatelj autorizira. Ako pošiljatelj šalje u vaše ime, morate ih odobriti dodavanjem IP adrese pošiljatelja u SPF zapis.
  
Dodatne informacije potražite [u članku Otklanjanje poteškoća s crvenim (sumnjivim) sigurnosnim vrhom za otkrivanje prijevare](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) .
  
Evo još nekih veza koje mogu pomoći:
  
- [Kako Microsoft koristi okvir pravilnik o pošiljatelju (SPF) da bi spriječio zavaravanje](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [Postavljanje SPF-a radi sprječavanja zavaravanja](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
