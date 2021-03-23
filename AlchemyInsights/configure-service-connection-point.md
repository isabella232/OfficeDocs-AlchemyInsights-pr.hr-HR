---
title: Konfiguriranje točke povezivanja servisa (SCP)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9732"
- "9003244"
ms.openlocfilehash: 9d733a1a0a3b8d92bdd5477a8978b6fbeede9653
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035097"
---
# <a name="configure-service-connection-point-scp"></a>Konfiguriranje točke povezivanja servisa (SCP)

**DSREG_AUTOJOIN_ADCONFIG_READ_FAILED (0x801c001d/-2145648611)**

- **Razlog**: nije moguće pročitati objekt SCP i nabaviti informacije o klijentu za Azure ad
- **Rezolucija**: Pogledajte odjeljak [Konfiguriranje točke povezivanja servisa](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains#configure-hybrid-azure-ad-join)


**Akcijski plan**

- Provjerite je li uređaj primio GPO za kontroliranu provjeru valjanosti.
- Provjerite je li GPO stvorio ključeve registra.
- Provjerite imate li dva ključa stvorena pomoću ID-a direktorija i domene u sustavu Microsoft.

**Konfiguriranje postavke registra na klijentskoj strani za SCP**

Pomoću sljedećeg primjera stvorite objekt pravilnika grupe (GPO) da biste implementirali postavku registra koja u registru uređaja konfigurira unos u SCP-u.

1. Otvorite konzolu za upravljanje pravilima grupe i stvorite novi GPO u svojoj domeni.
     - Navedite novostvoreni GPO naziv (primjerice, ClientSideSCP)

2. Uredite GPO i pronađite sljedeći put: postavke **računalne > postavke > Windows > Registry**.

3. Desnom tipkom miša kliknite **Registry** , a zatim odaberite **Nova > stavka registra**.

4. Na kartici **Općenito** konfigurirajte sljedeće:
  
- **Akcija**: Ažuriranje
    
- **Košnica**: HKEY_LOCAL_MACHINE
    
- **Ključ puta**: Software\microsoft\windows\currentversion\cdj\aad
    
- **Naziv vrijednosti**: tenantid
    
- **Vrsta vrijednosti**: REG_SZ
    
- **Podaci o vrijednosti**: ID GUID-a ili direktorij vaše instance Azure AD (ta se vrijednost može pronaći u **portalu Azure > azure Active directory > svojstva > ID direktorija**)
 
- Kliknite **U redu**.
 
5. Desnom tipkom miša kliknite **Registry** , a zatim odaberite **Nova > stavka registra**.

6. Na kartici **Općenito** konfigurirajte sljedeće:
  
- **Akcija**: Ažuriranje
    
- **Košnica**: HKEY_LOCAL_MACHINE
    
- **Ključ puta**: Software\microsoft\windows\currentversion\cdj\aad
    
- **Naziv vrijednosti**: tenantname
    
- **Vrsta vrijednosti**: REG_SZ
    
- **Podaci o vrijednosti**: potvrđeni naziv domene ako koristite Sjedinjenih okruženja kao što je AD FS. Potvrđeni naziv domene ili naziv domene onmicrosoft.com (primjerice contoso. inmicrosoft). com ako koristite upravljano okruženje

- Kliknite **U redu**.

7. Zatvaranje uređivača za novostvorenog GPO-a.

8. Povežite novostvorenu GPO u željenu domenu koja sadrži računala koja pripadaju vašoj kontroliranoj populaciji.

Dodatne informacije potražite u članku [kontrolirana provjera valjanosti hibridne Azure ad Join-Azure ad | Microsoft docs](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control) i  [Otklanjanje poteškoća s hibridom Azure Active Directory pridruženi uređaji | Microsoftovi dokumenti](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current).









