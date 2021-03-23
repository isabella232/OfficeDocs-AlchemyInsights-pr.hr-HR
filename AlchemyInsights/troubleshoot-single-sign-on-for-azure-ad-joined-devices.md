---
title: Otklanjanje poteškoća s jednom prijavom za uređaje koji se spajaju na Azure AD
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003246"
- "9327"
ms.openlocfilehash: d11c24719eb2db9e9fd87c158c80cec5cb75b946
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035105"
---
# <a name="troubleshoot-single-sign-on-for-azure-ad-joined-devices"></a><span data-ttu-id="be186-102">Otklanjanje poteškoća s jednom prijavom za uređaje koji se spajaju na Azure AD</span><span class="sxs-lookup"><span data-stu-id="be186-102">Troubleshoot Single-sign on for Azure AD Joined Devices</span></span>

<span data-ttu-id="be186-103">Ako imate lokalno okruženje servisa Active Directory (AD) i želite se uključiti u svoju oglasnu domenu u sustavu Azure AD, to možete postići pomoću hibridnih Azure AD Join.</span><span class="sxs-lookup"><span data-stu-id="be186-103">If you have an on-premises Active Directory (AD) environment and you want to join your AD domain-joined computers to Azure AD, you can accomplish this by doing hybrid Azure AD join.</span></span> <span data-ttu-id="be186-104">[Kako: planirati svoj hibridni Azure Active Directory implementacija](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) servisa nudi vam odgovarajuće korake za implementaciju hibridnog Azure ad Join u vašem okruženju.</span><span class="sxs-lookup"><span data-stu-id="be186-104">[How To: Plan your hybrid Azure Active Directory join implementation](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) provides you with the related steps to implement a hybrid Azure AD join in your environment.</span></span>

<span data-ttu-id="be186-105">Dodatne informacije potražite u članku [Konfiguriranje dodatka Azure ad pridruženi uređaji za lokalne Single-Sign na servisu Windows Hello za tvrtke](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base).</span><span class="sxs-lookup"><span data-stu-id="be186-105">For more information, see [Configure Azure AD joined devices for On-premises Single-Sign On using Windows Hello for Business](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base).</span></span>

<span data-ttu-id="be186-106">**Problemi s primarnim Osvježavanjem (PRT)**</span><span class="sxs-lookup"><span data-stu-id="be186-106">**Primary Refresh Token (PRT) issues**</span></span>

<span data-ttu-id="be186-107">Primarni token za osvježavanje (PRT) ključan je artefakt za provjeru autentičnosti Azure AD u sustavima Windows 10, Windows Server 2016 i novije verzije, iOS i android uređaji.</span><span class="sxs-lookup"><span data-stu-id="be186-107">A Primary Refresh Token (PRT) is a key artifact of Azure AD authentication on Windows 10, Windows Server 2016 and later versions, iOS, and Android devices.</span></span> <span data-ttu-id="be186-108">To je web-token za JSON (JWT) koji se posebno izdaje Microsoftovoj prvoj stranci token za tokene da bi omogućio jedinstvenu prijavu (SSO) u svim aplikacijama koje se koriste na tim uređajima.</span><span class="sxs-lookup"><span data-stu-id="be186-108">It is a JSON Web Token (JWT) specially issued to Microsoft first party token brokers to enable single sign-on (SSO) across the applications used on those devices.</span></span> <span data-ttu-id="be186-109">Pojedinosti o tome kako se PRT izdaje, koristi i štiti na uređajima sa sustavom Windows 10 potražite [u članku što je primarni token osvježavanja?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).</span><span class="sxs-lookup"><span data-stu-id="be186-109">For details on how a PRT is issued, used, and protected on Windows 10 devices, see [What is a Primary Refresh Token?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).</span></span>

<span data-ttu-id="be186-110">**WamDefaultSet: da i AzureADPrt: da**</span><span class="sxs-lookup"><span data-stu-id="be186-110">**WamDefaultSet: YES and AzureADPrt: YES**</span></span>

<span data-ttu-id="be186-111">Ova polja ukazuju na to je li korisnik uspješno ovjerio Azure AD prilikom prijave na uređaj.</span><span class="sxs-lookup"><span data-stu-id="be186-111">These fields indicate whether the user has successfully authenticated to Azure AD when signing in to the device.</span></span> <span data-ttu-id="be186-112">Ako vrijednosti **nisu, možda** je posljedica:</span><span class="sxs-lookup"><span data-stu-id="be186-112">If the values are **NO**, it could be due to:</span></span>

- <span data-ttu-id="be186-113">Loš ključ za pohranu u TPM-u povezan s uređajem pri registriranju (provjera tabulatora prilikom izvođenja povišenog)</span><span class="sxs-lookup"><span data-stu-id="be186-113">Bad storage key in the TPM associated with the device upon registration (check the KeySignTest while running elevated)</span></span>
- <span data-ttu-id="be186-114">Zamjenski ID za prijavu</span><span class="sxs-lookup"><span data-stu-id="be186-114">Alternate Login ID</span></span>
- <span data-ttu-id="be186-115">HTTP proxy nije pronađen</span><span class="sxs-lookup"><span data-stu-id="be186-115">HTTP Proxy not found</span></span>

<span data-ttu-id="be186-116">Otklanjanje poteškoća s uređajima pomoću naredbe dsregcmd potražite u članku [SSO State](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).</span><span class="sxs-lookup"><span data-stu-id="be186-116">To troubleshoot devices using the dsregcmd command, see [SSO state](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).</span></span>
