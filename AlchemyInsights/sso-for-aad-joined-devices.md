---
title: Single-Sign za pridružene uređaje servisa Azure Active Directory
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "9891"
ms.openlocfilehash: f6426a3fb4addc24c5041196fe837134bf0d296b
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/29/2021
ms.locfileid: "51404361"
---
# <a name="single-sign-on-for-azure-active-directory-joined-devices"></a><span data-ttu-id="97ffa-102">Jednostruka prijava za uređaje pridružene servisu Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="97ffa-102">Single-sign on for Azure Active Directory Joined Devices</span></span>

<span data-ttu-id="97ffa-103">Ako imate lokalno okruženje servisa Active Directory (AD) i želite se pridružiti računalima pridruženima AD domeni servisu Azure AD, to možete postići hibridnim pridruživanjem servisa Azure AD.</span><span class="sxs-lookup"><span data-stu-id="97ffa-103">If you have an on-premises Active Directory (AD) environment and you want to join your AD domain-joined computers to Azure AD, you can accomplish this by doing hybrid Azure AD join.</span></span> <span data-ttu-id="97ffa-104">[Upute: planiranje hibridne implementacije pridruživanja servisa Azure Active Directory](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) nudi vam povezane korake za implementaciju hibridnog pridruživanja servisa Azure AD u okruženju.</span><span class="sxs-lookup"><span data-stu-id="97ffa-104">[How To: Plan your hybrid Azure Active Directory join implementation](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) provides you with the related steps to implement a hybrid Azure AD join in your environment.</span></span>

[<span data-ttu-id="97ffa-105">Konfiguriranje uređaja pridruženih servisu Azure AD za lokalne Single-Sign u sustavu Windows Hello za tvrtke</span><span class="sxs-lookup"><span data-stu-id="97ffa-105">Configure Azure AD joined devices for On-premises Single-Sign On using Windows Hello for Business</span></span>](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) 

<span data-ttu-id="97ffa-106">**Problemi s tokenom primarnog osvježavanja (PRT)** Primarni token za osvježavanje (PRT) ključan je element provjere autentičnosti servisa Azure AD na uređajima sa sustavom Windows 10, Windows Server 2016 i novijim verzijama, uređajima sa sustavom iOS i Android.</span><span class="sxs-lookup"><span data-stu-id="97ffa-106">**Primary Refresh Token (PRT) issues** A Primary Refresh Token (PRT) is a key artifact of Azure AD authentication on Windows 10, Windows Server 2016 and later versions, iOS, and Android devices.</span></span> <span data-ttu-id="97ffa-107">To je JSON web-token (JWT) koji je posebno izdan Microsoftovim tokenima za tokene prve strane da bi omogućio jedinstvenu prijavu (SSO) u aplikacijama koje se koriste na tim uređajima.</span><span class="sxs-lookup"><span data-stu-id="97ffa-107">It is a JSON Web Token (JWT) specially issued to Microsoft first party token brokers to enable single sign-on (SSO) across the applications used on those devices.</span></span> <span data-ttu-id="97ffa-108">[U aplikaciji Što je token](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)primarnog osvježavanja? na uređajima sa sustavom Windows 10 na uređajima sa sustavom Windows 10 pronaći ćemo pojedinosti o tome kako se izdaje, koristi i štiti PRT.</span><span class="sxs-lookup"><span data-stu-id="97ffa-108">[In What is a Primary Refresh Token?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token), we will provide details on how a PRT is issued, used, and protected on Windows 10 devices.</span></span>

<span data-ttu-id="97ffa-109">**WamDefaultSet: DA i AzureADPrt: DA** Ta polja označavaju je li korisnik uspješno provjerio autentičnost servisa Azure AD prilikom prijave na uređaj.</span><span class="sxs-lookup"><span data-stu-id="97ffa-109">**WamDefaultSet: YES and AzureADPrt: YES** These fields indicate whether the user has successfully authenticated to Azure AD when signing in to the device.</span></span> <span data-ttu-id="97ffa-110">Ako su vrijednosti **NO**, može biti potrebno:</span><span class="sxs-lookup"><span data-stu-id="97ffa-110">If the values are **NO**, it could be due:</span></span>

- <span data-ttu-id="97ffa-111">Loš ključ za pohranu u TPM-u povezanom s uređajem nakon registracije (provjerite KeySignTest dok je pokrenuta povišena razina).</span><span class="sxs-lookup"><span data-stu-id="97ffa-111">Bad storage key in the TPM associated with the device upon registration (check the KeySignTest while running elevated).</span></span>
- <span data-ttu-id="97ffa-112">Zamjenski ID za prijavu</span><span class="sxs-lookup"><span data-stu-id="97ffa-112">Alternate Login ID</span></span>
- <span data-ttu-id="97ffa-113">HTTP proxy nije pronađen</span><span class="sxs-lookup"><span data-stu-id="97ffa-113">HTTP Proxy not found</span></span>

<span data-ttu-id="97ffa-114">Otklanjanje poteškoća s uređajima pomoću naredbe dsregcmd – [stanje SSO-a](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)</span><span class="sxs-lookup"><span data-stu-id="97ffa-114">Troubleshoot devices using the dsregcmd command - [SSO state](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)</span></span>
