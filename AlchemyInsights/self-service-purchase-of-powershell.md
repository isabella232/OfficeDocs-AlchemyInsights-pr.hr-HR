---
title: Samoposlužna kupnja komponente PowerShell
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3516"
ms.openlocfilehash: 5e47e08e3309b3d58908e10ee06021da00f230bb
ms.sourcegitcommit: cb9505f9eca032af3a4194c68d18c91789365690
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 02/16/2020
ms.locfileid: "42091673"
---
# <a name="self-service-purchase-of-powershell"></a><span data-ttu-id="ee5d5-102">Samoposlužna kupnja komponente PowerShell</span><span class="sxs-lookup"><span data-stu-id="ee5d5-102">Self-service purchase of PowerShell</span></span>

<span data-ttu-id="ee5d5-103">Da biste koristili modul MSCommerce PowerShell, morate ga instalirati na uređaj sa sustavom Windows 10 s TLS 1.2 (potrebne su dozvole lokalnog administratora).</span><span class="sxs-lookup"><span data-stu-id="ee5d5-103">To use the MSCommerce PowerShell module, you need to install it on a Windows 10 device with TLS 1.2 (local administrator permissions required).</span></span>  <span data-ttu-id="ee5d5-104">Uvoz i povezivanje s modulom MSCommerce.</span><span class="sxs-lookup"><span data-stu-id="ee5d5-104">Import and connect to the MSCommerce module.</span></span>  <span data-ttu-id="ee5d5-105">Kada se od vas zatraži prijava, morat ćete koristiti vjerodajnice uloge globalne ili administratorske administracije naplate.</span><span class="sxs-lookup"><span data-stu-id="ee5d5-105">When prompted to log in, you will need to use Global or Billing Admin role credentials.</span></span>  

<span data-ttu-id="ee5d5-106">Ako nemate TLS 1.2, prilikom pokušaja primanja ili ažuriranja pravila možete primiti sljedeću pogrešku:</span><span class="sxs-lookup"><span data-stu-id="ee5d5-106">If you don't have TLS 1.2, you may receive the following error when attempting to get or update the policy:</span></span>

<span data-ttu-id="ee5d5-107">*ErrorMessage -Veza u podlozi je zatvorena: Došlo je do neočekivane pogreške prilikom slanja*.</span><span class="sxs-lookup"><span data-stu-id="ee5d5-107">*ErrorMessage -The underlying connection was closed: An unexpected error occurred on a send*.</span></span>



