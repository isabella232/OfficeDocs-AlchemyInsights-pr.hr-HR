---
title: U centru za sigurnost nije pronađena nijedna pretplata
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6028"
- "9001222"
ms.openlocfilehash: 01117bc535df14533e426fd2d31c336fccc75611
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/15/2020
ms.locfileid: "50713338"
---
# <a name="no-subscriptions-found-message-in-the-security-center"></a><span data-ttu-id="358fc-102">U centru za sigurnost nije pronađena nijedna pretplata</span><span class="sxs-lookup"><span data-stu-id="358fc-102">No subscriptions found message in the Security Center</span></span>

<span data-ttu-id="358fc-103">Ako prilikom pristupanja centru za sigurnost programa Microsoft Defender dobijete poruku "nije pronađena pretplata", to znači da je Azure Active Directory (AAD) koji se koristi za prijavu korisnika na portal nema licencu za Microsoft Defender ATP.</span><span class="sxs-lookup"><span data-stu-id="358fc-103">If while accessing Microsoft Defender Security Center you get a  "No subscriptions found" message, it means the Azure Active Directory (AAD) used to login the user to the portal doesn't have a Microsoft Defender ATP license.</span></span>  

<span data-ttu-id="358fc-104">Licence za Windows E5 i Office E5 zasebne su licence.</span><span class="sxs-lookup"><span data-stu-id="358fc-104">The Windows E5 and Office E5 licenses are separate licenses.</span></span>

<span data-ttu-id="358fc-105">Otvorite slučaj podrške ako je licenca kupljena, ali nije dodijeljena ovoj instanci AAD-a.</span><span class="sxs-lookup"><span data-stu-id="358fc-105">Open a support case if the license was purchased but not provisioned to this AAD instance.</span></span> <span data-ttu-id="358fc-106">Ili imate sljedeće:</span><span class="sxs-lookup"><span data-stu-id="358fc-106">Either you have:</span></span> <br/>
-   <span data-ttu-id="358fc-107">Mogući problem dodjele licenci.</span><span class="sxs-lookup"><span data-stu-id="358fc-107">A possible license provisioning issue.</span></span><br/>
-   <span data-ttu-id="358fc-108">Nehotice ste dodijelili licencu drugim Microsoftovim AAD-ju od one koja se koristi za provjeru autentičnosti u servisu.</span><span class="sxs-lookup"><span data-stu-id="358fc-108">You inadvertently provisioned the license to a different Microsoft AAD than the one used for authentication into the service.</span></span>