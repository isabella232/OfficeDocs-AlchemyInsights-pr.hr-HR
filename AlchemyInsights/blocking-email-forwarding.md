---
title: 726 blokiranje prosljeđivanja e-pošte
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "726"
- "1200004"
ms.assetid: 8865c68e-7e8a-4135-a254-d7f69f1ded30
ms.openlocfilehash: 610013c4f46e999f1a8715aea14dd557ed8b0e2a
ms.sourcegitcommit: 88f24bb6ced16842de165af416e3f21feae13063
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 10/15/2020
ms.locfileid: "48478315"
---
# <a name="blocking-or-unblocking-email-forwarding"></a><span data-ttu-id="9d0b6-102">Blokiranje ili deblokiranje prosljeđivanja e-pošte</span><span class="sxs-lookup"><span data-stu-id="9d0b6-102">Blocking or unblocking email forwarding</span></span>

<span data-ttu-id="9d0b6-103">Da biste omogućili ili onemogućili prosljeđivanje e-pošte za određeni poštanski sandučić, pročitajte članak [Konfiguriranje prosljeđivanja e-pošte](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).</span><span class="sxs-lookup"><span data-stu-id="9d0b6-103">To enable or disable email forwarding for a specific mailbox, see [Configure email forwarding](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).</span></span>

<span data-ttu-id="9d0b6-104">Na razini korisnika kontrola vanjskog prosljeđivanja obavlja se pomoću izlaznog pravilnika o neželjenoj pošti.</span><span class="sxs-lookup"><span data-stu-id="9d0b6-104">On the tenant level, control of external forwarding is done using the outbound spam policy.</span></span> <span data-ttu-id="9d0b6-105">Pravilnik o izlaznom filtriranju neželjene pošte možete provjeriti u centru za sigurnost i usklađenost [ovdje](https://protection.office.com/antispam) ili pomoću [naredbe Dohvati-Hostedespamfilterpolicy](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy).</span><span class="sxs-lookup"><span data-stu-id="9d0b6-105">You can check the outbound spam filter policy from Security and Compliance Center [here](https://protection.office.com/antispam) or by using the [Get-HostedOutboundSpamFilterPolicy command](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy).</span></span>

<span data-ttu-id="9d0b6-106">Ako vam se prikaže sljedeća pogreška: **"550 5.7.520 je odbijen pristup, vaša tvrtka ili ustanova ne dopušta vanjsko prosljeđivanje"**, provjerite je li pravilo konfigurirano tako da omogući vanjsko automatsko prosljeđivanje.</span><span class="sxs-lookup"><span data-stu-id="9d0b6-106">If you are getting the following error: **“550 5.7.520 Access denied, Your organization does not allow external forwarding”**, please make sure the policy is configured to enable External Auto-forward.</span></span>

<span data-ttu-id="9d0b6-107">**Upozorenje:** Preporučuje se da vanjsko automatsko prosljeđivanje bude onemogućeno na zadanom pravilniku o izlaznom filtriranju neželjene pošte i omogućite ga samo korisnicima kojima je potreban vanjski prijenos stvaranjem prilagođenog pravilnika za te korisnike.</span><span class="sxs-lookup"><span data-stu-id="9d0b6-107">**Note:** It is recommended to keep the External Autoforward disabled on your default outbound spam filter policy and enable it only for the users who need external forwarding by creating a custom policy for those users.</span></span> <span data-ttu-id="9d0b6-108">Dodatne informacije možete pročitati u [konfiguriranju vanjskog prosljeđivanja e-pošte u sustavu Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).</span><span class="sxs-lookup"><span data-stu-id="9d0b6-108">You can read more in [Configuring external email forwarding in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).</span></span>