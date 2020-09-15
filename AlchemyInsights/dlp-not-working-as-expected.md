---
title: DLP ne funkcionira kako je očekivano
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: 0ed893420b5813d5d18639c2c226c12f0306a13f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679685"
---
# <a name="dlp-not-working-as-expected"></a>DLP ne funkcionira kako je očekivano

**Važno**: Tijekom ovih neočekivanih vremena poduzimamo korake kako bismo osigurali da servisi SharePoint Online i OneDrive i dalje budu široko raspoloživi – dodatne informacije potražite u [Privremene prilagodbe značajke SharePoint Online](https://aka.ms/ODSPAdjustments).

 **Postavljanje DLP-a**

Imate li problema s **prevencijom gubitka podataka (DLP)** u sustavu Office 365 ne funkcionira kao što ste očekivali? Ako je tako, provjerite je li **pravilnik za DLP** ispravno postavljen i sadrže li podaci što **pravilnik o DLP** -u traži kada se ona procjenjuje.
  
DLP pravila omogućuju vam identifikaciju i zaštitu osjetljivih podataka u tvrtki ili ustanovi. Da biste postavljanje DLP pravilnika, upotrijebite informacije [ovdje](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).
  
 **Koje su politike programa DLP potražili**
  
Kada koristite **ugrađene vrste osjetljivih informacija** u centrima za sigurnost i usklađenost, DLP politike potražite određene obrasce i elemente prilikom otkrivanja tih osjetljivih vrsta.
  
- **Ugrađene vrste osjetljivih informacija**

    Informacije o ugrađenim osjetljivim vrstama i onome što funkcija DLP traži prilikom otkrivanja osjetljive vrste potražite u članku: [što vrste osjetljivih informacija traže](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).

- **Prilagođene vrste osjetljivih informacija**

    Ako pokušavate stvoriti prilagođene vrste osjetljivih podataka, upotrijebite sljedeći članak da biste saznali kako stvoriti prilagođenu vrstu osjetljivog oblika: [Stvaranje prilagođene vrste osjetljivih podataka](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type).

**Testiranje pravilnika o DLP-u**

Da biste testirali podatke pomoću ugrađene ili prilagođene vrste osjetljivih informacija, upotrijebite mogućnost **vrsta testa** u odjeljku **razvrstavanje**  >  **osjetljivih podataka**. Dodatne informacije potražite u članku [testiranje prilagođenih vrsta podataka koje se razlikuju](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).

 **Izvješća**
  
- Dohvaćanje osjetljivih podataka iz uvida u [izvještaje programa DLP.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)

- Pogledajte detaljne pojedinosti o događaju uz izvješće o [incidentu](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).
