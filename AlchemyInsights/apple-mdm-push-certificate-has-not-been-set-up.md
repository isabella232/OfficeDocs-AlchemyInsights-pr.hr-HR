---
title: Certifikat za guranje u aplikaciji Apple MDM nije postavljen
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2634"
- "9000770"
ms.openlocfilehash: 5f95c9bee29db44a4153e0de0b8f6fb49b274920
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47716849"
---
# <a name="apple-mdm-push-certificate-has-not-been-set-up"></a><span data-ttu-id="14184-102">Certifikat za guranje u aplikaciji Apple MDM nije postavljen</span><span class="sxs-lookup"><span data-stu-id="14184-102">Apple MDM Push Certificate has not been set up</span></span>

<span data-ttu-id="14184-103">Potvrda dodatka Apple MDM (poznata i kao certifikat servisa Apple push notifikaciju (APN) nije konfigurirana za vašu pretplatu.</span><span class="sxs-lookup"><span data-stu-id="14184-103">An Apple MDM Push Certificate (also known as an Apple Push Notification Service (APNS) certificate) has not been configured for your subscription.</span></span> <span data-ttu-id="14184-104">Bez konfiguriranog certifikata za Apple MDM, ne možete upisati i upravljati uređajima sa sustavom iOS i Mac OS.</span><span class="sxs-lookup"><span data-stu-id="14184-104">Without an Apple MDM Push Certificate configured, you are unable to enroll and manage iOS and Mac OS devices.</span></span> <span data-ttu-id="14184-105">Kada dodate certifikat u Intune, korisnici mogu instalirati aplikaciju Portal tvrtke da bi upisali svoje iOS uređaje.</span><span class="sxs-lookup"><span data-stu-id="14184-105">After you add the certificate to Intune, users can install the Company Portal app to enroll their iOS devices.</span></span>

1. <span data-ttu-id="14184-106">Odaberite **"Slažem** se".</span><span class="sxs-lookup"><span data-stu-id="14184-106">Select **"I agree."**</span></span> <span data-ttu-id="14184-107">Da biste Microsoftu dopustili poslati podatke u Apple.</span><span class="sxs-lookup"><span data-stu-id="14184-107">to give Microsoft permission to send data to Apple.</span></span>

2. <span data-ttu-id="14184-108">Odaberite **Preuzmi CSR** da biste stvorili certifikat za potpisivanje Intune certifikatom koji je potreban za stvaranje dodatka Apple MDM.</span><span class="sxs-lookup"><span data-stu-id="14184-108">Select **Download your CSR** the Intune certificate signing request required to create an Apple MDM push certificate.</span></span> <span data-ttu-id="14184-109">Datoteka se koristi za zahtjev za certifikatom o pouzdanosti iz portala Appleov gumb za izdavanje certifikata.</span><span class="sxs-lookup"><span data-stu-id="14184-109">The file is used to request a trust relationship certificate from the Apple Push Certificates Portal.</span></span>

3. <span data-ttu-id="14184-110">Odaberite **Stvaranje certifikata za MDM** da biste prešli na portal Apple push certifikata.</span><span class="sxs-lookup"><span data-stu-id="14184-110">Select **Create your MDM push Certificate** to go to the Apple Push Certificates Portal.</span></span> <span data-ttu-id="14184-111">Prijavite se pomoću tvrtke Apple ID, a zatim odaberite **Stvori certifikat**.</span><span class="sxs-lookup"><span data-stu-id="14184-111">Sign in with your company Apple ID, and then select **Create a Certificate**.</span></span> <span data-ttu-id="14184-112">Odaberite **Odaberi datoteku**, dođite do datoteke zahtjeva za potpisivanje certifikata, a zatim odaberite **Prenesi**.</span><span class="sxs-lookup"><span data-stu-id="14184-112">Select **Choose File**, browse to the certificate signing request file, and then choose **Upload**.</span></span> <span data-ttu-id="14184-113">Na stranici za potvrdu odaberite **Preuzmi** da biste preuzeli datoteku certifikata (. Pem) i spremili datoteku lokalno.</span><span class="sxs-lookup"><span data-stu-id="14184-113">On the Confirmation page, choose **Download** to download the certificate (.pem) file, and save the file locally.</span></span>
 
<span data-ttu-id="14184-114">**Pažnja**: certifikat je povezan s Appleovim ID-om koji se koristi za stvaranje.</span><span class="sxs-lookup"><span data-stu-id="14184-114">**Note**: The certificate is associated with the Apple ID used to create it.</span></span> <span data-ttu-id="14184-115">Kao najbolja praksa koristite tvrtke Apple ID za zadatke upravljanja i provjerite nadzire li poštanski sandučić više osoba ili pomoću popisa za raspodjelu.</span><span class="sxs-lookup"><span data-stu-id="14184-115">As a best practice, use a company Apple ID for management tasks, and make sure the mailbox is monitored by more than one person or by using a distribution list.</span></span> <span data-ttu-id="14184-116">Nikad ne koristite osobni ID Apple.</span><span class="sxs-lookup"><span data-stu-id="14184-116">Never use a personal Apple ID.</span></span> <span data-ttu-id="14184-117">Koristite isti Apple ID da biste obnovili certifikat Apple push svakih 12 mjeseci.</span><span class="sxs-lookup"><span data-stu-id="14184-117">Use the same Apple ID to renew the Apple Push Certificate every 12 months.</span></span>
 
4. <span data-ttu-id="14184-118">Unesite Apple ID koji se koristi za stvaranje certifikata za slanje Apple MDM-a.</span><span class="sxs-lookup"><span data-stu-id="14184-118">Enter the Apple ID used to create your Apple MDM push certificate.</span></span> <span data-ttu-id="14184-119">Snimite ovaj ID kao podsjetnik kada morate obnoviti certifikat.</span><span class="sxs-lookup"><span data-stu-id="14184-119">Record this ID as a reminder for when you need to renew the certificate.</span></span>

5. <span data-ttu-id="14184-120">Idite na datoteku certifikata (. Pem), odaberite **Otvori**, a zatim odaberite **Prenesi**.</span><span class="sxs-lookup"><span data-stu-id="14184-120">Go to the certificate (.pem) file, choose **Open**, and then choose **Upload**.</span></span> <span data-ttu-id="14184-121">Uz certifikat push, Intune može upisati i upravljati uređajima sa sustavom Apple.</span><span class="sxs-lookup"><span data-stu-id="14184-121">With the push certificate, Intune can enroll and manage Apple devices.</span></span>