---
title: Intune Exchangeov konektor na lokaciji
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
ms.openlocfilehash: 8b470655efa2dfb460c29b6b840fa793ed2aa448
ms.sourcegitcommit: f8b41ecda6db0b8f64fe0c51f1e8e6619f504d61
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 10/28/2020
ms.locfileid: "48807274"
---
# <a name="intune-exchange-on-premise-connector"></a>Intune Exchangeov konektor na lokaciji

Pojedinosti o postavljanju konektora između Intune i Exchange koji je domaćin lokalno potražite u sljedećoj dokumentaciji:

[Postavljanje Intune lokalnog sustava Exchange Connector u programu Microsoft Intune Azure](https://docs.microsoft.com/intune/exchange-connector-install)

**NAJČEŠĆA pitanja**

P: prikazuje se pogreška kao što je "verzija poveznika sustava Exchange nije podržana" prilikom pokušaja postavljanja konektora sustava Exchange. Što bi mogao biti uzrok?

A: račun koji koristite licenciran je na odgovarajući način – mora imati aktivnu licencu za Intune

P: je li moguće imati više konektora sustava Exchange?

O: možete postaviti samo jedan poveznik sustava Exchange po neusklađeni stanar po tvrtki ili ustanovi za Exchange. Poveznik se može instalirati samo na jednom poslužitelju u tvrtki ili ustanovi za razmjenu više poslužitelja.

I ne možete imati konfigurirane konektore za Exchange on-premisu i Exchange Online konfigurirane u istom zakupcu.

P: može li konektor koristiti CAS Array kao vezu sa sustavom Exchange?

A: određivanje CAS polja nije podržana konfiguracija u postavljanju poveznika. Trebao bi biti naveden samo jedan poslužitelj i trebao bi biti hardcore u konfiguracijskoj datoteci konektora koja se može pronaći u programu

programski data\microsoft\microsoft Intune na odjeljku premisa Exchange Connector \ OnpremiseExchangeConnectorServiceConfiguration.xml

Pronađite sljedeći unos ```<ExchangeWebServiceURL />``` i zamijenite URL poslužiteljem sustava Exchange.

**Primjer**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```

Dodatne informacije o otklanjanju poteškoća potražite u sljedećoj dokumentaciji: [Otklanjanje poteškoća s ubiranjem lokalnog sustava Exchange Connector](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)

**Omogućivanje verbose zapisivanja za konektor sustava Exchange**

1. Otvorite konfiguracijsku datoteku praćenja Exchange Connector za uređivanje.  
Datoteka se nalazi na:%ProgramData%\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml  

**Primjer**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```
  
2. Pronađite TraceSourceLine s sljedećim ključem: ifunkcija aprostorisexchangeconnectorservice  
  
3. Promjena vrijednosti čvora SourceLevel iz informacija ActivityTracing (zadano) na verbose ActivityTracing  

**Primjer**
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
4. Ponovno pokretanje servisa Microsoft Intune Exchange  
5. Potpuna sinkronizacija na portalu Intune dok ne završi, a zatim ponovno promijenite XML u "Information ActivityTracing" i ponovno pokrenite servis Microsoft Intune Exchange.  
6. Mjesto zapisnika jest: `%ProgramData%\Microsoft\Windows Intune Exchange Connector`