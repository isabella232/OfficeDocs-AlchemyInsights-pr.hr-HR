---
title: Konfiguriranje Microsoft Intune sigurnosnih osnovica za Windows 10 uređaje
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9006500"
- "11142"
ms.openlocfilehash: 88525fccd6dcde0cb3949e348d1f2a7df3ee7ce7
ms.sourcegitcommit: f7a9e97d04b7b6cbb633b32094d40f1874bf0fce
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52793613"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a><span data-ttu-id="f78e0-102">Konfiguriranje Microsoft Intune sigurnosnih osnovica za Windows 10 uređaje</span><span class="sxs-lookup"><span data-stu-id="f78e0-102">Use Microsoft Intune security baselines to configure Windows 10 devices</span></span>

<span data-ttu-id="f78e0-103">Intune sigurnosne osnovne vrijednosti štite korisnike i uređaje.</span><span class="sxs-lookup"><span data-stu-id="f78e0-103">Intune security baselines help protect users and devices.</span></span> <span data-ttu-id="f78e0-104">Sigurnosne osnovne vrijednosti Windows unaprijed konfigurirane grupe koje se koriste za primjenu poznate grupe postavki i zadanih vrijednosti koje preporučuju odgovarajući sigurnosni timovi.</span><span class="sxs-lookup"><span data-stu-id="f78e0-104">Security baselines are Windows settings pre-configured groups used to apply a known group of settings and default values recommended by the relevant security teams.</span></span> <span data-ttu-id="f78e0-105">Stvaranjem sigurnosnog osnovnog profila u aplikaciji Intune stvarate predložak koji se sastoji od više profila konfiguracije uređaja.</span><span class="sxs-lookup"><span data-stu-id="f78e0-105">By creating a security baseline profile in Intune, you create a template that consists of multiple device-configuration profiles.</span></span>

<span data-ttu-id="f78e0-106">Prilikom implementacije sigurnosnih osnovica grupama korisnika ili uređaja postavke se primjenjuju na uređaje koji se Windows 10 novije verzije.</span><span class="sxs-lookup"><span data-stu-id="f78e0-106">When you deploy security baselines to groups of users or devices, the settings are applied to devices that run on Windows 10 or later.</span></span> <span data-ttu-id="f78e0-107">Na primjer, sigurnosna osnovica za upravljanje Microsoftovim mobilnim uređajima (MDM) automatski omogućuje BitLocker za uklonjive pogone, zahtijeva lozinku za otključavanje uređaja i onemogućuje osnovnu provjeru autentičnosti.</span><span class="sxs-lookup"><span data-stu-id="f78e0-107">For example, the Microsoft mobile device management (MDM) security baseline automatically enables BitLocker for removable drives, requires the password for unlocking a device, and disables basic authentication.</span></span> <span data-ttu-id="f78e0-108">Kada zadana vrijednost ne funkcionira za vaše okruženje, možete prilagoditi osnovnu vrijednost da biste primijenili potrebne postavke.</span><span class="sxs-lookup"><span data-stu-id="f78e0-108">When a default value doesn't work for your environment, you can customize the baseline to apply the settings you need.</span></span>

<span data-ttu-id="f78e0-109">Sigurnosne osnovice pomažu i pri uspostavi sigurnog tijeka rada s kraja na Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="f78e0-109">Security baselines also help establish an end-to-end secure workflow in Microsoft 365.</span></span> <span data-ttu-id="f78e0-110">Sigurnosna osnovica obuhvaća najbolje prakse i preporuke za postavke koje utječu na sigurnost.</span><span class="sxs-lookup"><span data-stu-id="f78e0-110">A security baseline includes the best practices and recommendations for settings that affect security.</span></span> <span data-ttu-id="f78e0-111">Intune partneri s Windows sigurnosnim timom koji stvaraju osnovne vrijednosti za pravilnike grupe, pa se te preporuke temelje na čvrstim smjernicama i opsežnom iskustvu.</span><span class="sxs-lookup"><span data-stu-id="f78e0-111">Intune partners with the Windows security team that creates baselines for group policies, so these recommendations are based on solid guidance and extensive experience.</span></span>

<span data-ttu-id="f78e0-112">Ako ste novi u programu Intune i niste sigurni gdje početi, sigurnosne osnovne vrijednosti pomoći će vam da brzo stvorite i implementite siguran profil.</span><span class="sxs-lookup"><span data-stu-id="f78e0-112">If you're new to Intune and unsure of where to start, security baselines help you quickly create and deploy a secure profile.</span></span> <span data-ttu-id="f78e0-113">Ako trenutno koristite pravilnik grupe, migriranje u Intune radi upravljanja mnogo je jednostavnije uz sigurnosne osnovne vrijednosti jer su ugrađene u Intune i obuhvaćaju vrhunske mogućnosti upravljanja.</span><span class="sxs-lookup"><span data-stu-id="f78e0-113">If you currently use a group policy, migrating to Intune for management purposes is much easier with security baselines because they are built into Intune and include cutting-edge management capabilities.</span></span>

<span data-ttu-id="f78e0-114">Dodatne informacije potražite u članku [Windows i](/windows/security/threat-protection/windows-security-baselines) upravljanje [mobilnim uređajima](/windows/client-management/mdm/).</span><span class="sxs-lookup"><span data-stu-id="f78e0-114">To learn more, see [Windows security baselines](/windows/security/threat-protection/windows-security-baselines) and [Mobile device management](/windows/client-management/mdm/).</span></span>

