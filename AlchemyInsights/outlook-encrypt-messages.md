---
title: S/ MIME u programu Outlook na webu
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 7184ffd68f56639a8bcb87e9c6cab88388868103
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43764864"
---
# <a name="encrypt-email-messages-in-outlook"></a><span data-ttu-id="18a5d-102">Šifriranje poruka e-pošte u programu Outlook</span><span class="sxs-lookup"><span data-stu-id="18a5d-102">Encrypt email messages in Outlook</span></span>

<span data-ttu-id="18a5d-103">Šifriranje poruka sustava Microsoft 365 izgrađeno je na servisu Microsoft Azure Rights Management (Azure RMS), koje je dio zaštite podataka usluge Azure.</span><span class="sxs-lookup"><span data-stu-id="18a5d-103">Microsoft 365 Message Encryption is built on Microsoft Azure Rights Management (Azure RMS), which is part of Azure Information Protection.</span></span> <span data-ttu-id="18a5d-104">Ako vaša pretplata uključuje upravljanje pravima na Azure ili Azure Information Protection, **ne morate poduzimati nikakve radnje da biste ručno omogućili ili aktivirali** uslugu upravljanja pravima.</span><span class="sxs-lookup"><span data-stu-id="18a5d-104">If your subscription includes Azure Rights Management or Azure Information Protection, **you do not need to take any actions to manually enable or activate** the Rights Management Service.</span></span>

<span data-ttu-id="18a5d-105">Na temelju povratnih informacija korisnika više nećemo moći omogućiti pravila tijeka pošte sustava Exchange da automatski šifriraju izlaznu e-poštu koja sadrži određenu vrstu osjetljivih podataka u klijentu prema zadanim postavkama.</span><span class="sxs-lookup"><span data-stu-id="18a5d-105">Based on customer feedback, we will no longer be enabling Exchange mail flow rules to automatically encrypt outbound email containing certain type of sensitive information in your tenant by default.</span></span> <span data-ttu-id="18a5d-106">Umjesto toga, dajemo detaljne upute o tome kako to možete učiniti sami.</span><span class="sxs-lookup"><span data-stu-id="18a5d-106">Instead, we are providing detailed instructions on how you can do so yourselves.</span></span> <span data-ttu-id="18a5d-107">Dodatne pojedinosti o stvaranju pravila prijenosa za šifriranje osjetljivih podataka potražite [u ovom članku](https://aka.ms/OmeEtr).</span><span class="sxs-lookup"><span data-stu-id="18a5d-107">For additional details on how to create a transport rule to encrypt sensitive information, see [this article](https://aka.ms/OmeEtr).</span></span>

- <span data-ttu-id="18a5d-108">Ako koristite Outlook na webu (bivši **OWA):** Prilikom sastavljanja poruke e-pošte jednostavno kliknite **Zaštiti** u programu OWA.</span><span class="sxs-lookup"><span data-stu-id="18a5d-108">If using Outlook on the Web (formerly **OWA**): When composing an email message, simply click **Protect** in OWA.</span></span> <span data-ttu-id="18a5d-109">To će primijeniti dozvolu "Ne prosljeđuj".</span><span class="sxs-lookup"><span data-stu-id="18a5d-109">This will apply "Do not forward" permission.</span></span> <span data-ttu-id="18a5d-110">Kliknite **Promijeni dozvolu** i odaberite **Šifriraj** da biste šifrirali samo poruku.</span><span class="sxs-lookup"><span data-stu-id="18a5d-110">Click **Change permission** and choose **Encrypt** to only encrypt the message.</span></span>

- <span data-ttu-id="18a5d-111">Ako koristite **klijent programa Outlook**: Za slanje šifrirane poruke iz programa Outlook 2013 ili 2016 ili Outlook 2016 za Mac odaberite **Dozvole** > **mogućnosti**, a zatim odaberite željenu mogućnost zaštite.</span><span class="sxs-lookup"><span data-stu-id="18a5d-111">If using **Outlook client**: To send an encrypted message from Outlook 2013 or 2016, or Outlook 2016 for Mac, select **Options** > **Permissions**, then select the protection option you need.</span></span>

- <span data-ttu-id="18a5d-112">Da biste **automatski šifrirali svu e-poštu** poslanu određenim primateljima ili vanjskim partnerskim organizacijama, morate stvoriti pravilo prijenosa tijeka pošte u centru za administratore sustava Exchange.</span><span class="sxs-lookup"><span data-stu-id="18a5d-112">To **automatically encrypt all email** sent to certain recipients or external partner organizations, you need to create a mail flow transport rule in the Exchange Admin Center.</span></span> <span data-ttu-id="18a5d-113">Detaljne upute navedene su u [ovom članku podrške](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities).</span><span class="sxs-lookup"><span data-stu-id="18a5d-113">Detailed instructions are provided in [this support article](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities).</span></span>

