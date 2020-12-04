---
title: Konfiguriranje uređaja sa sustavom Windows 10 pomoću Microsoft Intune sigurnosne osnove
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004135"
- "7211"
ms.openlocfilehash: 24257f1ac5752df1598d08fcfdb95ee2642adfea
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573298"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a><span data-ttu-id="0bc4f-102">Konfiguriranje uređaja sa sustavom Windows 10 pomoću Microsoft Intune sigurnosne osnove</span><span class="sxs-lookup"><span data-stu-id="0bc4f-102">Use Microsoft Intune security baselines to configure Windows 10 devices</span></span>

<span data-ttu-id="0bc4f-103">Umetanje sigurnosnih osnovnih stranica olakšava zaštitu korisnika i uređaja.</span><span class="sxs-lookup"><span data-stu-id="0bc4f-103">Intune security baselines help protect users and devices.</span></span> <span data-ttu-id="0bc4f-104">Sigurnosne osnove sustava Windows postavke su prije konfigurirane grupe koje se koriste za primjenu poznate grupe postavki i zadanih vrijednosti koje preporučuje relevantni sigurnosni timovi.</span><span class="sxs-lookup"><span data-stu-id="0bc4f-104">Security baselines are Windows settings' pre-configured groups used to apply a known group of settings and default values recommended by the relevant security teams.</span></span> <span data-ttu-id="0bc4f-105">Stvaranjem profila sigurnosnog osnovnog sustava u programu Intune stvara se predložak koji se sastoji od više profila za konfiguraciju uređaja.</span><span class="sxs-lookup"><span data-stu-id="0bc4f-105">By creating a security baseline profile in Intune, you create a template that consists of multiple device-configuration profiles.</span></span>

<span data-ttu-id="0bc4f-106">Kada implementirate sigurnosne osnovice na grupe korisnika ili uređaja, postavke se primjenjuju na uređaje koji se pokreću u sustavu Windows 10 ili novijim verzijama.</span><span class="sxs-lookup"><span data-stu-id="0bc4f-106">When you deploy security baselines to groups of users or devices, the settings are applied to devices that run on Windows 10 or later.</span></span> <span data-ttu-id="0bc4f-107">Na primjer, MDM sigurnost Baseline automatski (1) omogućuje BitLocker za uklonjive pogone, (2) potrebna je lozinka za otključavanje uređaja i (3) onemogućuje osnovnu provjeru autentičnosti.</span><span class="sxs-lookup"><span data-stu-id="0bc4f-107">For example, MDM Security Baseline automatically (1) enables BitLocker for removable drives, (2) requires the password for unlocking a device, and (3) disables basic authentication.</span></span> <span data-ttu-id="0bc4f-108">Kada zadana vrijednost ne funkcionira u vašem okruženju, prilagodite osnovicu da biste primijenili postavke koje su vam potrebne.</span><span class="sxs-lookup"><span data-stu-id="0bc4f-108">When a default value doesn't work for your environment, customize the baseline to apply the settings you need.</span></span>

<span data-ttu-id="0bc4f-109">Sigurnosni bazelini također pomažu u osnivanju krajnje sigurnog tijeka rada u programu Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="0bc4f-109">Security baselines also help establish an end-to-end secure workflow in Microsoft 365.</span></span> <span data-ttu-id="0bc4f-110">Slijede neke prednosti ovog:</span><span class="sxs-lookup"><span data-stu-id="0bc4f-110">The following are some benefits of this:</span></span>

- <span data-ttu-id="0bc4f-111">Sigurnosno osnovica obuhvaća najbolje prakse i preporuke za postavke koje utječu na sigurnost.</span><span class="sxs-lookup"><span data-stu-id="0bc4f-111">A security baseline includes the best practices and recommendations for settings that affect security.</span></span> <span data-ttu-id="0bc4f-112">Budući da je Intune Partners s timom za sigurnost sustava Windows koji stvara osnovice za pravila grupe, ove se preporuke temelje na čvrstim smjernicama i opsežnom iskustvu.</span><span class="sxs-lookup"><span data-stu-id="0bc4f-112">Because Intune partners with the Windows security team that creates baselines for group policies, these recommendations are based on solid guidance and extensive experience.</span></span>
- <span data-ttu-id="0bc4f-113">Ako ste novi u Intune i niste sigurni gdje početi, onda će vam sigurnosne osnove pomoći da brzo stvorite i implementirate siguran profil.</span><span class="sxs-lookup"><span data-stu-id="0bc4f-113">If you're new to Intune and unsure of where to start, then security baselines will help you quickly create and deploy a secure profile.</span></span>
- <span data-ttu-id="0bc4f-114">Ako trenutno koristite pravilo grupe, zatim Migriranje u potrebe za upravljanjem znatno je jednostavnije uz sigurnosne osnovice, jer su ugrađene u Intune i obuhvaćaju najmodernije mogućnosti za upravljanje.</span><span class="sxs-lookup"><span data-stu-id="0bc4f-114">If you currently use a group policy, then migrating to Intune for management purposes is much easier with security baselines, because they are built into Intune and include cutting-edge capabilities for management.</span></span>

<span data-ttu-id="0bc4f-115">Dodatne informacije potražite u članku [sigurnosne osnove sustava Windows](https://go.microsoft.com/fwlink/?linkid=2141503) i [Upravljanje mobilnim uređajima](https://go.microsoft.com/fwlink/?linkid=2141701).</span><span class="sxs-lookup"><span data-stu-id="0bc4f-115">To learn more, see [Windows security baselines](https://go.microsoft.com/fwlink/?linkid=2141503) and [Mobile device management](https://go.microsoft.com/fwlink/?linkid=2141701).</span></span>