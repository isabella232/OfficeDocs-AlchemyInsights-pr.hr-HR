---
title: Otvori pomoću programa Explorer ne radi
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 12/10/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: f788c3c626cdeb19970edb59563c59eea60e2992
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 02/12/2019
ms.locfileid: "29906796"
---
# <a name="open-with-explorer-isnt-working"></a>Otvori pomoću programa Explorer ne radi

**Otvori pomoću programa Explorer** ili **Prikaz Explorer datoteka** ne radi Provjerite je li servis WebClient je postavljeno na **izvodi** slijedeći dolje navedene korake. Na primjer, ga potrajati dugo otvorite biblioteku SharePoint ili OneDrive kada servis nije pokrenut. 
  
1. U okvir za pretraživanje Windows vrsta pokrenuti, odaberite Pokreni radne površine app, vrsta services.msc i zatim odaberite **Enter**.
    
2. Pomaknite WebClient servisa i provjerite stupac **Stanje** . Servis stanja WebClient nije **pokrenut**, dvaput kliknite servis, kliknite **Start**, a zatim kliknite **u redu**. Omogućiti servis, ako je potrebno, odabirom **ručno** ili **Automatsko** u okviru **Vrsta pokretanja** . 
    
> [!NOTE]
> Za rješavanje problema s otvaranjem datoteka Explorer vidjeti [otvorene u programu Explorer](https://go.microsoft.com/fwlink/?linkid=871665). Istražite sinkronizaciju kao bolja alternativa: [SharePoint sinkronizaciju datoteke s novom klijentu sinkronizaciju OneDrive](https://go.microsoft.com/fwlink/?linkid=871666). 
  

