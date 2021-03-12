---
title: Omogućivanje programa Microsoft Defender za Office 365 za SharePoint Online, OneDrive i Microsoftove timove
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 1c29afdcc52e7032fea22d698371677918665fa9
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50743547"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="b8899-102">Omogućivanje programa Microsoft Defender za Office 365 za SharePoint Online, OneDrive i Microsoftove timove</span><span class="sxs-lookup"><span data-stu-id="b8899-102">Enable Microsoft Defender for Office 365 for SharePoint Online, OneDrive and Microsoft Teams</span></span>

1. <span data-ttu-id="b8899-103">Pomoću vjerodajnica globalnog administratora ili administratora sigurnosti prijavite se u centar za [Sigurnost i usklađenost sustava Office 365](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="b8899-103">Using your global admin or security admin credentials, log in to the [Office 365 Security and Compliance Center](https://protection.office.com/).</span></span>
2. <span data-ttu-id="b8899-104">U levom oknu odaberite **Upravljanje prijetnjom** , a zatim odaberite   >  [sigurne privitke](https://protection.office.com/safeattachment)pravilnika.</span><span class="sxs-lookup"><span data-stu-id="b8899-104">Select **Threat management** in the left pane, and then select **Policy** > [Safe attachments](https://protection.office.com/safeattachment).</span></span>
3. <span data-ttu-id="b8899-105">Odaberite **Uključi Microsoft Defender za Office 365 za SharePoint, OneDrive i Microsoftove timove**, a zatim odaberite **Spremi**.</span><span class="sxs-lookup"><span data-stu-id="b8899-105">Select **Turn on Microsoft Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams**, and then select **Save**.</span></span>
    > [!TIP]
    >
    > - <span data-ttu-id="b8899-106">Kao globalni administrator ili administrator sustava SharePoint Online, pokrenite sljedeći cmdlet za PowerShell s parametrom **Disallowinfectedfiledownload** postavljen na *True*: [set-SPO,](https://go.microsoft.com/fwlink/?linkid=2092301)</span><span class="sxs-lookup"><span data-stu-id="b8899-106">As a global admin or a SharePoint Online admin, run the following PowerShell cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*: [Set-SPOTenant](https://go.microsoft.com/fwlink/?linkid=2092301)</span></span>
    > - [<span data-ttu-id="b8899-107">Postavljanje upozorenja za otkrivene datoteke</span><span class="sxs-lookup"><span data-stu-id="b8899-107">Set up alerts for detected files</span></span>](https://go.microsoft.com/fwlink/?linkid=2092110)

<span data-ttu-id="b8899-108">Dodatne informacije potražite u članku [Microsoft Defender za Office 365 za SharePoint, OneDrive i Microsoftove timove](https://go.microsoft.com/fwlink/?linkid=2092041).</span><span class="sxs-lookup"><span data-stu-id="b8899-108">For more information, see [Microsoft Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams](https://go.microsoft.com/fwlink/?linkid=2092041).</span></span>
