---
title: Implementacija aplikacije Win32 app
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6446"
- "6700004"
ms.openlocfilehash: 5ccbf37bd3f06da2f8c3955d87e449ea58caab1c
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 10/06/2020
ms.locfileid: "48461758"
---
# <a name="intune-win32-app-deployment"></a><span data-ttu-id="1bf24-102">Implementacija aplikacije Win32 app</span><span class="sxs-lookup"><span data-stu-id="1bf24-102">Intune Win32 app deployment</span></span>

<span data-ttu-id="1bf24-103">Microsoft Intune omogućuje aplikacije Win32, uključujući, ali ne ograničavajući se na MSI i. EXE će se implementirati na uređajima sa sustavom Windows 10.</span><span class="sxs-lookup"><span data-stu-id="1bf24-103">Microsoft Intune allows Win32 applications, including but not limited to MSI and .EXE’s to be deployed to Windows 10 devices.</span></span> <span data-ttu-id="1bf24-104">Korišten je mehanizam implementacije da bi se na ciljnom uređaju prikazao proširenje (IME) za upravljanje.</span><span class="sxs-lookup"><span data-stu-id="1bf24-104">The deployment mechanism used requires the Intune Management Extension (IME) to be present on the target device.</span></span> <span data-ttu-id="1bf24-105">IME će se automatski instalirati kao rezultat ciljanja skripte za PowerShell ili programa Win32 na korisnika/uređaja.</span><span class="sxs-lookup"><span data-stu-id="1bf24-105">The IME will be installed automatically as a result of targeting a powershell script or win32 application deployment to a user / device.</span></span>

<span data-ttu-id="1bf24-106">Postoji i skup unaprijed obaveznih zahtjeva koji se moraju zadovoljiti da bi se implementirali Win32 aplikacije koje obuhvaćaju sljedeće:</span><span class="sxs-lookup"><span data-stu-id="1bf24-106">There are also a set of pre-requisites which must be met in order to deploy Win32 apps which include:</span></span>

- <span data-ttu-id="1bf24-107">Podržane platforme: Windows 10 verzija 1607 ili novija (verzije poduzeća, Pro i obrazovne ustanove).</span><span class="sxs-lookup"><span data-stu-id="1bf24-107">Supported platforms: Windows 10 version 1607 or later (Enterprise, Pro, and Education versions).</span></span>
- <span data-ttu-id="1bf24-108">Podržana arhitektura: x86 i x64.</span><span class="sxs-lookup"><span data-stu-id="1bf24-108">Supported architecture: x86 and x64.</span></span>
- <span data-ttu-id="1bf24-109">Upravljanje uređajima: AAD se pridružio i automatski upisuje (uključujući hibridnu domenu i pravila grupe automatski se upisuju).</span><span class="sxs-lookup"><span data-stu-id="1bf24-109">Device Management: AAD joined and auto-enrolled (including hybrid domain joined and group policy auto-enrolled).</span></span>
- <span data-ttu-id="1bf24-110">Oblik paketa aplikacija:. **intunewin**  datoteka koju priprema [alat za pripremu sadržaja u programu Microsoft Win32](https://docs.microsoft.com/mem/intune/apps/apps-win32-prepare).</span><span class="sxs-lookup"><span data-stu-id="1bf24-110">Application Package format: .**intunewin**  file prepared by the [Microsoft Win32 content Prep tool](https://docs.microsoft.com/mem/intune/apps/apps-win32-prepare).</span></span>
- <span data-ttu-id="1bf24-111">Ograničenja</span><span class="sxs-lookup"><span data-stu-id="1bf24-111">Limitations:</span></span>
    - <span data-ttu-id="1bf24-112">Maksimalna veličina: 8GB.</span><span class="sxs-lookup"><span data-stu-id="1bf24-112">Maximum size: 8GB.</span></span>
    - <span data-ttu-id="1bf24-113">Nepodržana arhitektura: ruke.</span><span class="sxs-lookup"><span data-stu-id="1bf24-113">Unsupported architecture: ARMs.</span></span>

<span data-ttu-id="1bf24-114">Pregledajte dokument "[Dodavanje, dodjeljivanje i praćenje aplikacije Win32 u programu Microsoft Intune](https://docs.microsoft.com/mem/intune/apps/apps-win32-add)" za informacije vezane uz te korake.</span><span class="sxs-lookup"><span data-stu-id="1bf24-114">Review the doc "[Add, assign, and monitor a Win32 app in Microsoft Intune](https://docs.microsoft.com/mem/intune/apps/apps-win32-add)" for information related to those steps.</span></span>

<span data-ttu-id="1bf24-115">Pojedinosti o otklanjanju poteškoća prilikom implementacije aplikacija u sustavu Windows, uključujući aplikacije Win32, mogu se pregledati u sljedećim dokumentima</span><span class="sxs-lookup"><span data-stu-id="1bf24-115">Details on troubleshooting application deployment on Windows including Win32 apps can be reviewed in the following documents</span></span>

- [<span data-ttu-id="1bf24-116">Otklanjanje poteškoća s instalacijom aplikacija</span><span class="sxs-lookup"><span data-stu-id="1bf24-116">Troubleshoot App Installation issues</span></span>](https://docs.microsoft.com/mem/intune/apps/troubleshoot-app-install)  
- [<span data-ttu-id="1bf24-117">Otklanjanje poteškoća s aplikacijama Win32</span><span class="sxs-lookup"><span data-stu-id="1bf24-117">Troubleshoot Win32 Apps</span></span>](https://docs.microsoft.com/mem/intune/apps/apps-win32-troubleshoot)