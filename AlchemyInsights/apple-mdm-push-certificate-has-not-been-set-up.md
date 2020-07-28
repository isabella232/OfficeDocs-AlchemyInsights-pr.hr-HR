---
title: Apple MDM push certifikat nije postavljen
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2634"
- "9000770"
ms.openlocfilehash: 5888eeb9b1dfde0b1ac5e7569f00d812e3d9d1bb
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 07/28/2020
ms.locfileid: "45438853"
---
# <a name="apple-mdm-push-certificate-has-not-been-set-up"></a><span data-ttu-id="ed5bc-102">Apple MDM push certifikat nije postavljen</span><span class="sxs-lookup"><span data-stu-id="ed5bc-102">Apple MDM Push Certificate has not been set up</span></span>

<span data-ttu-id="ed5bc-103">AppleM push certifikat (poznat i kao certifikat servisa za slanje push obavijesti tvrtke Apple) nije konfiguriran za vašu pretplatu.</span><span class="sxs-lookup"><span data-stu-id="ed5bc-103">An Apple MDM Push Certificate (also known as an Apple Push Notification Service (APNS) certificate) has not been configured for your subscription.</span></span> <span data-ttu-id="ed5bc-104">Bez konfiguriranog Apple MDM push certifikata ne možete prijaviti i upravljati uređajima sa sustavom iOS i Mac OS.</span><span class="sxs-lookup"><span data-stu-id="ed5bc-104">Without an Apple MDM Push Certificate configured, you are unable to enroll and manage iOS and Mac OS devices.</span></span> <span data-ttu-id="ed5bc-105">Nakon što dodate certifikat u Intune, korisnici mogu instalirati aplikaciju Portal tvrtke da bi prijavili svoje iOS uređaje.</span><span class="sxs-lookup"><span data-stu-id="ed5bc-105">After you add the certificate to Intune, users can install the Company Portal app to enroll their iOS devices.</span></span>

1. <span data-ttu-id="ed5bc-106">Odaberite **"Slažem se".**</span><span class="sxs-lookup"><span data-stu-id="ed5bc-106">Select **"I agree."**</span></span> <span data-ttu-id="ed5bc-107">da biste Microsoftu dali dozvolu za slanje podataka Appleu.</span><span class="sxs-lookup"><span data-stu-id="ed5bc-107">to give Microsoft permission to send data to Apple.</span></span>

2. <span data-ttu-id="ed5bc-108">Odaberite **Preuzmite CSR** zahtjev za potpisivanje intune certifikata potreban za izradu Apple MDM push certifikata.</span><span class="sxs-lookup"><span data-stu-id="ed5bc-108">Select **Download your CSR** the Intune certificate signing request required to create an Apple MDM push certificate.</span></span> <span data-ttu-id="ed5bc-109">Datoteka se koristi za traženje certifikata pouzdanog odnosa s Appleovog portala push certifikata.</span><span class="sxs-lookup"><span data-stu-id="ed5bc-109">The file is used to request a trust relationship certificate from the Apple Push Certificates Portal.</span></span>

3. <span data-ttu-id="ed5bc-110">Odaberite **Izradi MDM push certifikat** da biste otišli na Apple push certificates portal.</span><span class="sxs-lookup"><span data-stu-id="ed5bc-110">Select **Create your MDM push Certificate** to go to the Apple Push Certificates Portal.</span></span> <span data-ttu-id="ed5bc-111">Prijavite se pomoću Apple ID-a tvrtke, a zatim odaberite **Stvori certifikat**.</span><span class="sxs-lookup"><span data-stu-id="ed5bc-111">Sign in with your company Apple ID, and then select **Create a Certificate**.</span></span> <span data-ttu-id="ed5bc-112">Odaberite **Odaberi datoteku**, pronađite datoteku zahtjeva za potpisivanje certifikata, a zatim odaberite **Prijenos**.</span><span class="sxs-lookup"><span data-stu-id="ed5bc-112">Select **Choose File**, browse to the certificate signing request file, and then choose **Upload**.</span></span> <span data-ttu-id="ed5bc-113">Na stranici Potvrda odaberite **Preuzmi** da biste preuzeli datoteku certifikata (.pem) i spremite datoteku lokalno.</span><span class="sxs-lookup"><span data-stu-id="ed5bc-113">On the Confirmation page, choose **Download** to download the certificate (.pem) file, and save the file locally.</span></span>
 
<span data-ttu-id="ed5bc-114">**Napomena:** Certifikat je povezan s Apple ID-om koji se koristi za stvaranje.</span><span class="sxs-lookup"><span data-stu-id="ed5bc-114">**Note**: The certificate is associated with the Apple ID used to create it.</span></span> <span data-ttu-id="ed5bc-115">Kao najbolju praksu koristite tvrtku Apple ID za zadatke upravljanja i provjerite nadzire li poštanski sandučić više osoba ili pomoću popisa za distribuciju.</span><span class="sxs-lookup"><span data-stu-id="ed5bc-115">As a best practice, use a company Apple ID for management tasks, and make sure the mailbox is monitored by more than one person or by using a distribution list.</span></span> <span data-ttu-id="ed5bc-116">Nikada ne koristite osobni Apple ID.</span><span class="sxs-lookup"><span data-stu-id="ed5bc-116">Never use a personal Apple ID.</span></span> <span data-ttu-id="ed5bc-117">Koristite isti Apple ID za obnovu Apple push certifikata svakih 12 mjeseci.</span><span class="sxs-lookup"><span data-stu-id="ed5bc-117">Use the same Apple ID to renew the Apple Push Certificate every 12 months.</span></span>
 
4. <span data-ttu-id="ed5bc-118">Unesite Apple ID koji se koristi za izradu Apple MDM push certifikata.</span><span class="sxs-lookup"><span data-stu-id="ed5bc-118">Enter the Apple ID used to create your Apple MDM push certificate.</span></span> <span data-ttu-id="ed5bc-119">Zabilježite ovaj ID kao podsjetnik kada trebate obnoviti certifikat.</span><span class="sxs-lookup"><span data-stu-id="ed5bc-119">Record this ID as a reminder for when you need to renew the certificate.</span></span>

5. <span data-ttu-id="ed5bc-120">Idite na datoteku certifikata (.pem), odaberite **Otvori**, a zatim **prenesi**.</span><span class="sxs-lookup"><span data-stu-id="ed5bc-120">Go to the certificate (.pem) file, choose **Open**, and then choose **Upload**.</span></span> <span data-ttu-id="ed5bc-121">Pomoću push certifikata Intune može upisati Apple uređaje i upravljati njima.</span><span class="sxs-lookup"><span data-stu-id="ed5bc-121">With the push certificate, Intune can enroll and manage Apple devices.</span></span>