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
ms.openlocfilehash: c0d9ed14f83d3c7d47e1728d5ed9ca3a19412ad2
ms.sourcegitcommit: f74c9698a31634154ce58dda8b3145bb10685ace
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/23/2020
ms.locfileid: "48219847"
---
# <a name="blocking-or-unblocking-email-forwarding"></a><span data-ttu-id="162b1-102">Blokiranje ili deblokiranje prosljeđivanja e-pošte</span><span class="sxs-lookup"><span data-stu-id="162b1-102">Blocking or unblocking email forwarding</span></span>

<span data-ttu-id="162b1-103">Da biste omogućili ili onemogućili prosljeđivanje e-pošte za određeni poštanski sandučić, pročitajte članak [Konfiguriranje prosljeđivanja e-pošte](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).</span><span class="sxs-lookup"><span data-stu-id="162b1-103">To enable or disable email forwarding for a specific mailbox, see [Configure email forwarding](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).</span></span>

<span data-ttu-id="162b1-104">Na razini korisnika kontrola vanjskog prosljeđivanja obavlja se pomoću izlaznog pravilnika o suzbijanju neželjene pošte.</span><span class="sxs-lookup"><span data-stu-id="162b1-104">On the tenant level, control of External forwarding is done using the outbound anti-spam policy.</span></span> <span data-ttu-id="162b1-105">Ako je postavljena na Isključeno ili automatsko, možda blokira prosljeđivanje e-pošte pomoću pogreške "550 5.7.520 Access denied, vaša tvrtka ili ustanova ne dopušta pogrešku za vanjsko prosljeđivanje".</span><span class="sxs-lookup"><span data-stu-id="162b1-105">If it is set to Off or Automatic, it might block email forwarding with the “550 5.7.520 Access denied, Your organization does not allow external forwarding” error.</span></span> <span data-ttu-id="162b1-106">Nakon toga, ako je prosljeđivanje postavljeno na blokiranje, to je pogreška koju će korisnici vidjeti.</span><span class="sxs-lookup"><span data-stu-id="162b1-106">Subsequently, if forwarding was set to be blocked, that is the error your users will see.</span></span>

<span data-ttu-id="162b1-107">Ako je prosljeđivanje blokirano, provjerite je li pravilo konfigurirano tako da omogući vanjsko automatsko prosljeđivanje.</span><span class="sxs-lookup"><span data-stu-id="162b1-107">If forwarding is being blocked, please make sure the policy is configured to enable External Autoforward.</span></span> <span data-ttu-id="162b1-108">Pravilnik o izlaznom filtriranju neželjene pošte možete provjeriti iz centra za sigurnost i usklađenost ili pokretanjem naredbe Get-Hostedespamfilterpolicy | FL naziv, Autoforwardingmodu.</span><span class="sxs-lookup"><span data-stu-id="162b1-108">You can check the Outbound Spam Filter Policy from Security and Compliance Center or by running command Get-HostedOutboundSpamFilterPolicy | fl name,AutoForwardingMode.</span></span> <span data-ttu-id="162b1-109">Ako želite postaviti blokiranje automatskog prosljeđivanja, ta će vam naredba odmah reći stanje pravilnika.</span><span class="sxs-lookup"><span data-stu-id="162b1-109">If you want to set up Autoforward blocking, the same command will tell you the state of policy now.</span></span>

<span data-ttu-id="162b1-110">Imajte na glavi: preporučuje se da vanjsko automatsko prosljeđivanje bude onemogućeno na zadanom pravilniku o izlaznom filtriranju neželjene pošte i omogućite ga samo korisnicima kojima je potreban vanjski prijenos stvaranjem prilagođenog pravilnika za te korisnike.</span><span class="sxs-lookup"><span data-stu-id="162b1-110">Note: It is recommended to keep the External Autoforward disabled on your Default Outbound Spam Filter Policy and enable it only for the users who need external forwarding by creating a custom policy for those users.</span></span> <span data-ttu-id="162b1-111">Dodatne informacije možete pročitati u [konfiguriranju vanjskog prosljeđivanja e-pošte u sustavu Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).</span><span class="sxs-lookup"><span data-stu-id="162b1-111">You can read more in [Configuring external email forwarding in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).</span></span>