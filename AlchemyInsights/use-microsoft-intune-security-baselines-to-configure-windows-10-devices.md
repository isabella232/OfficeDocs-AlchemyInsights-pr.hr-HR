---
title: Konfiguriranje uređaja sa sustavom Windows 10 pomoću Microsoft Intune sigurnosne osnove
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/10/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8371"
- "9004622"
ms.openlocfilehash: b95454ec8ce8d0d69d1f55f7ce4adc596929e2de
ms.sourcegitcommit: 1b554c31d008492f9e6464f0249af0332212a3fc
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50692904"
---
# <a name="use-the-microsoft-intune-security-baselines-for-configuring-windows-10-devices"></a><span data-ttu-id="1c036-102">Korištenje Microsoftovih sigurnosnih osnovnih stranica za konfiguriranje uređaja sa sustavom Windows 10</span><span class="sxs-lookup"><span data-stu-id="1c036-102">Use the Microsoft Intune security baselines for configuring Windows 10 devices</span></span>

<span data-ttu-id="1c036-103">Umetanje sigurnosnih osnovnih stranica olakšava zaštitu korisnika i uređaja.</span><span class="sxs-lookup"><span data-stu-id="1c036-103">Intune security baselines help protect users and devices.</span></span> <span data-ttu-id="1c036-104">Sigurnosne osnove sustava Windows postavke su prije konfigurirane grupe koje se koriste za primjenu poznate grupe postavki i zadanih vrijednosti koje preporučuje relevantni sigurnosni timovi.</span><span class="sxs-lookup"><span data-stu-id="1c036-104">Security baselines are Windows settings' pre-configured groups used to apply a known group of settings and default values recommended by the relevant security teams.</span></span> <span data-ttu-id="1c036-105">Stvaranjem profila sigurnosnog osnovnog sustava u programu Intune stvara se predložak koji se sastoji od više profila za konfiguraciju uređaja.</span><span class="sxs-lookup"><span data-stu-id="1c036-105">By creating a security baseline profile in Intune, you create a template that consists of multiple device-configuration profiles.</span></span>

<span data-ttu-id="1c036-106">Kada implementirate sigurnosne osnovice na grupe korisnika ili uređaja, postavke se primjenjuju na uređaje koji se pokreću u sustavu Windows 10 ili novijim verzijama.</span><span class="sxs-lookup"><span data-stu-id="1c036-106">When you deploy security baselines to groups of users or devices, the settings are applied to devices that run on Windows 10 or later versions.</span></span> <span data-ttu-id="1c036-107">Primjerice, sigurnosno osnovica za upravljanje Microsoftovim mobilnim uređajima (MDM) automatski (1) omogućuje BitLocker za uklonjive pogone, (2) potrebna je lozinka za otključavanje uređaja i (3) onemogućuje osnovnu provjeru autentičnosti.</span><span class="sxs-lookup"><span data-stu-id="1c036-107">For example, the Microsoft mobile device management (MDM) security baseline automatically (1) enables BitLocker for removable drives, (2) requires the password for unlocking a device, and (3) disables basic authentication.</span></span> <span data-ttu-id="1c036-108">Kada zadana vrijednost ne funkcionira u vašem okruženju, možete prilagoditi osnovicu da biste primijenili postavke koje su vam potrebne.</span><span class="sxs-lookup"><span data-stu-id="1c036-108">When a default value doesn't work for your environment, you can customize the baseline to apply the settings you need.</span></span>

<span data-ttu-id="1c036-109">Sigurnosni bazelini također pomažu u osnivanju krajnje sigurnog tijeka rada u programu Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="1c036-109">Security baselines also help establish an end-to-end secure workflow in Microsoft 365.</span></span> <span data-ttu-id="1c036-110">Slijede neke prednosti ove funkcionalnosti:</span><span class="sxs-lookup"><span data-stu-id="1c036-110">The following are some benefits of this functionality:</span></span>
- <span data-ttu-id="1c036-111">Sigurnosno osnovica obuhvaća najbolje prakse i preporuke za postavke koje utječu na sigurnost.</span><span class="sxs-lookup"><span data-stu-id="1c036-111">A security baseline includes the best practices and recommendations for settings that affect security.</span></span> <span data-ttu-id="1c036-112">Budući da je Intune Partners s timom za sigurnost sustava Windows koji stvara osnovice za pravila grupe, ove se preporuke temelje na čvrstim smjernicama i opsežnom iskustvu.</span><span class="sxs-lookup"><span data-stu-id="1c036-112">Because Intune partners with the Windows security team that creates baselines for group policies, these recommendations are based on solid guidance and extensive experience.</span></span>
- <span data-ttu-id="1c036-113">Ako ste novi u Intune i niste sigurni gdje početi, onda će vam sigurnosne osnove pomoći da brzo stvorite i implementirate siguran profil.</span><span class="sxs-lookup"><span data-stu-id="1c036-113">If you're new to Intune and unsure of where to start, then security baselines will help you quickly create and deploy a secure profile.</span></span>
- <span data-ttu-id="1c036-114">Ako trenutno koristite pravilo grupe, zatim Migriranje u potrebe za upravljanjem znatno je jednostavnije uz sigurnosne osnovice, jer se te sigurnosne osnove ugrađuju u Intune i obuhvaćaju najmodernije mogućnosti za upravljanje.</span><span class="sxs-lookup"><span data-stu-id="1c036-114">If you are currently using a group policy, then migrating to Intune for management purposes is much easier with security baselines, because these security baselines are built into Intune and include cutting-edge capabilities for management.</span></span>

<span data-ttu-id="1c036-115">Dodatne informacije potražite u članku [sigurnosne osnove sustava Windows](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines) i [Upravljanje mobilnim uređajima](https://docs.microsoft.com/windows/client-management/mdm/).</span><span class="sxs-lookup"><span data-stu-id="1c036-115">For more information, see [Windows security baselines](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines) and [Mobile device management](https://docs.microsoft.com/windows/client-management/mdm/).</span></span>