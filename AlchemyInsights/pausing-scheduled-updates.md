---
title: Pauziranje zakazanih ažuriranja
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/30/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1129"
- "6700007"
ms.openlocfilehash: 13abc7c9201b1897a9c766add4d105ef12f0d66f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47721547"
---
# <a name="pausing-scheduled-updates"></a><span data-ttu-id="b9f6e-102">Pauziranje zakazanih ažuriranja</span><span class="sxs-lookup"><span data-stu-id="b9f6e-102">Pausing scheduled updates</span></span>

<span data-ttu-id="b9f6e-103">Kada se izda naredba Pause, uređaji ne obrađuju naredbu dok se sljedeći put ne prijave u Intune.</span><span class="sxs-lookup"><span data-stu-id="b9f6e-103">When a pause command is issued, devices don't process the command until the next time they check in to Intune.</span></span> <span data-ttu-id="b9f6e-104">Zbog toga vaši uređaji mogu imati sljedeće:</span><span class="sxs-lookup"><span data-stu-id="b9f6e-104">Because of this, your devices might have:</span></span>

- <span data-ttu-id="b9f6e-105">Instalirana zakazana ažuriranja prije prijave.</span><span class="sxs-lookup"><span data-stu-id="b9f6e-105">Installed the scheduled updates prior to check-in.</span></span>
- <span data-ttu-id="b9f6e-106">Isključeno je kada ste izdali naredbu Pause.</span><span class="sxs-lookup"><span data-stu-id="b9f6e-106">Been powered off when you issued the pause command.</span></span> <span data-ttu-id="b9f6e-107">U ovom slučaju, kada su uređaji bili uključeni, možda su preuzeli i instalirali zakazana ažuriranja prije prijave.</span><span class="sxs-lookup"><span data-stu-id="b9f6e-107">In this case, when the devices were powered on, they might have downloaded and installed the scheduled updates prior to check-in.</span></span>