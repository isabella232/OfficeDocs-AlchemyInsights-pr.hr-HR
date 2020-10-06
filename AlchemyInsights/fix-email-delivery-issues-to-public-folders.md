---
title: Rješavanje problema s isporučenjem e-pošte javnim mapama s omogućenim e-poštom
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.openlocfilehash: 74a26306766ed7952a3bbbcb06f1f0113a113024
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 10/06/2020
ms.locfileid: "48366456"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a><span data-ttu-id="4a15d-102">Rješavanje problema s isporučenjem e-pošte javnim mapama s omogućenim e-poštom</span><span class="sxs-lookup"><span data-stu-id="4a15d-102">Fix email delivery issues to mail-enabled public folders</span></span>

<span data-ttu-id="4a15d-103">Ako vanjski pošiljatelji ne mogu slati poruke u javne mape koje su omogućene za e-poštu, a pošiljatelji primaju pogrešku: **nije ga moguće pronaći (550 je)**, provjerite je li domena e-pošte za javnu mapu konfigurirana kao domena za interni prijenos, a ne autoritativna domena:</span><span class="sxs-lookup"><span data-stu-id="4a15d-103">If external senders can't send messages to your mail-enabled public folders, and the senders receive the error: **couldn't be found (550 5.4.1)**, verify the email domain for the public folder is configured as an internal relay domain instead of an authoritative domain:</span></span>

1. <span data-ttu-id="4a15d-104">Otvorite [centar za administratore sustava Exchange (AAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span><span class="sxs-lookup"><span data-stu-id="4a15d-104">Open the [Exchange admin center (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span></span>

2. <span data-ttu-id="4a15d-105">Otvorite domene koje su prihvaćene za **tijek pošte** \> **Accepted domains**, odaberite prihvaćenu domenu, a zatim kliknite **Uredi**.</span><span class="sxs-lookup"><span data-stu-id="4a15d-105">Go to **Mail flow** \> **Accepted domains**, select the accepted domain, and then click **Edit**.</span></span>

3. <span data-ttu-id="4a15d-106">Na stranici svojstva koja se otvara, ako je vrsta domene postavljena na **autoritativna**, promijenite vrijednost u **interni prijenos** , a zatim kliknite **Spremi**.</span><span class="sxs-lookup"><span data-stu-id="4a15d-106">In the properties page that opens, if the domain type is set to **Authoritative**, change the value to **Internal relay** and then click **Save**.</span></span>

<span data-ttu-id="4a15d-107">Ako vanjski pošiljatelji dobiju pogrešku koja nema **dozvolu (550 5.7.13)**, pokrenite sljedeću naredbu u komponenti [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) da biste vidjeli dozvole za anonimne korisnike u javnoj mapi:</span><span class="sxs-lookup"><span data-stu-id="4a15d-107">If external senders receive the error **you don't have permission (550 5.7.13)**, run the following command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) to see the permissions for anonymous users in the public folder:</span></span>

<span data-ttu-id="4a15d-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` Na primjer, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous` .</span><span class="sxs-lookup"><span data-stu-id="4a15d-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` For example, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span></span>

<span data-ttu-id="4a15d-109">Da biste vanjskim korisnicima dopustili slanje e-pošte u tu javnu mapu, dodajte mogućnost pristupa CreateItems izravno korisniku anonimnom.</span><span class="sxs-lookup"><span data-stu-id="4a15d-109">To allow external users to send email to this public folder, add the CreateItems access right to the user Anonymous.</span></span> <span data-ttu-id="4a15d-110">Na primjer, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems` .</span><span class="sxs-lookup"><span data-stu-id="4a15d-110">For example, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span></span>
