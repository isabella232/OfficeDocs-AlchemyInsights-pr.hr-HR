---
title: Otklanjanje poteškoća s Neometanjem jedinstvene prijave (SSO) za lokalno
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/12/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9370"
- "9004357"
ms.openlocfilehash: a8d14b12bfb3b02da0468eee70af26344465a2a2
ms.sourcegitcommit: 3fb39a080cc8680d960b8468ac9355389a3e2df4
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50816093"
---
# <a name="troubleshoot-seamless-single-sign-on-sso-for-on-premises"></a><span data-ttu-id="0d250-102">Otklanjanje poteškoća s Neometanjem jedinstvene prijave (SSO) za lokalno</span><span class="sxs-lookup"><span data-stu-id="0d250-102">Troubleshoot Seamless Single Sign-on (SSO) for on-premises</span></span>

<span data-ttu-id="0d250-103">Da biste riješili bešavne probleme s jedinstvenim prijavom (SSO), učinite sljedeće:</span><span class="sxs-lookup"><span data-stu-id="0d250-103">To resolve Seamless Single Sign-on (SSO) issues, perform the following steps:</span></span>

<span data-ttu-id="0d250-104">**Kako mogu prijeći na ključ za dešifriranje Kerberos za računalni račun AZUREADSSO?**</span><span class="sxs-lookup"><span data-stu-id="0d250-104">**How can I roll over the Kerberos decryption key of the AZUREADSSO computer account?**</span></span>

<span data-ttu-id="0d250-105">Preporučujemo da tijekom svakog 30 dana zagledate ključ za dešifriranje Kerberos.</span><span class="sxs-lookup"><span data-stu-id="0d250-105">We highly recommend that you roll over the Kerberos decryption key at least every 30 days.</span></span> <span data-ttu-id="0d250-106">Da biste to učinili ručno, pročitajte članak [kako okrenuti tipke za dešifriranje Kerberos](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq#).</span><span class="sxs-lookup"><span data-stu-id="0d250-106">To do this manually, see [How to roll over Kerberos decryption keys](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq#).</span></span>

<span data-ttu-id="0d250-107">**Konfiguriranje bešavnih SSO-a**</span><span class="sxs-lookup"><span data-stu-id="0d250-107">**Configure Seamless SSO**</span></span>

<span data-ttu-id="0d250-108">Da biste implementirali bešavne SSO, slijedite korake u programu [Azure Active Directory neprekinutu jedinstvenu prijavu: Quickstart](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start#step-5-roll-over-keys).</span><span class="sxs-lookup"><span data-stu-id="0d250-108">To deploy Seamless SSO, follow the steps in [Azure Active Directory Seamless Single Sign-On: Quickstart](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start#step-5-roll-over-keys).</span></span>

<span data-ttu-id="0d250-109">**Savjetodavni**</span><span class="sxs-lookup"><span data-stu-id="0d250-109">**Advisory**</span></span>

- <span data-ttu-id="0d250-110">[Neprimjetna jedinstvena prijava u servisu Azure Active Directory: najčešća pitanja](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq) u ovom članku obraćamo se često postavljanim pitanjima o programu Azure Active Directory bez neprekinutih pojedinačnih Sign-On (besprijekoran SSO).</span><span class="sxs-lookup"><span data-stu-id="0d250-110">[Azure Active Directory Seamless Single Sign-On: Frequently asked questions](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq) - In this article, we address frequently asked questions about Azure Active Directory Seamless Single Sign-On (Seamless SSO).</span></span> <span data-ttu-id="0d250-111">Nastavite se ponovno prijaviti za novi sadržaj.</span><span class="sxs-lookup"><span data-stu-id="0d250-111">Keep checking back for new content.</span></span>
- <span data-ttu-id="0d250-112">[Microsoft Q&A](https://docs.microsoft.com/answers/topics/azure-ad-single-sign-on.html) -ovaj članak sadrži informacije o tome kako izvršiti zahtjeve za značajku ili postavljati tehnička pitanja o BEŠAVNOM SSO-u.</span><span class="sxs-lookup"><span data-stu-id="0d250-112">[Microsoft Q&A](https://docs.microsoft.com/answers/topics/azure-ad-single-sign-on.html) - This article provides information on how to make feature requests or ask technical questions about Seamless SSO.</span></span>

<span data-ttu-id="0d250-113">**Otklanjanje poteškoća s**</span><span class="sxs-lookup"><span data-stu-id="0d250-113">**Troubleshoot**</span></span>

<span data-ttu-id="0d250-114">[Otklanjanje poteškoća s jedinstvenim prijavom u servisu Azure Active Directory](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso) -ovaj članak omogućuje vam da pronađete otklanjanje poteškoća s uobičajenim problemima u vezi sa jedinstvenim neometanima u programu Azure Active Directory (Azure AD) Sign-On (bešavni SSO).</span><span class="sxs-lookup"><span data-stu-id="0d250-114">[Troubleshoot Azure Active Directory Seamless Single Sign-On](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso) - This article helps you find troubleshooting information about common problems regarding Azure Active Directory (Azure AD) Seamless Single Sign-On (Seamless SSO).</span></span>







