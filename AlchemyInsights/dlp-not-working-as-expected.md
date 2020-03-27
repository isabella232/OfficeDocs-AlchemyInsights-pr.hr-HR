---
title: DLP ne radi prema očekivanom
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 1/9/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: 574a8a43d8264e98c6af2bfeb1bb472475e6e334
ms.sourcegitcommit: d108a2da2f5dab05246e30b5108cca5173e09051
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/26/2020
ms.locfileid: "42977430"
---
# <a name="dlp-not-working-as-expected"></a>DLP ne radi prema očekivanom

**Važno**: Tijekom ovih dosad nezabilježenih vremena poduzimamo korake kako bismo osigurali da usluge sustava SharePoint Online i onedrive ostanu vrlo dostupne – dodatne informacije [potražite u članku Prilagodbe privremenih značajki sustava SharePoint Online.](https://aka.ms/ODSPAdjustments)

 **Postavljanje DLP-a**

Imate li problema s **asprječavanjegubitka podataka (DLP)** u sustavu Office 365 koji ne funkcionira prema i očekivanom? Ako je tako, provjerite je li **pravilo dlp-a** ispravno postavljeno i sadrže li vaši podaci ono što **pravila DLP-a** traže prilikom procjene.
  
DLP pravila omogućuju prepoznavanje i zaštitu osjetljivih informacija u tvrtki ili ustanovi. Da biste postavili DLP pravila, koristite informacije [ovdje](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).
  
 **Što traže politike DLP-a**
  
Kada koristite **ugrađene osjetljive vrste informacija** u centru za sigurnost i usklađenost sustava Office 365, DLP pravila traže određene uzorke i elemente prilikom otkrivanja tih osjetljivih vrsta.
  
- **Ugrađene vrste osjetljivih informacija**

    Informacije o ugrađenim osjetljivim vrstama i što traži DLP pravilo prilikom otkrivanja osjetljive vrste [potražite u odjeljku Sljedeće koje osjetljive vrste informacija traži](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).

- **Prilagođene vrste osjetljivih informacija**

    Ako pokušavate stvoriti prilagođene vrste osjetljivih informacija, koristite sljedeći članak za informacije o stvaranju prilagođene osjetljive vrste: [Stvaranje prilagođene osjetljive vrste informacija](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).

**Testiranje pravila o DLP-u**

Da biste testirali podatke pomoću ugrađene ili prilagođene osjetljive vrste informacija, upotrijebite opciju **Vrsta testiranja** u odjeljku **Klasifikacije Osjetljive** > **vrste podataka**. Dodatne informacije potražite [u odjeljku Testiranje prilagođenih osjetljivih vrsta informacija](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).

 **Izvješća**
  
- Dobijte uvid u osjetljive podatke pomoću [DLP izvješća.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)

- Pogledajte specifične pojedinosti događaja s [izvješćem o incidentu](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).
