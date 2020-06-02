---
title: S / MIME u programu Outlook na webu
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 6bbbf8722dacb8b7d5191d57ce1055a48dcb4dd0
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511500"
---
# <a name="encrypt-email-messages-in-outlook"></a><span data-ttu-id="25186-102">Šifriranje poruka e-pošte u programu Outlook</span><span class="sxs-lookup"><span data-stu-id="25186-102">Encrypt email messages in Outlook</span></span>

<span data-ttu-id="25186-103">Microsoft 365 Šifriranje poruka izgrađen je na Microsoft Azure prava management (Azure RMS), koji je dio Azure Information Protection.</span><span class="sxs-lookup"><span data-stu-id="25186-103">Microsoft 365 Message Encryption is built on Microsoft Azure Rights Management (Azure RMS), which is part of Azure Information Protection.</span></span> <span data-ttu-id="25186-104">Ako vaša pretplata uključuje upravljanje pravima na Azure ili zaštitu informacija o platformi Azure, **ne morate poduzimati nikakve radnje da biste ručno omogućili ili aktivirali** uslugu upravljanja pravima.</span><span class="sxs-lookup"><span data-stu-id="25186-104">If your subscription includes Azure Rights Management or Azure Information Protection, **you do not need to take any actions to manually enable or activate** the Rights Management Service.</span></span>

<span data-ttu-id="25186-105">Na temelju povratnih informacija korisnika više nećemo omogućiti pravilima tijeka pošte sustava Exchange da automatski šifriraju odlaznu e-poštu koja sadrži određenu vrstu osjetljivih podataka na klijentu prema zadanim postavkama.</span><span class="sxs-lookup"><span data-stu-id="25186-105">Based on customer feedback, we will no longer be enabling Exchange mail flow rules to automatically encrypt outbound email containing certain type of sensitive information in your tenant by default.</span></span> <span data-ttu-id="25186-106">Umjesto toga, pružamo detaljne upute o tome kako to možete učiniti sami.</span><span class="sxs-lookup"><span data-stu-id="25186-106">Instead, we are providing detailed instructions on how you can do so yourselves.</span></span> <span data-ttu-id="25186-107">Dodatne pojedinosti o stvaranju pravila prijenosa za šifriranje osjetljivih informacija potražite u [ovom članku](https://aka.ms/OmeEtr).</span><span class="sxs-lookup"><span data-stu-id="25186-107">For additional details on how to create a transport rule to encrypt sensitive information, see [this article](https://aka.ms/OmeEtr).</span></span>

- <span data-ttu-id="25186-108">Ako koristite Outlook na webu (bivši **OWA):** Prilikom sastavljanja poruke e-pošte jednostavno kliknite **Zaštiti** u OWA.</span><span class="sxs-lookup"><span data-stu-id="25186-108">If using Outlook on the Web (formerly **OWA**): When composing an email message, simply click **Protect** in OWA.</span></span> <span data-ttu-id="25186-109">To će primijeniti dozvolu "Ne prosljeđujte".</span><span class="sxs-lookup"><span data-stu-id="25186-109">This will apply "Do not forward" permission.</span></span> <span data-ttu-id="25186-110">Kliknite **Promijeni dozvolu,** a zatim odaberite **Šifriraj** da biste šifrirali samo poruku.</span><span class="sxs-lookup"><span data-stu-id="25186-110">Click **Change permission** and choose **Encrypt** to only encrypt the message.</span></span>

- <span data-ttu-id="25186-111">Ako koristite **klijent programa Outlook**: Da biste poslali šifriranu poruku iz programa Outlook 2013 ili 2016 ili Outlook 2016 za Mac, odaberite **Dozvole za mogućnosti**, a zatim odaberite  >  **Permissions**željenu mogućnost zaštite.</span><span class="sxs-lookup"><span data-stu-id="25186-111">If using **Outlook client**: To send an encrypted message from Outlook 2013 or 2016, or Outlook 2016 for Mac, select **Options** > **Permissions**, then select the protection option you need.</span></span>

- <span data-ttu-id="25186-112">Da biste **automatski šifrirali svu e-poštu** poslanu određenim primateljima ili vanjskim partnerskim organizacijama, morate stvoriti pravilo prijenosa tijeka pošte u centru za administratore sustava Exchange.</span><span class="sxs-lookup"><span data-stu-id="25186-112">To **automatically encrypt all email** sent to certain recipients or external partner organizations, you need to create a mail flow transport rule in the Exchange Admin Center.</span></span> <span data-ttu-id="25186-113">Detaljne upute navedene su u [ovom članku podrške](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities).</span><span class="sxs-lookup"><span data-stu-id="25186-113">Detailed instructions are provided in [this support article](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities).</span></span>

