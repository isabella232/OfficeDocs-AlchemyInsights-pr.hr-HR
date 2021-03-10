---
title: Otklanjanje poteškoća sa potpisom SAML certifikata
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9406"
- "9004341"
ms.openlocfilehash: 3bc8b2e751395b8a099fb5079ad40c5c93222e0e
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/08/2021
ms.locfileid: "50692652"
---
# <a name="troubleshoot-saml-signing-certificate-issues"></a><span data-ttu-id="f50b1-102">Otklanjanje poteškoća sa potpisom SAML certifikata</span><span class="sxs-lookup"><span data-stu-id="f50b1-102">Troubleshoot SAML Signing certificate issues</span></span>

<span data-ttu-id="f50b1-103">Da biste riješili problem sa potpisom SAML certifikata, izvedite sljedeće preporučene korake:</span><span class="sxs-lookup"><span data-stu-id="f50b1-103">To resolve SAML Signing certificate issue, perform the following recommended steps:</span></span>

1. <span data-ttu-id="f50b1-104">Kada dodate korporacijsku aplikaciju koja podržava SSO, Azure će generirati certifikat koji se naziva [certifikatom saml za potpisivanje](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#auto-generated-certificate-for-gallery-and-non-gallery-applications).</span><span class="sxs-lookup"><span data-stu-id="f50b1-104">When you add an enterprise application which supports SSO, Azure will generate a certificate which is called the [SAML Signing certificate](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#auto-generated-certificate-for-gallery-and-non-gallery-applications).</span></span> <span data-ttu-id="f50b1-105">Ovaj certifikat ima Datum isteka od 3 godine.</span><span class="sxs-lookup"><span data-stu-id="f50b1-105">This certificate has an expiration date of 3 years.</span></span> <span data-ttu-id="f50b1-106">Da biste promijenili datum isteka certifikata, pročitajte članak [Prilagodba datuma isteka za certifikat Federacije i njegovo pretvaranje u novi certifikat](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#customize-the-expiration-date-for-your-federation-certificate-and-roll-it-over-to-a-new-certificate).</span><span class="sxs-lookup"><span data-stu-id="f50b1-106">To change the expiration date of your certificate, see [Customize the expiration date for your federation certificate and roll it over to a new certificate](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#customize-the-expiration-date-for-your-federation-certificate-and-roll-it-over-to-a-new-certificate).</span></span>
2. <span data-ttu-id="f50b1-107">Azure će ovaj certifikat koristiti za potpisivanje tokena za SAML koje zatraži aplikacija i poslat će ga u aplikaciju za uspješan SSO.</span><span class="sxs-lookup"><span data-stu-id="f50b1-107">Azure will use this certificate to sign the SAML tokens requested by the application and send it over to the application for a successful SSO.</span></span> <span data-ttu-id="f50b1-108">Da biste to dovršili, Preuzmite certifikat s portala Azure i poљaljite ga dobavljaču aplikacije da biste dovršili postupak SSO.</span><span class="sxs-lookup"><span data-stu-id="f50b1-108">In order for this to complete, download the certificate from the Azure portal and send it to the application vendor to complete the SSO process.</span></span>

<span data-ttu-id="f50b1-109">Nakon završetka postupka, aplikacija će potvrditi taj certifikat i sve tokene za SAML koje je potpisao taj certifikat.</span><span class="sxs-lookup"><span data-stu-id="f50b1-109">After this process completes your application will trust this certificate and all the SAML tokens signed by this certificate will be accepted by the application.</span></span>

3. <span data-ttu-id="f50b1-110">Ako ovaj certifikat istekne, stvorite novi certifikat, ažurirajte ga proizvođaču aplikacija, a zatim ga učinite aktivnim na stranici Azure.</span><span class="sxs-lookup"><span data-stu-id="f50b1-110">If this certificate expires, create a new certificate, update it to the application vendor and then make it active on the Azure side.</span></span> <span data-ttu-id="f50b1-111">Dodatne informacije potražite u članku [obnavljanje certifikata koji će uskoro isteći](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#renew-a-certificate-that-will-soon-expire).</span><span class="sxs-lookup"><span data-stu-id="f50b1-111">For more information, see [Renew a certificate that will soon expire](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#renew-a-certificate-that-will-soon-expire).</span></span>

> [!NOTE]
> <span data-ttu-id="f50b1-112">Ako certifikat istekne, korisnik neće biti blokiran.</span><span class="sxs-lookup"><span data-stu-id="f50b1-112">If the certificate expires, the user will not be blocked.</span></span>

4. <span data-ttu-id="f50b1-113">[Dodajte adresu e-pošte](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#add-email-notification-addresses-for-certificate-expiration) da bi se obavijesti primljene prije isteka tekućeg certifikata.</span><span class="sxs-lookup"><span data-stu-id="f50b1-113">[Add an email address for notifications](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#add-email-notification-addresses-for-certificate-expiration) to be received before the current certificate expires.</span></span>

> [!NOTE]
> <span data-ttu-id="f50b1-114">Korak-4 je neobavezan jedan.</span><span class="sxs-lookup"><span data-stu-id="f50b1-114">Step-4 is an optional one.</span></span>

5. <span data-ttu-id="f50b1-115">Promjena mogućnosti potpisivanja certifikata za SAML i algoritam potpisivanja certifikata.</span><span class="sxs-lookup"><span data-stu-id="f50b1-115">Change an application's SAML certificate signing options and the certificate signing algorithm.</span></span> <span data-ttu-id="f50b1-116">Dodatne informacije potražite u članku [Promjena mogućnosti potpisivanja certifikata i algoritma potpisivanja](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).</span><span class="sxs-lookup"><span data-stu-id="f50b1-116">For more information, see [Change certificate signing options and signing algorithm](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).</span></span>

