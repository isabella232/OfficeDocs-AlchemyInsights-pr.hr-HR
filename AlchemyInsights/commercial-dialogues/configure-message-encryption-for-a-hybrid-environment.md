---
title: Konfiguriranje šifriranja poruke za hibridno okruženje
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: 22c2468b7639680b447b6464431a79b69f7198c3
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50743579"
---
# <a name="configure-message-encryption-for-a-hybrid-environment"></a><span data-ttu-id="8c402-102">Konfiguriranje šifriranja poruke za hibridno okruženje</span><span class="sxs-lookup"><span data-stu-id="8c402-102">Configure message encryption for a hybrid environment</span></span>

<span data-ttu-id="8c402-103">Za hibridnu Exchange okruženja lokalni korisnici mogu slati šifriranu e-poštu pomoću šifriranja poruke sustava Office (om) samo ako je e-pošta usmjerena putem sustava Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="8c402-103">For hybrid Exchange environments, on-premises users can send encrypted email using Office Message Encryption (OME) only if email is routed through Exchange Online.</span></span>

<span data-ttu-id="8c402-104">Da biste šifrirali poruke e-pošte pomoću sustava Oma, učinite sljedeće:</span><span class="sxs-lookup"><span data-stu-id="8c402-104">To encrypt emails using OME, perform the following steps:</span></span>

1. <span data-ttu-id="8c402-105">Pomoću [čarobnjaka za hibridnu konfiguraciju](https://docs.microsoft.com/Exchange/hybrid-configuration-wizard) postavite hibridno okruženje.</span><span class="sxs-lookup"><span data-stu-id="8c402-105">Use the [Hybrid Configuration wizard](https://docs.microsoft.com/Exchange/hybrid-configuration-wizard) to set up your hybrid environment.</span></span> <span data-ttu-id="8c402-106">Za postavljanje šifriranja nije potrebna nijedna specijalna koraka.</span><span class="sxs-lookup"><span data-stu-id="8c402-106">No special steps are required for setting up encryption.</span></span>
2. <span data-ttu-id="8c402-107">[Postavite pravila protoka pošte radi šifriranja](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email) kao što to obično činite.</span><span class="sxs-lookup"><span data-stu-id="8c402-107">[Set up your mail flow rules for encryption](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email) like you normally would.</span></span>


