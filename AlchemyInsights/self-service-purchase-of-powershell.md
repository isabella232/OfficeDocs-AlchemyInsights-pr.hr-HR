---
title: Samoservisna Kupnja komponente PowerShell
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3516"
ms.openlocfilehash: e6cc504ebef19cbe78f576d9b207fe2d951d0ef5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47739962"
---
# <a name="self-service-purchase-of-powershell"></a><span data-ttu-id="6401f-102">Samoservisna Kupnja komponente PowerShell</span><span class="sxs-lookup"><span data-stu-id="6401f-102">Self-service purchase of PowerShell</span></span>

<span data-ttu-id="6401f-103">Da biste koristili modul MSCommerce PowerShell, morate ga instalirati na uređaj sa sustavom Windows 10 s TLS 1,2 (potrebne su lokalne administratorske dozvole).</span><span class="sxs-lookup"><span data-stu-id="6401f-103">To use the MSCommerce PowerShell module, you need to install it on a Windows 10 device with TLS 1.2 (local administrator permissions required).</span></span>  <span data-ttu-id="6401f-104">Uvezite i povežite se s modulom MSCommerce.</span><span class="sxs-lookup"><span data-stu-id="6401f-104">Import and connect to the MSCommerce module.</span></span>  <span data-ttu-id="6401f-105">Kada se od vas zatraži prijava, morat ćete koristiti vjerodajnice globalne ili administratorske uloge.</span><span class="sxs-lookup"><span data-stu-id="6401f-105">When prompted to log in, you will need to use Global or Billing Admin role credentials.</span></span>  

<span data-ttu-id="6401f-106">Ako nemate TLS 1,2, možda će se prilikom pokušaja ažuriranja pravilnika pojaviti sljedeća pogreška:</span><span class="sxs-lookup"><span data-stu-id="6401f-106">If you don't have TLS 1.2, you may receive the following error when attempting to get or update the policy:</span></span>

<span data-ttu-id="6401f-107">*ErrorMessage – veza u podlozi je zatvorena: došlo je do neočekivane pogreške na slanju*.</span><span class="sxs-lookup"><span data-stu-id="6401f-107">*ErrorMessage -The underlying connection was closed: An unexpected error occurred on a send*.</span></span>



