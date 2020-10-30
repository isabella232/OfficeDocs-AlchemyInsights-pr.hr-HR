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
# <a name="intune-exchange-on-premise-connector"></a><span data-ttu-id="e57b3-102">Intune Exchangeov konektor na lokaciji</span><span class="sxs-lookup"><span data-stu-id="e57b3-102">Intune Exchange on-premise Connector</span></span>

<span data-ttu-id="e57b3-103">Pojedinosti o postavljanju konektora između Intune i Exchange koji je domaćin lokalno potražite u sljedećoj dokumentaciji:</span><span class="sxs-lookup"><span data-stu-id="e57b3-103">For details of setting up the connector between Intune and Exchange which is hosted on-premises please see the following documentation:</span></span>

[<span data-ttu-id="e57b3-104">Postavljanje Intune lokalnog sustava Exchange Connector u programu Microsoft Intune Azure</span><span class="sxs-lookup"><span data-stu-id="e57b3-104">Set up the Intune on-premises Exchange connector in Microsoft Intune Azure</span></span>](https://docs.microsoft.com/intune/exchange-connector-install)

<span data-ttu-id="e57b3-105">**NAJČEŠĆA pitanja**</span><span class="sxs-lookup"><span data-stu-id="e57b3-105">**FAQ:**</span></span>

<span data-ttu-id="e57b3-106">P: prikazuje se pogreška kao što je "verzija poveznika sustava Exchange nije podržana" prilikom pokušaja postavljanja konektora sustava Exchange.</span><span class="sxs-lookup"><span data-stu-id="e57b3-106">Q: I see an error such as "The Exchange Connector version is not supported" when attempting to set up the Exchange connector.</span></span> <span data-ttu-id="e57b3-107">Što bi mogao biti uzrok?</span><span class="sxs-lookup"><span data-stu-id="e57b3-107">What could be the cause?</span></span>

<span data-ttu-id="e57b3-108">A: račun koji koristite licenciran je na odgovarajući način – mora imati aktivnu licencu za Intune</span><span class="sxs-lookup"><span data-stu-id="e57b3-108">A: The account you are using is licensed appropriately - it must have an active Intune license</span></span>

<span data-ttu-id="e57b3-109">P: je li moguće imati više konektora sustava Exchange?</span><span class="sxs-lookup"><span data-stu-id="e57b3-109">Q: Is it possible to have multiple Exchange connectors?</span></span>

<span data-ttu-id="e57b3-110">O: možete postaviti samo jedan poveznik sustava Exchange po neusklađeni stanar po tvrtki ili ustanovi za Exchange.</span><span class="sxs-lookup"><span data-stu-id="e57b3-110">A: You can only set up one Exchange connector per Intune tenant per Exchange organization.</span></span> <span data-ttu-id="e57b3-111">Poveznik se može instalirati samo na jednom poslužitelju u tvrtki ili ustanovi za razmjenu više poslužitelja.</span><span class="sxs-lookup"><span data-stu-id="e57b3-111">The connector can only be installed on one server in a multi server exchange organization.</span></span>

<span data-ttu-id="e57b3-112">I ne možete imati konfigurirane konektore za Exchange on-premisu i Exchange Online konfigurirane u istom zakupcu.</span><span class="sxs-lookup"><span data-stu-id="e57b3-112">Also you cannot have connectors configured for both Exchange on-premise and Exchange Online configured in the same tenant.</span></span>

<span data-ttu-id="e57b3-113">P: može li konektor koristiti CAS Array kao vezu sa sustavom Exchange?</span><span class="sxs-lookup"><span data-stu-id="e57b3-113">Q: Can the connector use a CAS array as its connection to Exchange?</span></span>

<span data-ttu-id="e57b3-114">A: određivanje CAS polja nije podržana konfiguracija u postavljanju poveznika.</span><span class="sxs-lookup"><span data-stu-id="e57b3-114">A: Specifying a CAS array is not a supported configuration in the connector setup.</span></span> <span data-ttu-id="e57b3-115">Trebao bi biti naveden samo jedan poslužitelj i trebao bi biti hardcore u konfiguracijskoj datoteci konektora koja se može pronaći u programu</span><span class="sxs-lookup"><span data-stu-id="e57b3-115">Only a single server should be specified and should be hardcoded in the connector configuration file which can be found in</span></span>

<span data-ttu-id="e57b3-116">programski data\microsoft\microsoft Intune na odjeljku premisa Exchange Connector \ OnpremiseExchangeConnectorServiceConfiguration.xml</span><span class="sxs-lookup"><span data-stu-id="e57b3-116">program data\microsoft\microsoft Intune on premise Exchange connector\ OnpremiseExchangeConnectorServiceConfiguration.xml</span></span>

<span data-ttu-id="e57b3-117">Pronađite sljedeći unos ```<ExchangeWebServiceURL />``` i zamijenite URL poslužiteljem sustava Exchange.</span><span class="sxs-lookup"><span data-stu-id="e57b3-117">Locate the following entry ```<ExchangeWebServiceURL />``` and replace the URL with the exchange server.</span></span>

<span data-ttu-id="e57b3-118">**Primjer**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```</span><span class="sxs-lookup"><span data-stu-id="e57b3-118">**Example:**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```</span></span>

<span data-ttu-id="e57b3-119">Dodatne informacije o otklanjanju poteškoća potražite u sljedećoj dokumentaciji: [Otklanjanje poteškoća s ubiranjem lokalnog sustava Exchange Connector](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)</span><span class="sxs-lookup"><span data-stu-id="e57b3-119">Please see the following documentation for additional troubleshooting: [Troubleshoot the Intune on-premises Exchange connector](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)</span></span>

<span data-ttu-id="e57b3-120">**Omogućivanje verbose zapisivanja za konektor sustava Exchange**</span><span class="sxs-lookup"><span data-stu-id="e57b3-120">**Enabling Verbose logging for the Exchange connector**</span></span>

1. <span data-ttu-id="e57b3-121">Otvorite konfiguracijsku datoteku praćenja Exchange Connector za uređivanje.</span><span class="sxs-lookup"><span data-stu-id="e57b3-121">Open the Exchange Connector tracing configuration file for editing.</span></span>  
<span data-ttu-id="e57b3-122">Datoteka se nalazi na:%ProgramData%\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml</span><span class="sxs-lookup"><span data-stu-id="e57b3-122">The file is located at : %ProgramData%\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml</span></span>  

<span data-ttu-id="e57b3-123">**Primjer**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```</span><span class="sxs-lookup"><span data-stu-id="e57b3-123">**Example:**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```</span></span>
  
2. <span data-ttu-id="e57b3-124">Pronađite TraceSourceLine s sljedećim ključem: ifunkcija aprostorisexchangeconnectorservice</span><span class="sxs-lookup"><span data-stu-id="e57b3-124">Locate the TraceSourceLine with the following key: OnPremisesExchangeConnectorService</span></span>  
  
3. <span data-ttu-id="e57b3-125">Promjena vrijednosti čvora SourceLevel iz informacija ActivityTracing (zadano) na verbose ActivityTracing</span><span class="sxs-lookup"><span data-stu-id="e57b3-125">Change the SourceLevel node value from Information ActivityTracing (the default) to Verbose ActivityTracing</span></span>  

<span data-ttu-id="e57b3-126">**Primjer**</span><span class="sxs-lookup"><span data-stu-id="e57b3-126">**Example:**</span></span>
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
4. <span data-ttu-id="e57b3-127">Ponovno pokretanje servisa Microsoft Intune Exchange</span><span class="sxs-lookup"><span data-stu-id="e57b3-127">Restart the Microsoft Intune Exchange Service</span></span>  
5. <span data-ttu-id="e57b3-128">Potpuna sinkronizacija na portalu Intune dok ne završi, a zatim ponovno promijenite XML u "Information ActivityTracing" i ponovno pokrenite servis Microsoft Intune Exchange.</span><span class="sxs-lookup"><span data-stu-id="e57b3-128">Full sync in Intune Portal until it finishes and then change the XML back to "Information ActivityTracing" and restart the Microsoft Intune Exchange Service.</span></span>  
6. <span data-ttu-id="e57b3-129">Mjesto zapisnika jest: `%ProgramData%\Microsoft\Windows Intune Exchange Connector`</span><span class="sxs-lookup"><span data-stu-id="e57b3-129">Location of the logs is : `%ProgramData%\Microsoft\Windows Intune Exchange Connector`</span></span>