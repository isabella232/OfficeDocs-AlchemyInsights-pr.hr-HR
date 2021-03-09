---
title: Pogreška Proxy adrese prilikom stvaranja zajedničkog poštanskog sandučića
ms.author: pebaum
author: CrystalThomasMS
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ece4bcce-1053-4ed3-a194-9d0af8f73c6f
ms.custom:
- "19"
- "6"
ms.openlocfilehash: ab491e883ab294f08d0b5d2e686dc059b468d29f
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/09/2021
ms.locfileid: "50568282"
---
# <a name="proxy-address-error-while-creating-a-mailbox-or-other-email-enabled-object"></a><span data-ttu-id="bbd2f-102">Pogreška Proxy adrese prilikom stvaranja poštanskog sandučića ili drugog objekta koji je omogućen za e-poštu</span><span class="sxs-lookup"><span data-stu-id="bbd2f-102">Proxy address error while creating a mailbox or other email enabled object</span></span>

<span data-ttu-id="bbd2f-103">Ako ste pokušali stvoriti objekt omogućen za e-poštu (poštanski sandučić, zajednički poštanski sandučić itd.) i primili pogrešku "proxy adresa" SMTP:alias@domain.com "već se koristi...", adresa e-pošte koju ste odabrali već je uzeo neki drugi objekt omogućen za e-poštu u vašoj tvrtki ili ustanovi.</span><span class="sxs-lookup"><span data-stu-id="bbd2f-103">If you tried to create an email-enabled object (mailbox, shared mailbox etc.) and received the error "The proxy address "SMTP:alias@domain.com" is already being used…", the email address you chose is already taken by another email-enabled object in your organization.</span></span>
  
<span data-ttu-id="bbd2f-104">Morate pronaći korisnika, grupu, zajednički poštanski sandučić ili javnu mapu koja sadrži ovu adresu e-pošte i izbrisati je ili promijeniti adresu e-pošte.</span><span class="sxs-lookup"><span data-stu-id="bbd2f-104">You need to find the user, group, shared mailbox or public folder that has this email address and delete it or change its email address.</span></span> <span data-ttu-id="bbd2f-105">Zatim možete stvoriti novi objekt omogućen za e-poštu s oslobođenom adresom e-pošte.</span><span class="sxs-lookup"><span data-stu-id="bbd2f-105">Then you can create a new email-enabled object with the freed email address.</span></span> <span data-ttu-id="bbd2f-106">Pronađite ga pomoću pretraživanja na početnoj stranici.</span><span class="sxs-lookup"><span data-stu-id="bbd2f-106">Use Search on the Home page to find it.</span></span> <span data-ttu-id="bbd2f-107">Da biste ga potražili, možete koristiti i sljedeću naredbu sustava Exchange Online PowerShell:</span><span class="sxs-lookup"><span data-stu-id="bbd2f-107">You can also use the following Exchange Online PowerShell command to search for it:</span></span>

`
    Get-EXORecipient -Filter "EmailAddresses -eq 'email@contoso.onmicrosoft.com'"
`
  
<span data-ttu-id="bbd2f-108">Ako ne želite izbrisati postojeću adresu e-pošte, odaberite novu adresu e-pošte za novi objekt koji stvarate.</span><span class="sxs-lookup"><span data-stu-id="bbd2f-108">If you don't want to delete the existing email address, choose a new email address for the new object you are creating.</span></span>
  