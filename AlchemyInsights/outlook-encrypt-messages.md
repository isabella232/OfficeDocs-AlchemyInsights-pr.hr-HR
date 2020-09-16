---
title: S/MIME u programu Outlook na webu
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 052149d1f11387246bc1ff24ba48c45b944ba52c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47772254"
---
# <a name="encrypt-email-messages-in-outlook"></a><span data-ttu-id="6afdb-102">Šifriranje poruka e-pošte u programu Outlook</span><span class="sxs-lookup"><span data-stu-id="6afdb-102">Encrypt email messages in Outlook</span></span>

<span data-ttu-id="6afdb-103">Šifriranje poruka u sustavu Microsoft 365 izgrađeno je na servisu Microsoft Azure Rights Management (Azure RMS), koji je dio zaštite informacija za Azure.</span><span class="sxs-lookup"><span data-stu-id="6afdb-103">Microsoft 365 Message Encryption is built on Microsoft Azure Rights Management (Azure RMS), which is part of Azure Information Protection.</span></span> <span data-ttu-id="6afdb-104">Ako vaša pretplata obuhvaća upravljanje pravima na Azure i Azure, ne **morate poduzeti nikakve akcije da biste ručno omogućili ili aktivirali** servis za upravljanje pravima.</span><span class="sxs-lookup"><span data-stu-id="6afdb-104">If your subscription includes Azure Rights Management or Azure Information Protection, **you do not need to take any actions to manually enable or activate** the Rights Management Service.</span></span>

<span data-ttu-id="6afdb-105">Na temelju povratnih informacija o klijentu više neće biti omogućeno automatsko šifriranje odlaznih poruka e-pošte koja sadrži određene vrste osjetljivih podataka u zakupcu.</span><span class="sxs-lookup"><span data-stu-id="6afdb-105">Based on customer feedback, we will no longer be enabling Exchange mail flow rules to automatically encrypt outbound email containing certain type of sensitive information in your tenant by default.</span></span> <span data-ttu-id="6afdb-106">Umjesto toga dajemo detaljne upute o tome kako to sami možete učiniti.</span><span class="sxs-lookup"><span data-stu-id="6afdb-106">Instead, we are providing detailed instructions on how you can do so yourselves.</span></span> <span data-ttu-id="6afdb-107">Dodatne informacije o stvaranju pravila prijenosa radi šifriranja osjetljivih informacija potražite u [ovom članku](https://aka.ms/OmeEtr).</span><span class="sxs-lookup"><span data-stu-id="6afdb-107">For additional details on how to create a transport rule to encrypt sensitive information, see [this article](https://aka.ms/OmeEtr).</span></span>

- <span data-ttu-id="6afdb-108">Ako koristite Outlook na webu (bivši **OWA**): prilikom skladanja poruke e-pošte jednostavno kliknite **zaštiti** u aplikaciji OWA.</span><span class="sxs-lookup"><span data-stu-id="6afdb-108">If using Outlook on the Web (formerly **OWA**): When composing an email message, simply click **Protect** in OWA.</span></span> <span data-ttu-id="6afdb-109">Time će se primijeniti dozvola "Ne prosljeđuj".</span><span class="sxs-lookup"><span data-stu-id="6afdb-109">This will apply "Do not forward" permission.</span></span> <span data-ttu-id="6afdb-110">Kliknite **Promijeni dozvolu** , a zatim **Šifriraj** samo da biste šifrirali poruku.</span><span class="sxs-lookup"><span data-stu-id="6afdb-110">Click **Change permission** and choose **Encrypt** to only encrypt the message.</span></span>

- <span data-ttu-id="6afdb-111">Ako koristite **klijent programa Outlook**: da biste slali šifriranu poruku iz programa Outlook 2013 ili 2016 ili Outlook 2016 za Mac, odaberite **mogućnosti**  >  **dozvole**, a zatim odaberite mogućnost zaštite koja vam je potrebna.</span><span class="sxs-lookup"><span data-stu-id="6afdb-111">If using **Outlook client**: To send an encrypted message from Outlook 2013 or 2016, or Outlook 2016 for Mac, select **Options** > **Permissions**, then select the protection option you need.</span></span>

- <span data-ttu-id="6afdb-112">Da biste **automatski šifrirali sve poruke e-pošte** poslane određenim primateljima ili vanjskim partnerskim organizacijama, morate stvoriti pravilo prijenosa tijeka pošte u centru za administratore sustava Exchange.</span><span class="sxs-lookup"><span data-stu-id="6afdb-112">To **automatically encrypt all email** sent to certain recipients or external partner organizations, you need to create a mail flow transport rule in the Exchange Admin Center.</span></span> <span data-ttu-id="6afdb-113">Detaljne upute navedene su u [ovom članku podrške](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities).</span><span class="sxs-lookup"><span data-stu-id="6afdb-113">Detailed instructions are provided in [this support article](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities).</span></span>

