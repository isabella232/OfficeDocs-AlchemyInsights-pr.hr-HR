---
title: Otklanjanje poteškoća sa sigurnosnim savjetom za provjere otkrivanja prijevara
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: 85faa0086935fb7e7132ee9fdced546bafdb344c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834723"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>Otklanjanje poteškoća sa sigurnosnim savjetom za provjere otkrivanja prijevara

Ako vam se prikaže savjet o sigurnosti na koji piše "Pošiljatelj nije uspio provjeriti naše provjere otkrivanja prijevare i možda nije onaj koji izgleda kao da je", pošiljatelj nije uspio proći provjere DKIM ili SPF provjere autentičnosti. Najbolji način rješavanja tog problema jest da pošiljatelj odobri sam sebe. Ako pošiljatelj šalje u vaše ime, morate ih autorizirati dodavanjem IP adrese pošiljatelja u SPF zapis.
  
Dodatne [informacije potražite u članku Otklanjanje poteškoća s crvenim (sumnjivim) sigurnosnim savjetom](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) za provjeru otkrivanja prijevara.
  
Evo nekih drugih veza koje vam mogu pomoći:
  
- [Kako Microsoft koristi okvir pravilnika pošiljatelja (SPF) radi sprječavanja podvala](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [Postavljanje SPF-a radi sprječavanja podvala](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
