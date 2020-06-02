---
title: DLP ne radi prema očekivanjima
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: e96904e2f0da2fe1fafb3f8722465eaf22681b71
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507470"
---
# <a name="dlp-not-working-as-expected"></a>DLP ne radi prema očekivanjima

**Važno**: Tijekom ovih neočekivanih vremena poduzimamo korake kako bismo osigurali da servisi SharePoint Online i OneDrive i dalje budu široko raspoloživi – dodatne informacije potražite u [Privremene prilagodbe značajke SharePoint Online](https://aka.ms/ODSPAdjustments).

 **Postavljanje DLP-a**

Imate li problema sa **sprječavanjem gubitka podataka (DLP)** u sustavu Office 365 koji ne funkcioniraju prema očekivanjima? Ako je tako, provjerite je li **pravilo DLP** ispravno postavljeno i sadrži li vaši podaci ono što **pravilo DLP-a** traži prilikom procjene.
  
DLP pravila omogućuju vam prepoznavanje i zaštitu osjetljivih podataka u tvrtki ili ustanovi. Da biste postavili DLP pravila, ovdje koristite [informacije](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).
  
 **Što DLP politike traže**
  
Kada koristite **ugrađene vrste osjetljivih informacija** u centrima za sigurnost i usklađenost, DLP pravila traže određene uzorke i elemente prilikom otkrivanja tih osjetljivih vrsta.
  
- **Ugrađene vrste osjetljivih informacija**

    Informacije o ugrađenim osjetljivim vrstama i što DLP pravilo traži prilikom otkrivanja vrste Osjetljivo [potražite u odjeljku Što traže vrste osjetljivih informacija](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).

- **Prilagođene vrste osjetljivih informacija**

    Ako pokušavate stvoriti prilagođene vrste osjetljivih informacija, koristite sljedeći članak za informacije o stvaranju prilagođene osjetljive vrste: [Stvaranje prilagođene vrste osjetljivih informacija](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type).

**Testiranje pravila O DLP-u**

Da biste testirali podatke s ugrađenom ili prilagođenom osjetljivom vrstom informacija, upotrijebite mogućnost **Vrsta testiranja** u odjeljku **Vrste osjetljivih podataka Klasifikacije**  >  **Sensitive info types**. Dodatne informacije potražite u [odjeljku Testiranje prilagođenih vrsta osjetljivih informacija](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).

 **Izvješća**
  
- Dobijte osjetljive uvide u podatke pomoću [DLP izvješća.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)

- Pogledajte određene pojedinosti događaja pomoću [izvješća o incidentu](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).
