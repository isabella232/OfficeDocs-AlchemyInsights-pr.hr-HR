---
title: Slanje poruke e-pošte pružanjem ID-a mrežne poruke
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
ms.openlocfilehash: e4a0a3d9b4fede9198c8a235d05945b30a6e0807
ms.sourcegitcommit: 60c504f3ac187eaf1141b3ba701d9e0633bdd968
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/08/2021
ms.locfileid: "50692775"
---
# <a name="submit-an-email-message-by-providing-the-network-message-id"></a><span data-ttu-id="3a4d2-102">Slanje poruke e-pošte pružanjem ID-a mrežne poruke</span><span class="sxs-lookup"><span data-stu-id="3a4d2-102">Submit an email message by providing the network message ID</span></span>

1. <span data-ttu-id="3a4d2-103">U nastavku **nove prijave za podnošenje** odaberite ID **e-pošte** i **mrežne poruke**.</span><span class="sxs-lookup"><span data-stu-id="3a4d2-103">In the **New submission** flyout, select **Email** and **Network Message ID**.</span></span>
2. <span data-ttu-id="3a4d2-104">Slijedite ove korake da biste pronašli ID poruke za poruku e-pošte u programu Outlook:</span><span class="sxs-lookup"><span data-stu-id="3a4d2-104">Follow these steps to find the message ID for an email message in Outlook:</span></span>
    1. <span data-ttu-id="3a4d2-105">Dvokliknite poruku e-pošte da biste je otvorili.</span><span class="sxs-lookup"><span data-stu-id="3a4d2-105">Double-click the email message to open it.</span></span>
    1. <span data-ttu-id="3a4d2-106">Odaberite   >  **Svojstva** datoteke.</span><span class="sxs-lookup"><span data-stu-id="3a4d2-106">Select **File** > **Properties**.</span></span>
    1. <span data-ttu-id="3a4d2-107">Otvorite Notepad ili prazan dokument programa Word, a zatim kopirajte i zalijepite sadržaj koji se nalazi u okviru **Internetska zaglavlja** u otvoreni dokument radi bolje vidljivosti.</span><span class="sxs-lookup"><span data-stu-id="3a4d2-107">Open Notepad or a blank Word document, and then copy and paste the content found in the **Internet headers** box into the open document for better visibility.</span></span>
    1. <span data-ttu-id="3a4d2-108">Pronađite polje **X-MS-Exchange-Organization-Network-ID** .</span><span class="sxs-lookup"><span data-stu-id="3a4d2-108">Locate the **X-MS-Exchange-Organization-Network-Message-Id** field.</span></span> <span data-ttu-id="3a4d2-109">Vrijednost iza **:** je ID koji vam je potreban za podnošenje.</span><span class="sxs-lookup"><span data-stu-id="3a4d2-109">The value after the **:** is the ID you need for your submission.</span></span>
3. <span data-ttu-id="3a4d2-110">U odjeljku **Primatelji**, ako je poruka e-pošte sletjela u mapu Bezvrijedna pošta za sve primatelje ove e-pošte, odaberite **Odaberi sve**.</span><span class="sxs-lookup"><span data-stu-id="3a4d2-110">Under **Recipients**, if the email landed in the junk mail folder for all recipients of this email, choose **Select All**.</span></span> <span data-ttu-id="3a4d2-111">Ako nije, odaberite samo korisnika koji je prijavio problem.</span><span class="sxs-lookup"><span data-stu-id="3a4d2-111">If not, select only the user who reported the issue.</span></span>
4. <span data-ttu-id="3a4d2-112">Ako ste odabrali **razlog za podnošenje**, navedite je li poruka trebala **biti blokirana kao** **neželjena pošta**, **phishing** ili **zlonamjerni softver**, a zatim odaberite **Pošalji**.</span><span class="sxs-lookup"><span data-stu-id="3a4d2-112">Under **Reason for submission**, if you select **Should have been blocked**, specify whether the message should have been blocked as **Spam**, **Phishing**, or **Malware**, and then select **Submit**.</span></span>

<span data-ttu-id="3a4d2-113">Da biste doznali više, pročitajte članak [upute za skeniranje u programu Microsoft radi skeniranja](https://go.microsoft.com/fwlink/?linkid=2101479).</span><span class="sxs-lookup"><span data-stu-id="3a4d2-113">To learn more, see [How to submit suspected spam, phish, URLs, and files to Microsoft for scanning](https://go.microsoft.com/fwlink/?linkid=2101479).</span></span>
