---
title: Otklanjanje poteškoća sa sustavom Office 365 Napredno zaštita od prijetnje
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1039
ms.assetid: ''
ms.openlocfilehash: 5a13653ba08d8c6b822354ff70f6d276d31cd816
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658906"
---
# <a name="troubleshooting-office-365-advanced-threat-protection"></a><span data-ttu-id="666e7-102">Otklanjanje poteškoća sa sustavom Office 365 Napredno zaštita od prijetnje</span><span class="sxs-lookup"><span data-stu-id="666e7-102">Troubleshooting Office 365 Advanced Threat Protection</span></span>

- <span data-ttu-id="666e7-103">Primjećujete li kašnjenje u isporuci poruke?</span><span class="sxs-lookup"><span data-stu-id="666e7-103">Do you notice delays in message delivery?</span></span> <span data-ttu-id="666e7-104">Pomoću mogućnosti [dinamičke isporuke](https://docs.microsoft.com/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) u pravilima programa ATP siguran privici.</span><span class="sxs-lookup"><span data-stu-id="666e7-104">Use the [Dynamic Delivery](https://docs.microsoft.com/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) option in your ATP Safe Attachments policy.</span></span> <span data-ttu-id="666e7-105">Time će se izbjeći kašnjenje poruka dok se primatelji štite od zlonamjernih datoteka.</span><span class="sxs-lookup"><span data-stu-id="666e7-105">This will help avoid message delays while protecting recipients from malicious files.</span></span>

- <span data-ttu-id="666e7-106">Želite li Microsoftu prijaviti netočne ili FALSE negative?</span><span class="sxs-lookup"><span data-stu-id="666e7-106">Do you want to report false positives or false negatives to Microsoft?</span></span> <span data-ttu-id="666e7-107">Upotrijebite ovu [vezu](https://www.microsoft.com/wdsi/filesubmission/) da biste poslali datoteke za analizu.</span><span class="sxs-lookup"><span data-stu-id="666e7-107">Use this [link](https://www.microsoft.com/wdsi/filesubmission/) to submit files for analysis.</span></span>

- <span data-ttu-id="666e7-108">Jeste li znali da možete omogućiti sigurnu vezu za zaštitu interne e-pošte poslane među primateljima unutar tvrtke ili ustanove?</span><span class="sxs-lookup"><span data-stu-id="666e7-108">Did you know that you can enable Safe Links protection for internal email sent between recipients within your organization?</span></span> <span data-ttu-id="666e7-109">Slijedite ove korake:</span><span class="sxs-lookup"><span data-stu-id="666e7-109">Follow these steps:</span></span>

  1. <span data-ttu-id="666e7-110">Idite na [https://protection.office.com](https://protection.office.com) i prijavite se pomoću računa globalnog administratora ili sigurnosnog administratora.</span><span class="sxs-lookup"><span data-stu-id="666e7-110">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

  2. <span data-ttu-id="666e7-111">U lijevoj navigacijskom oknu u odjeljku **Upravljanje prijetnjama**odaberite **Policy** \> **sigurne veze**za pravilnik.</span><span class="sxs-lookup"><span data-stu-id="666e7-111">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Links**.</span></span>

  3. <span data-ttu-id="666e7-112">U **pravilima koja se odnose na cijelu tvrtku ili ustanovu** odaberite pravilo, a zatim kliknite **Uredi**.</span><span class="sxs-lookup"><span data-stu-id="666e7-112">In the **Policies that apply to the entire organization** section, select the policy and click **Edit**.</span></span>

  4. <span data-ttu-id="666e7-113">U odjeljku **Postavke**omogućite **primjenu sigurnih veza na poruke poslane unutar tvrtke ili ustanove**.</span><span class="sxs-lookup"><span data-stu-id="666e7-113">Under **Settings**, enable **Apply safe links to messages sent within the organization**.</span></span>
