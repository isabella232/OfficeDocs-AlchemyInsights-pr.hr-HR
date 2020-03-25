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
ms.openlocfilehash: a56e18ddadef3a2f9056978b8542c1dba8f29665
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932614"
---
# <a name="dlp-not-working-as-expected"></a>DLP ne radi prema očekivanom

**Važno**: Mnogi korisnici sustava SharePoint Online i OneDrive pokrenuti poslovne kritične aplikacije protiv servisa koji se izvodi u pozadini. To uključuje migraciju sadržaja, sprječavanje gubitka podataka (DLP) i sigurnosna rješenja. Tijekom ovih dosad nezabilježenih vremena poduzimamo korake kako bismo osigurali da usluge sustava SharePoint Online i OneDrive ostanu vrlo dostupne i pouzdane za korisnike koji više nego ikad ovise o usluzi.

U prilog tom cilju, implementirali smo stroža ograničenja regulacije pozadinskih aplikacija (migracije, DLP i backup rješenja) tijekom radnih dana. Trebali biste očekivati da ove aplikacije će postići vrlo ograničen propusnost tijekom tih vremena. Međutim, tijekom večernjih i vikend sati za regiju, usluga će biti spremna za obradu znatno veći volumen zahtjeva iz pozadinskih aplikacija.

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
