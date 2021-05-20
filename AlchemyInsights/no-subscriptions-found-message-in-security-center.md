---
title: U centru za sigurnost nije pronađena poruka o pretplatama
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
ms.openlocfilehash: 777fb9b09aa26d166f9971589bda464ccb90f4be
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: HT
ms.contentlocale: hr-HR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52544100"
---
# <a name="no-subscriptions-found-message-in-the-security-center"></a><span data-ttu-id="f8353-102">U centru za sigurnost nije pronađena poruka o pretplatama</span><span class="sxs-lookup"><span data-stu-id="f8353-102">No subscriptions found message in the Security Center</span></span>

<span data-ttu-id="f8353-103">Ako prilikom pristupa Microsoft Defender Security Center poruku "Nema pronađenih pretplata", to znači da Azure Active Directory (AAD) koji se koristi za prijavu korisnika na portal nema licencu za Microsoft Defender ATP.</span><span class="sxs-lookup"><span data-stu-id="f8353-103">If while accessing Microsoft Defender Security Center you get a "No subscriptions found" message, it means the Azure Active Directory (AAD) used to login the user to the portal doesn't have a Microsoft Defender ATP license.</span></span>  

<span data-ttu-id="f8353-104">Licence Windows E5 i Office E5 zasebne su licence.</span><span class="sxs-lookup"><span data-stu-id="f8353-104">The Windows E5 and Office E5 licenses are separate licenses.</span></span>

<span data-ttu-id="f8353-105">Otvorite slučaj podrške ako je licenca kupljena, ali nije dodijeljena ovoj instanci AAD-a.</span><span class="sxs-lookup"><span data-stu-id="f8353-105">Open a support case if the license was purchased but not provisioned to this AAD instance.</span></span> <span data-ttu-id="f8353-106">Imate sljedeće:</span><span class="sxs-lookup"><span data-stu-id="f8353-106">Either you have:</span></span> <br/>
-   <span data-ttu-id="f8353-107">Mogući problem s dodjelom licenci.</span><span class="sxs-lookup"><span data-stu-id="f8353-107">A possible license provisioning issue.</span></span><br/>
-   <span data-ttu-id="f8353-108">Nenamjerno ste licencu dodijeliti microsoftu AAD-u koji se razlikuje od one koja se koristi za provjeru autentičnosti u servis.</span><span class="sxs-lookup"><span data-stu-id="f8353-108">You inadvertently provisioned the license to a different Microsoft AAD than the one used for authentication into the service.</span></span>