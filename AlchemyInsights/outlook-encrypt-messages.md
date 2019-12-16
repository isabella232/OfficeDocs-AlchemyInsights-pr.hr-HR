---
title: S/MIME u programu Outlook na webu
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 33e94eac6a2982b8036e13d17bf60015f244f2cb
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 12/15/2019
ms.locfileid: "40053217"
---
# <a name="encrypt-email-messages-in-outlook"></a><span data-ttu-id="4325b-102">Šifriranje poruka e-pošte u programu Outlook</span><span class="sxs-lookup"><span data-stu-id="4325b-102">Encrypt email messages in Outlook</span></span>

<span data-ttu-id="4325b-103">Office 365 šifriranje poruka izgrađeno je na servisu Microsoft Azure Rights Management (Azure RMS), koja je dio usluge Azure Information Protection.</span><span class="sxs-lookup"><span data-stu-id="4325b-103">Office 365 Message Encryption is built on Microsoft Azure Rights Management (Azure RMS), which is part of Azure Information Protection.</span></span> <span data-ttu-id="4325b-104">Ako vaša pretplata uključuje upravljanje pravima na Azure ili zaštitu informacija za Azure, **ne morate poduzeti nikakve radnje kako biste ručno omogućili ili aktivirali** uslugu upravljanja pravima.</span><span class="sxs-lookup"><span data-stu-id="4325b-104">If your subscription includes Azure Rights Management or Azure Information Protection, **you do not need to take any actions to manually enable or activate** the Rights Management Service.</span></span>

<span data-ttu-id="4325b-105">Na temelju povratnih informacija kupaca više nećemo omogućiti Exchange pravila tijeka pošte za automatsko šifriranje izlazne e-pošte koja sadrži određenu vrstu osjetljivih podataka u vašem klijentu po zadanim postavkama.</span><span class="sxs-lookup"><span data-stu-id="4325b-105">Based on customer feedback, we will no longer be enabling Exchange mail flow rules to automatically encrypt outbound email containing certain type of sensitive information in your tenant by default.</span></span> <span data-ttu-id="4325b-106">Umjesto toga, pružamo detaljne upute o tome kako to možete učiniti sami.</span><span class="sxs-lookup"><span data-stu-id="4325b-106">Instead, we are providing detailed instructions on how you can do so yourselves.</span></span> <span data-ttu-id="4325b-107">Dodatne pojedinosti o stvaranju pravila prijevoza za šifriranje osjetljivih podataka potražite u [ovom članku](https://aka.ms/OmeEtr).</span><span class="sxs-lookup"><span data-stu-id="4325b-107">For additional details on how to create a transport rule to encrypt sensitive information, see [this article](https://aka.ms/OmeEtr).</span></span>

- <span data-ttu-id="4325b-108">Ako koristite Outlook na webu (nekadašnji **OWA**): prilikom sastavljanja poruke e-pošte, jednostavno kliknite **Zaštitite** u OWI.</span><span class="sxs-lookup"><span data-stu-id="4325b-108">If using Outlook on the Web (formerly **OWA**): When composing an email message, simply click **Protect** in OWA.</span></span> <span data-ttu-id="4325b-109">To će primijeniti dopuštenje "ne prosljeđivati".</span><span class="sxs-lookup"><span data-stu-id="4325b-109">This will apply "Do not forward" permission.</span></span> <span data-ttu-id="4325b-110">Kliknite **Promijeni dozvolu** i odaberite **Šifriraj** da biste šifrirali poruku.</span><span class="sxs-lookup"><span data-stu-id="4325b-110">Click **Change permission** and choose **Encrypt** to only encrypt the message.</span></span>

- <span data-ttu-id="4325b-111">Ako koristite **Outlook Client**: za slanje šifrirane poruke iz programa Outlook 2013 ili 2016 ili Outlook 2016 za Mac, odaberite **opcije** > **dozvole**, a zatim odaberite mogućnost zaštite koja vam je potrebna.</span><span class="sxs-lookup"><span data-stu-id="4325b-111">If using **Outlook client**: To send an encrypted message from Outlook 2013 or 2016, or Outlook 2016 for Mac, select **Options** > **Permissions**, then select the protection option you need.</span></span>

- <span data-ttu-id="4325b-112">Da biste **automatski šifrirali svu e-poštu** poslanu određenim primateljima ili vanjskim partnerskim organizacijama, morate stvoriti pravilo transporta prijenosa pošte u centru za administraciju sustava Exchange.</span><span class="sxs-lookup"><span data-stu-id="4325b-112">To **automatically encrypt all email** sent to certain recipients or external partner organizations, you need to create a mail flow transport rule in the Exchange Admin Center.</span></span> <span data-ttu-id="4325b-113">Detaljne upute navedene su u [ovom članku podrške](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities).</span><span class="sxs-lookup"><span data-stu-id="4325b-113">Detailed instructions are provided in [this support article](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities).</span></span>

