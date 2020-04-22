---
title: DLP ne radi prema očekivanom
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
ms.openlocfilehash: efb4a19f345fe6b8a1e8bb72abeba4a923c05777
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704405"
---
# <a name="dlp-not-working-as-expected"></a>DLP ne radi prema očekivanom

**Važno**: Tijekom ovih neočekivanih vremena poduzimamo korake kako bismo osigurali da servisi SharePoint Online i OneDrive i dalje budu široko raspoloživi – dodatne informacije potražite u [Privremene prilagodbe značajke SharePoint Online](https://aka.ms/ODSPAdjustments).

 **Postavljanje DLP-a**

Imate li problema s **asprječavanjegubitka podataka (DLP)** u sustavu Office 365 koji ne funkcionira prema i očekivanom? Ako je tako, provjerite je li **pravilo dlp-a** ispravno postavljeno i sadrže li vaši podaci ono što **pravila DLP-a** traže prilikom procjene.
  
DLP pravila omogućuju prepoznavanje i zaštitu osjetljivih informacija u tvrtki ili ustanovi. Da biste postavili DLP pravila, koristite informacije [ovdje](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).
  
 **Što traže politike DLP-a**
  
Kada koristite **ugrađene osjetljive vrste informacija** u centrima za sigurnost i usklađenost, DLP pravila traže određene uzorke i elemente prilikom otkrivanja tih osjetljivih vrsta.
  
- **Ugrađene vrste osjetljivih informacija**

    Informacije o ugrađenim osjetljivim vrstama i što traži DLP pravilo prilikom otkrivanja osjetljive vrste [potražite u odjeljku Sljedeće koje osjetljive vrste informacija traži](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).

- **Prilagođene vrste osjetljivih informacija**

    Ako pokušavate stvoriti prilagođene vrste osjetljivih informacija, koristite sljedeći članak za informacije o stvaranju prilagođene osjetljive vrste: [Stvaranje prilagođene osjetljive vrste informacija](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).

**Testiranje pravila o DLP-u**

Da biste testirali podatke pomoću ugrađene ili prilagođene osjetljive vrste informacija, upotrijebite opciju **Vrsta testiranja** u odjeljku **Klasifikacije Osjetljive** > **vrste podataka**. Dodatne informacije potražite [u odjeljku Testiranje prilagođenih osjetljivih vrsta informacija](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).

 **Izvješća**
  
- Dobijte uvid u osjetljive podatke pomoću [DLP izvješća.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)

- Pogledajte specifične pojedinosti događaja s [izvješćem o incidentu](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).
