---
title: 1048 5.7.750 Usluga nije dostupna. Klijent je blokirao slanje s neregistriranih domena
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 8cf6d70b-9a78-4f04-ac59-7ffcf44ffd22
ms.custom:
- "1048"
- "3100026"
ms.openlocfilehash: 48b9c2de27f8d7f52215c3a3d547bdf746a3a4cd
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43676705"
---
# <a name="57750-client-blocked-from-sending-from-unregistered-domain"></a><span data-ttu-id="df02d-103">5.7.750 Klijent je blokirao slanje iz neregistrirane domene</span><span class="sxs-lookup"><span data-stu-id="df02d-103">5.7.750 Client blocked from sending from unregistered domain</span></span>

<span data-ttu-id="df02d-104">Pogreška se pojavljuje kada se velika količina poruka šalje iz domena koje nisu dodijeljene vašem klijentu (dodane kao prihvaćene domene i provjerene).</span><span class="sxs-lookup"><span data-stu-id="df02d-104">The error occurs when a large volume of messages are sent from domains that aren't provisioned in your tenant (added as accepted domains and validated).</span></span>

<span data-ttu-id="df02d-105">Da biste izbjegli tu pogrešku, možete koristiti konektor tijeka pošte utemeljen na certifikatu gdje je domena certifikata dodijeljena domena ili možete dodijeliti sve domene koje šalju.</span><span class="sxs-lookup"><span data-stu-id="df02d-105">To avoid this error, you can use a certificate-based mail flow connector where the certificate's domain is a provisioned domain, or you can provision all sending domains.</span></span>
