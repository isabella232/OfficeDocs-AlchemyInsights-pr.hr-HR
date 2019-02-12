---
title: Kako onemogućiti vanjski grupe
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: 4d911c319c3e8e327f9b3af3ba67816e646bc468
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 02/12/2019
ms.locfileid: "29899128"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="0cf75-102">Kako onemogućiti vanjski grupe</span><span class="sxs-lookup"><span data-stu-id="0cf75-102">How to disable External Groups</span></span>

<span data-ttu-id="0cf75-p101">Vanjski messaging primjenjuje Exchange prijevoza pravila (ETRs), postavite određene proaktivne kontrole da biste spriječili tvrtke informacije iz zajednički koristi za Yammer. Za ograničavanje korisnicima stvaranje vanjskih grupa, potrebno je konfigurirati pravilo prijevoza Exchange (ETR), a zatim konfigurirajte Yammer koristiti pravilo Exchangeov Transport Blokiranje vanjskog messaging.</span><span class="sxs-lookup"><span data-stu-id="0cf75-p101">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared. In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span> 
  
<span data-ttu-id="0cf75-105">Kada ste stvorili pravilo u centru za Exchange Online admin, slijedite ove korake da biste postavili ETR za primjenu u servisu Yammer:</span><span class="sxs-lookup"><span data-stu-id="0cf75-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="0cf75-106">Prijavite se na Yammer kao administraciju provjereno i u **centru za administraciju servisa Yammer**, idite na C **ontent i sigurnosti \> sigurnosne postavke.**</span><span class="sxs-lookup"><span data-stu-id="0cf75-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **ontent and Security \> Security Settings.**</span></span>
    
- <span data-ttu-id="0cf75-107">U odjeljku **Vanjski Messaging**odaberite **nametnuti Exchange Online Exchange prijevoza pravila (ETRs) u servisu Yammer.**</span><span class="sxs-lookup"><span data-stu-id="0cf75-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>
    
- <span data-ttu-id="0cf75-108">Odaberite **Spremi**.</span><span class="sxs-lookup"><span data-stu-id="0cf75-108">Choose **Save**.</span></span> 
    
<span data-ttu-id="0cf75-109">Dodatne informacije potražite [kontrolu vanjski messaging u mrežu servisa Yammer s pravilima Exchangeov Transport](https://support.office.com/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9)</span><span class="sxs-lookup"><span data-stu-id="0cf75-109">For more information, see [Control external messaging in a Yammer network with Exchange Transport rules](https://support.office.com/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9)</span></span>
  

