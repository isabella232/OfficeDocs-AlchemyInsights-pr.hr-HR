---
title: DLP ne funkcionira prema očekivanom
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
ms.openlocfilehash: e1049f160a9b92040095b6725fa5771218a0956d17f99ea8a6e9cc279e7c73f6
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54079694"
---
# <a name="dlp-not-working-as-expected"></a>DLP ne funkcionira prema očekivanom

**Važno**: Tijekom ovih neočekivanih vremena poduzimamo korake kako bismo osigurali da servisi SharePoint Online i OneDrive i dalje budu široko raspoloživi – dodatne informacije potražite u [Privremene prilagodbe značajke SharePoint Online](https://aka.ms/ODSPAdjustments).

 **Postavljanje DLP-a**

Imate li problema s **sprječavanjem gubitka podataka (DLP- om)** u Office 365 ne funkcionira na očekivani datum? Ako je tako, provjerite je li **pravilnik za DLP** pravilno postavljen te sadrže li vaši podaci ono što **DLP** pravilnik traži prilikom procjene.
  
DLP pravilnik omogućuje prepoznavanje i zaštitu osjetljivih podataka u tvrtki ili ustanovi. Da biste e-postavu DLP pravilnika e-aplikacije [](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template)
  
 **Koje DLP pravilnike potražite**
  
Prilikom korištenja **ugrađenih osjetljivih** vrsta podataka u centrima za sigurnost i usklađenost DLP-ovi prilikom otkrivanja tih osjetljivih vrsta potražite određene uzorke i elemente.
  
- **Ugrađene vrste osjetljivih informacija**

    Informacije o ugrađenim osjetljivim vrstama i o tome što DLP pravilnik traži prilikom otkrivanja osjetljive vrste potražite u članku: Što [osjetljive vrste podataka izgledaju](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).

- **Prilagođene osjetljive vrste podataka**

    Ako pokušavate stvoriti prilagođene osjetljive vrste podataka, informacije o stvaranju prilagođene osjetljive vrste potražite u sljedećem [članku: Stvaranje prilagođene osjetljive vrste podataka.](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type)

**Testiranje pravilnika o DLP-u**

Da biste testirajte podatke ugrađenom ili prilagođenom osjetljivom vrstom podataka, upotrijebite **mogućnost Vrsta** testiranja u **odjeljku Klasifikacije**  >  **Osjetljive vrste podataka**. Dodatne informacije potražite u članku [Testiranje prilagođenih osjetljivih vrsta podataka](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).

 **Izvješća**
  
- Nabavite osjetljive uvide u podatke pomoću [DLP izvješća.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)

- Pogledajte konkretne pojedinosti o događaju pomoću izvješća [o incidentu](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).
