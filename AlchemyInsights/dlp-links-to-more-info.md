---
title: Dodatne informacije o problemima s DLP-om
ms.author: pebaum
author: pebaum
manager: laurawi
ms.audience: admin
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2447"
- "3200001"
ms.openlocfilehash: 6525cee0555f1ae67b7d4e32445b9a1537d4a804
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932686"
---
# <a name="information-about-dlp-issues"></a><span data-ttu-id="d0218-102">Informacije o DLP pitanjima</span><span class="sxs-lookup"><span data-stu-id="d0218-102">Information about DLP issues</span></span>

<span data-ttu-id="d0218-103">**Važno**: Mnogi korisnici sustava SharePoint Online i OneDrive pokrenuti poslovne kritične aplikacije protiv servisa koji se izvodi u pozadini.</span><span class="sxs-lookup"><span data-stu-id="d0218-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="d0218-104">To uključuje migraciju sadržaja, sprječavanje gubitka podataka (DLP) i sigurnosna rješenja.</span><span class="sxs-lookup"><span data-stu-id="d0218-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="d0218-105">Tijekom ovih dosad nezabilježenih vremena poduzimamo korake kako bismo osigurali da usluge sustava SharePoint Online i OneDrive ostanu vrlo dostupne i pouzdane za korisnike koji više nego ikad ovise o usluzi.</span><span class="sxs-lookup"><span data-stu-id="d0218-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="d0218-106">U prilog tom cilju, implementirali smo stroža ograničenja regulacije pozadinskih aplikacija (migracije, DLP i backup rješenja) tijekom radnih dana.</span><span class="sxs-lookup"><span data-stu-id="d0218-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="d0218-107">Trebali biste očekivati da ove aplikacije će postići vrlo ograničen propusnost tijekom tih vremena.</span><span class="sxs-lookup"><span data-stu-id="d0218-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="d0218-108">Međutim, tijekom večernjih i vikend sati za regiju, usluga će biti spremna za obradu znatno veći volumen zahtjeva iz pozadinskih aplikacija.</span><span class="sxs-lookup"><span data-stu-id="d0218-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="d0218-109">**Informacije o pravilima dlp-a**</span><span class="sxs-lookup"><span data-stu-id="d0218-109">**Information on DLP policy**</span></span>

<span data-ttu-id="d0218-110">Pomoću Pravila dlp-a možete prepoznati, nadzirati i automatski zaštititi osjetljive podatke u sustavu Office 365.</span><span class="sxs-lookup"><span data-stu-id="d0218-110">With a DLP policy, you can identify, monitor, and automatically protect sensitive information across Office 365.</span></span>

<span data-ttu-id="d0218-111">Molimo posjetite ove linkove za više informacija:</span><span class="sxs-lookup"><span data-stu-id="d0218-111">Please visit these links for more information:</span></span>

- [<span data-ttu-id="d0218-112">Pregled prevencije gubitka podataka</span><span class="sxs-lookup"><span data-stu-id="d0218-112">Overview of data loss prevention</span></span>](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies)
- [<span data-ttu-id="d0218-113">Što traže osjetljive vrste informacija</span><span class="sxs-lookup"><span data-stu-id="d0218-113">What the sensitive information types look for</span></span>](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
- [<span data-ttu-id="d0218-114">Stvaranje prilagođene vrste osjetljivih informacija</span><span class="sxs-lookup"><span data-stu-id="d0218-114">Create a custom sensitive information type</span></span>](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type)
- [<span data-ttu-id="d0218-115">Slanje obavijesti e-poštom i prikaz savjeta o pravilima</span><span class="sxs-lookup"><span data-stu-id="d0218-115">Send email notifications and show policy tips</span></span>](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)
- [<span data-ttu-id="d0218-116">Zaštita datoteka sustava SharePoint Online oznakama zadržavanja i DLP-om</span><span class="sxs-lookup"><span data-stu-id="d0218-116">Protect SharePoint Online files with retention labels and DLP</span></span>](https://docs.microsoft.com/office365/securitycompliance/protect-sharepoint-online-files-with-office-365-labels-and-dlp)
- [<span data-ttu-id="d0218-117">DLP i Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="d0218-117">DLP and Microsoft Teams</span></span>](https://docs.microsoft.com/office365/securitycompliance/dlp-microsoft-teams)

<span data-ttu-id="d0218-118">Da biste testirali podatke pomoću ugrađene ili prilagođene osjetljive vrste informacija, upotrijebite opciju **Vrsta testiranja** u odjeljku **Klasifikacije Osjetljive** > **vrste podataka**.</span><span class="sxs-lookup"><span data-stu-id="d0218-118">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="d0218-119">Dodatne informacije potražite [u odjeljku Testiranje prilagođenih osjetljivih vrsta informacija](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span><span class="sxs-lookup"><span data-stu-id="d0218-119">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>