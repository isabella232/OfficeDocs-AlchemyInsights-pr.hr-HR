---
title: Intune Exchange lokalni poveznik
ms.author: mandia
author: mandia
manager: dougeby
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6732"
- "9003775"
ms.openlocfilehash: 744758739c2ca839823d2c8b440ed7b0d9dd4f06ebbb6f19fe52041a6710c4b4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013956"
---
# <a name="intune-exchange-on-premise-connector"></a>Intune Exchange lokalni poveznik

Detalje o postavljanju poveznika između aplikacije Intune i Exchange koji se hostira lokalno potražite u sljedećoj dokumentaciji:

[Postavljanje lokalnog priključka intune Exchange na servisu Microsoft Intune Azure](https://docs.microsoft.com/intune/exchange-connector-install)

**Najčešća pitanja:**

P: Prilikom pokušaja postavili poveznik za Exchange prikazuje se pogreška kao što je "Verzija Exchange Exchange Connector nije podržana". Koji bi uzrok mogao biti?

O: Račun koji koristite licenciran je na odgovarajući način – mora imati aktivnu licencu za Intune

P: Je li moguće imati više Exchange poveznika?

O: Po klijentu aplikacije Intune po Exchange možete postaviti samo jedan Exchange tvrtke ili ustanove. Poveznik se može instalirati samo na jedan poslužitelj u tvrtki ili ustanovi za razmjenu više poslužitelja.

Osim toga, konektore nije moguće konfigurirati za Exchange lokalno i Exchange Online konfigurirane na istom klijentu.

P: Može li poveznik koristiti POLJE CAS kao vezu s Exchange?

O: Određivanje POLJA CAS nije podržana konfiguracija u postavljanju poveznika. Potrebno je navesti samo jedan poslužitelj i u konfiguracijskoj datoteci poveznika koji se može pronaći u

programski podaci\microsoft\microsoft Intune na lokalnom Exchange poveznik\ OnpremiseExchangeConnectorServiceConfiguration.xml

Pronađite sljedeću stavku ```<ExchangeWebServiceURL />``` i zamijenite URL poslužiteljem sustava Exchange.

**Primjer:**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```

Dodatne informacije o otklanjanju poteškoća potražite u sljedećoj dokumentaciji: Otklanjanje poteškoća s lokalnim [Exchange intune](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)

**Omogućivanje opširanog zapisivanja za Exchange poveznik**

1. Otvorite konfiguracijsku Exchange poveznik radi uređivanja.  
Datoteka se nalazi na : %ProgramData%\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml  

**Primjer:**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```
  
2. Pronađite TraceSourceLine pomoću sljedećeg ključa: OnPremisesExchangeConnectorService  
  
3. Promjena vrijednosti sourceLevel node iz Information ActivityTracing (zadano) u Verbose ActivityTracing  

**Primjer:**
```
<TraceSourceLine>  
<Key xsi:type="xsd:string">OnPremisesExchangeConnectorService</Key>  
<Value xsi:type="TraceSource">  
<SourceLevel>All</SourceLevel>  
<Listeners>  
<Listener>  
<ListenerType>CircularTraceListener</ListenerType>
<SourceLevel>Verbose ActivityTracing</SourceLevel>
```
4. Ponovno pokrenite Microsoft Intune Exchange servis  
5. Potpuna sinkronizacija na portalu Intune dok ne završi, a zatim ponovno promijenite XML u "Information ActivityTracing" (Informacije ActivityTracing) pa ponovno pokrenite Microsoft Intune Exchange servis.  
6. Mjesto zapisnika je: `%ProgramData%\Microsoft\Windows Intune Exchange Connector`