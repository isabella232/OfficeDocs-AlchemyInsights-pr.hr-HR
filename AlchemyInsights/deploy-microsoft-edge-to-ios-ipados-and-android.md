---
title: Implementacija sustava Microsoft Edge na iOS, iPadOS i Android
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/10/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8241"
- "9004604"
ms.openlocfilehash: 524e87ab57e29823361053093708c83831f19687
ms.sourcegitcommit: 03378c78eadac5d950802dcbacc328bca3314032
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 02/10/2021
ms.locfileid: "50194463"
---
# <a name="deploy-microsoft-edge-to-ios-ipados-and-android"></a><span data-ttu-id="4cfd6-102">Implementacija sustava Microsoft Edge na iOS, iPadOS i Android</span><span class="sxs-lookup"><span data-stu-id="4cfd6-102">Deploy Microsoft Edge to iOS, iPadOS, and Android</span></span>

<span data-ttu-id="4cfd6-103">Vođeni scenarij u nastavku pomoći će vam da dodijelite Microsoft Edge korisnicima sustava iOS, iPadOS i uređajima sa sustavom Android.</span><span class="sxs-lookup"><span data-stu-id="4cfd6-103">The guided scenario summarized below will help you assign Microsoft Edge to users of iOS, iPadOS, and Android devices.</span></span>

> [!NOTE]
> <span data-ttu-id="4cfd6-104">Ako ste korisnike blokirali u upisivanju mobilnih uređaja, ovaj vođeni scenarij neće funkcionirati, a korisnici će morati sami instalirati Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="4cfd6-104">If you blocked users from enrolling mobile devices, this guided scenario won't work and the users will need to install Microsoft Edge on their own.</span></span>

<span data-ttu-id="4cfd6-105">Vođeni scenarij obuhvaća sljedeće korake:</span><span class="sxs-lookup"><span data-stu-id="4cfd6-105">The guided scenario involves the following steps:</span></span>

1. [<span data-ttu-id="4cfd6-106">Preduvjeti</span><span class="sxs-lookup"><span data-stu-id="4cfd6-106">Prerequisites</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#prerequisites)
2. [<span data-ttu-id="4cfd6-107">Uvod</span><span class="sxs-lookup"><span data-stu-id="4cfd6-107">Introduction</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-1---introduction)
3. [<span data-ttu-id="4cfd6-108">Osnove</span><span class="sxs-lookup"><span data-stu-id="4cfd6-108">Basics</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-2---basics)
4. [<span data-ttu-id="4cfd6-109">Konfiguracije</span><span class="sxs-lookup"><span data-stu-id="4cfd6-109">Configuration</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-3---configuration)
5. [<span data-ttu-id="4cfd6-110">Zadatke</span><span class="sxs-lookup"><span data-stu-id="4cfd6-110">Assignments</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-4---assignments)
6. [<span data-ttu-id="4cfd6-111">Pregled i stvaranje</span><span class="sxs-lookup"><span data-stu-id="4cfd6-111">Review and creation</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-5---review--create)

<span data-ttu-id="4cfd6-112">Nakon dovršetka koraka u vođenom scenariju, Microsoft Intune pravila omogućit će sljedeće značajke sustava Microsoft Edge za tvrtke:</span><span class="sxs-lookup"><span data-stu-id="4cfd6-112">After you complete the steps in the guided scenario, Microsoft Intune policies will enable the following features of Microsoft Edge for business:</span></span>

- <span data-ttu-id="4cfd6-113">Dvostruki identitet</span><span class="sxs-lookup"><span data-stu-id="4cfd6-113">Dual identity</span></span>
- <span data-ttu-id="4cfd6-114">Integracija s pravilima zaštite aplikacija za Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="4cfd6-114">Integration with Microsoft Intune app protection policy</span></span>
- <span data-ttu-id="4cfd6-115">Integracija s proxy aplikacijom Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="4cfd6-115">Integration with Azure Active Directory Application Proxy</span></span>
- <span data-ttu-id="4cfd6-116">Tipkovni prečaci za upravljanje omiljenim i početnoj stranici</span><span class="sxs-lookup"><span data-stu-id="4cfd6-116">Managed favorites and home page shortcuts</span></span>
