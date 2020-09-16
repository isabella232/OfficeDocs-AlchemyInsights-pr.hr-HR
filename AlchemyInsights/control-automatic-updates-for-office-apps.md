---
title: Kontrola automatskih ažuriranja za aplikacije sustava Office
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1743"
- "9000140"
ms.openlocfilehash: ab3d6e60bc1b67220adbdf7ba61599a6b7aa663a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47747768"
---
# <a name="control-automatic-updates-for-office-apps"></a><span data-ttu-id="44f37-102">Kontrola automatskih ažuriranja za aplikacije sustava Office</span><span class="sxs-lookup"><span data-stu-id="44f37-102">Control automatic updates for Office Apps</span></span>

<span data-ttu-id="44f37-103">Ažuriranja za aplikacije sustava Office po zadanom se preuzimaju automatski i primjenjuju u pozadini bez ikakvih intervencija korisnika.</span><span class="sxs-lookup"><span data-stu-id="44f37-103">By default, updates for Office Apps are downloaded automatically and applied in the background without any user intervention.</span></span> <span data-ttu-id="44f37-104">No administratori mogu kontrolirati kako se ažuriranja primjenjuju pomoću postavki sustava Office Update.</span><span class="sxs-lookup"><span data-stu-id="44f37-104">However, administrators can control how updates are applied by using Office Update settings.</span></span> <span data-ttu-id="44f37-105">Postavke ažuriranja administratorima omogućuju Omogućivanje i onemogućivanje automatskih ažuriranja, prikazivanje ili sakrivanje gumba **Ažuriraj sada** u sustavu Office, postavljanje rokova ažuriranja i još mnogo toga.</span><span class="sxs-lookup"><span data-stu-id="44f37-105">Update settings allow administrators to enable or disable automatic updates, show or hide the **Update Now** button in Office, set update deadlines, and more.</span></span> <span data-ttu-id="44f37-106">Detaljne informacije potražite u članku:</span><span class="sxs-lookup"><span data-stu-id="44f37-106">For detailed information, see:</span></span>

- [<span data-ttu-id="44f37-107">Konfiguriranje postavki ažuriranja za Office</span><span class="sxs-lookup"><span data-stu-id="44f37-107">Configure update settings for Office</span></span>](https://docs.microsoft.com/deployoffice/configure-update-settings-for-office-365-proplus)  
- [<span data-ttu-id="44f37-108">Automatsko ažuriranje za Office nije omogućeno</span><span class="sxs-lookup"><span data-stu-id="44f37-108">Automatic updating for Office is not enabled</span></span>](https://support.microsoft.com/help/2753538/automatic-updating-for-office-2013-and-office-2016-click-to-run-is-not)  
- [<span data-ttu-id="44f37-109">Definiranje načina ažuriranja sustava Office nakon instalacije</span><span class="sxs-lookup"><span data-stu-id="44f37-109">Define how Office is updated after it's installed</span></span>](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#updates-element)

<span data-ttu-id="44f37-110">Da biste pregledali postojeće postavke ažuriranja primijenjene na klijentsko računalo, slijedite ove korake:</span><span class="sxs-lookup"><span data-stu-id="44f37-110">To review the existing updates settings applied to a client machine, follow these steps:</span></span>

1. <span data-ttu-id="44f37-111">Otvorite uređivač registra tako da **počnete**  >  **pokretati**  >  **regedit**.</span><span class="sxs-lookup"><span data-stu-id="44f37-111">Open the Registry Editor by going to **Start** > **Run** > **regedit**.</span></span>
2. <span data-ttu-id="44f37-112">Prijeđite na sljedeće mjesto i pregledajte postavke sustava Office Update:</span><span class="sxs-lookup"><span data-stu-id="44f37-112">Switch to the following location and review the Office Update settings:</span></span>  
    <span data-ttu-id="44f37-113">je.</span><span class="sxs-lookup"><span data-stu-id="44f37-113">a.</span></span> <span data-ttu-id="44f37-114">HKEY_LOCAL_MACHINE \software\microsoft\office</span><span class="sxs-lookup"><span data-stu-id="44f37-114">HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Office</span></span>\  
    <span data-ttu-id="44f37-115">b.</span><span class="sxs-lookup"><span data-stu-id="44f37-115">b.</span></span> <span data-ttu-id="44f37-116">ClickToRun\Configuration</span><span class="sxs-lookup"><span data-stu-id="44f37-116">ClickToRun\Configuration</span></span>

<span data-ttu-id="44f37-117">**Notes**  Ako je ključ servisa officemgmtcom postavljen, možda će se prikazati poruka "ažuriranjima upravlja administrator sustava" u ažuriranju Office **Office**  >  **računa**  >  **Office Updates**.</span><span class="sxs-lookup"><span data-stu-id="44f37-117">**Note**  If the OfficeMgmtCOM key is set, you might see the "Updates are managed by your system administrator" message in **Office** > **Account** > **Office Updates**.</span></span> <span data-ttu-id="44f37-118">Dodatne informacije potražite u članku [upravljanje ažuriranjima aplikacija microsoft 365 pomoću upravitelja konfiguracije programa Microsoft Endpoint](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager).</span><span class="sxs-lookup"><span data-stu-id="44f37-118">For more info, see [Manage updates to Microsoft 365 Apps with Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager).</span></span>  