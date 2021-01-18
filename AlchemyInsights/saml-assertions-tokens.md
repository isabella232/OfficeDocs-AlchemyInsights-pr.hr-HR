---
title: SAML tvrdnje (tokeni)
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004341"
- "7753"
ms.openlocfilehash: 557e23da09df3ab066c2ad7c0352f5fd904b5490
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 01/18/2021
ms.locfileid: "49884861"
---
# <a name="saml-assertions-tokens"></a><span data-ttu-id="70e55-102">SAML tvrdnje (tokeni)</span><span class="sxs-lookup"><span data-stu-id="70e55-102">SAML Assertions (Tokens)</span></span>

1. <span data-ttu-id="70e55-103">Tokeni za sigurnosne tvrdnje Markup Language (SAML) XML su prikazi potraživanja.</span><span class="sxs-lookup"><span data-stu-id="70e55-103">Security Assertions Markup Language (SAML) tokens are XML representations of claims.</span></span> <span data-ttu-id="70e55-104">Po zadanom, SAML tokeni Windows Communication Foundation (WCF) koristi se u vanjskim sigurnosnim scenarijima izdane su tokeni.</span><span class="sxs-lookup"><span data-stu-id="70e55-104">By default, SAML tokens Windows Communication Foundation (WCF) uses in federated security scenarios are issued tokens.</span></span> <span data-ttu-id="70e55-105">Dodatne informacije potražite u članku [tokeni i tvrdnje o saml-](https://docs.microsoft.com/dotnet/framework/wcf/feature-details/saml-tokens-and-claims)u.</span><span class="sxs-lookup"><span data-stu-id="70e55-105">For more information, see [SAML Tokens and Claims](https://docs.microsoft.com/dotnet/framework/wcf/feature-details/saml-tokens-and-claims).</span></span>
2. <span data-ttu-id="70e55-106">Microsoftova platforma identiteta emitira nekoliko vrsta sigurnosnih tokena u obradi svakog tijeka provjere autentičnosti.</span><span class="sxs-lookup"><span data-stu-id="70e55-106">The Microsoft identity platform emits several types of security tokens in the processing of each authentication flow.</span></span> <span data-ttu-id="70e55-107">[Referenca zahtjeva za saml token](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens) opisuje oblikovanje, sigurnosne karakteristike i sadržaj žetona saml 2,0.</span><span class="sxs-lookup"><span data-stu-id="70e55-107">[SAML token claims reference](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens) describes the format, security characteristics, and contents of SAML 2.0 tokens.</span></span>
3. <span data-ttu-id="70e55-108">Slijedite upute u [konfiguracibilan token vijek u programu Microsoft Identity Platform](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes) da biste razumjeli kako konfigurisati životni vijek tokena.</span><span class="sxs-lookup"><span data-stu-id="70e55-108">Follow the guidance in [Configurable token lifetimes in Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes) to understand how to configure token lifetimes.</span></span>
4. <span data-ttu-id="70e55-109">Slijedite korake opisane u [ovom članku](https://docs.microsoft.com/azure/active-directory/manage-apps/howto-saml-token-encryption) da biste shvatili kako konfigurirati enkripciju tokena za Azure ad saml.</span><span class="sxs-lookup"><span data-stu-id="70e55-109">Follow the steps outlined in [this article](https://docs.microsoft.com/azure/active-directory/manage-apps/howto-saml-token-encryption) to understand how to configure Azure AD SAML token encryption.</span></span>
5. <span data-ttu-id="70e55-110">U servisu Azure AD možete postaviti mogućnosti potpisivanja certifikata i algoritam potpisivanja certifikata.</span><span class="sxs-lookup"><span data-stu-id="70e55-110">In Azure AD, you can set up certificate signing options and the certificate signing algorithm.</span></span> <span data-ttu-id="70e55-111">Dodatne informacije potražite u članku dodatne [mogućnosti potpisivanja certifikata u Tokanu SAML-a za aplikacije Gallery u servisu Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).</span><span class="sxs-lookup"><span data-stu-id="70e55-111">For more information, see [Advanced certificate signing options in the SAML token for gallery apps in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).</span></span>
