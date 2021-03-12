---
title: Pravila lozinke
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/11/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "9277"
ms.openlocfilehash: 826e266d08aa68c0d4213d8058a0244f404fe965
ms.sourcegitcommit: 186281d0b87d67f041c127d4334faa937da9a48a
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50743440"
---
# <a name="password-policies"></a><span data-ttu-id="2cd96-102">Pravila lozinke</span><span class="sxs-lookup"><span data-stu-id="2cd96-102">Password policies</span></span>

<span data-ttu-id="2cd96-103">**Imam problema s pravilima o lozinkama za korisnika**</span><span class="sxs-lookup"><span data-stu-id="2cd96-103">**I'm having problems with the password policy for a user**</span></span>

- <span data-ttu-id="2cd96-104">Pravilnik o lozinci za korisnika ovisi o tome je li korisnik samo oblak ili lokalni.</span><span class="sxs-lookup"><span data-stu-id="2cd96-104">The password policy for a user depends on whether the user is cloud only or on-premises.</span></span>
- <span data-ttu-id="2cd96-105">U oblaku samo korisnici moraju odabrati lozinku koja zadovoljava preduvjete u ovom članku: [pravila lozinke koja se primjenjuju samo na korisničke račune u oblaku](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#password-policies-that-only-apply-to-cloud-user-accounts)</span><span class="sxs-lookup"><span data-stu-id="2cd96-105">Cloud only users must choose a password that meets the requirements in this article: [Password policies that only apply to cloud user accounts](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#password-policies-that-only-apply-to-cloud-user-accounts)</span></span>
- <span data-ttu-id="2cd96-106">Lokalni korisnici moraju odabrati lozinku koja zadovoljava lokalne preduvjete.</span><span class="sxs-lookup"><span data-stu-id="2cd96-106">On-premises users must choose a password that meets the on-premises requirements.</span></span> <span data-ttu-id="2cd96-107">Ako lokalni korisnik ne može postaviti lozinku, provjerite lokalne preduvjete.</span><span class="sxs-lookup"><span data-stu-id="2cd96-107">If an on-premises user is unable to set their password, check your on-premises requirements.</span></span>

<span data-ttu-id="2cd96-108">**Ne znam kako postaviti ili provjeriti pravila isteka lozinke**</span><span class="sxs-lookup"><span data-stu-id="2cd96-108">**I don't know how to set or check password expiration policies**</span></span>

- <span data-ttu-id="2cd96-109">Možete postaviti i provjeriti pravilnik o isteku za korisnike oblaka u svom zakupcu pomoću komponente PowerShell.</span><span class="sxs-lookup"><span data-stu-id="2cd96-109">You can set and check the expiration policy for cloud users in your tenant by using PowerShell.</span></span> <span data-ttu-id="2cd96-110">Slijedite upute u ovom članku: [Postavljanje ili provjera pravilnika o lozinci pomoću komponente PowerShell](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)</span><span class="sxs-lookup"><span data-stu-id="2cd96-110">Follow the instructions in this article: [Set or check the password policies by using PowerShell](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)</span></span>
- <span data-ttu-id="2cd96-111">Pravilnik o isteku lozinke za lokalne korisnike postavljen je u lokalnom OGLASU.</span><span class="sxs-lookup"><span data-stu-id="2cd96-111">The password expiration policy for on-premises users is set in your on-premises AD.</span></span>

<span data-ttu-id="2cd96-112">**Ostale korisne veze:**</span><span class="sxs-lookup"><span data-stu-id="2cd96-112">**Other Helpful links:**</span></span>
- [<span data-ttu-id="2cd96-113">Početak rada s resetiranju lozinke</span><span class="sxs-lookup"><span data-stu-id="2cd96-113">Getting Started with Password Reset</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)
- [<span data-ttu-id="2cd96-114">Otklanjanje poteškoća s inicijalima administratora koji je pokrenuo lozinku</span><span class="sxs-lookup"><span data-stu-id="2cd96-114">Troubleshoot Administrator-initiated Password Reset</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshoot-the-password-reset-portal)
