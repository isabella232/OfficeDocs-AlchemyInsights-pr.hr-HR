---
title: Ispravite probleme isporuke e-pošte javne mape
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1956
ms.assetid: ''
ms.openlocfilehash: 45665f900014c52e6a920325b0a3b0f6f79fb72d
ms.sourcegitcommit: d1c1d5bcb52ba9083e8dd7603feb72436c5154c8
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/17/2019
ms.locfileid: "31910583"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a><span data-ttu-id="86927-102">Ispravite probleme isporuke e-pošte javne mape</span><span class="sxs-lookup"><span data-stu-id="86927-102">Fix email delivery issues to mail-enabled public folders</span></span>

<span data-ttu-id="86927-103">Ako vanjskih pošiljatelja nije moguće slati poruke pošte omogućeno javne mape i pošiljatelji pogrešci: **ne može se pronaći (550 5.4.1)**, provjerite domena e-pošte za javnu mapu konfiguriran kao Interna preusmjeravanja domene umjesto programa Mjerodavne domene:</span><span class="sxs-lookup"><span data-stu-id="86927-103">If external senders can't send messages to your mail-enabled public folders, and the senders receive the error: **couldn't be found (550 5.4.1)**, verify the email domain for the public folder is configured as an internal relay domain instead of an authoritative domain:</span></span>

1. <span data-ttu-id="86927-104">Otvorili [Centar za administraciju sustava Exchange (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span><span class="sxs-lookup"><span data-stu-id="86927-104">Open the [Exchange admin center (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span></span>

2. <span data-ttu-id="86927-105">Idi na **Protok e-pošte** \> **domena prihvaćeno**, odaberite domenom prihvaćene, a zatim kliknite **Uređivanje**.</span><span class="sxs-lookup"><span data-stu-id="86927-105">Go to **Mail flow** \> **Accepted domains**, select the accepted domain, and then click **Edit**.</span></span>

3. <span data-ttu-id="86927-106">U svojstvima stranice da otvara ako je vrsta domene za **Authoritative**, promijenite vrijednost **Interna preusmjeravanja** i kliknite **Spremi**.</span><span class="sxs-lookup"><span data-stu-id="86927-106">In the properties page that opens, if the domain type is set to **Authoritative**, change the value to **Internal relay** and then click **Save**.</span></span>

<span data-ttu-id="86927-107">Vanjskih pošiljatelja primanje pogreška **nemate dozvolu (550 5.7.13)**, pokrenite sljedeću naredbu u [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) da biste vidjeli dozvole za anonimne korisnike u javnu mapu:</span><span class="sxs-lookup"><span data-stu-id="86927-107">If external senders receive the error **you don't have permission (550 5.7.13)**, run the following command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) to see the permissions for anonymous users in the public folder:</span></span>

<span data-ttu-id="86927-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous`Na primjer, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span><span class="sxs-lookup"><span data-stu-id="86927-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` For example, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span></span>

<span data-ttu-id="86927-109">Dopustiti vanjskim korisnicima da šalju e-pošte javne mape, dodajte CreateItems access desno korisnik anonimno.</span><span class="sxs-lookup"><span data-stu-id="86927-109">To allow external users to send email to this public folder, add the CreateItems access right to the user Anonymous.</span></span> <span data-ttu-id="86927-110">Na primjer, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span><span class="sxs-lookup"><span data-stu-id="86927-110">For example, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span></span>
