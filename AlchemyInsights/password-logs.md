---
title: Zapisnici lozinki
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9361"
- "9003259"
ms.openlocfilehash: ed151b436fa2043c610931deeb74a202af88fcf4
ms.sourcegitcommit: 226fe97678b6be215eda0c278399f8be9be525c1
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/08/2021
ms.locfileid: "50524120"
---
# <a name="password-logs"></a><span data-ttu-id="8088e-102">Zapisnici lozinki</span><span class="sxs-lookup"><span data-stu-id="8088e-102">Password logs</span></span>

<span data-ttu-id="8088e-103">**Imam problema s pristupom zapisnicima nadzora pri ponovnom postavljanju lozinki**</span><span class="sxs-lookup"><span data-stu-id="8088e-103">**I'm having problems accessing password reset audit logs**</span></span>

<span data-ttu-id="8088e-104">Da biste otklonili poteškoće vezane uz pristup zapisnicima nadzora pri ponovnom postavljanju lozinke, izvedite sljedeći korak:</span><span class="sxs-lookup"><span data-stu-id="8088e-104">To troubleshoot issues regarding access to password reset audit logs, perform the following step:</span></span>

<span data-ttu-id="8088e-105">Provjerite jeste li ovlašteni za prikaz zapisnika nadzora.</span><span class="sxs-lookup"><span data-stu-id="8088e-105">Ensure you are authorized to view audit logs.</span></span> 

<span data-ttu-id="8088e-106">Ovlašteni su samo sljedeće uloge:</span><span class="sxs-lookup"><span data-stu-id="8088e-106">Only the following roles are authorized:</span></span>
 - <span data-ttu-id="8088e-107">Globalni administrator</span><span class="sxs-lookup"><span data-stu-id="8088e-107">Global administrator</span></span>
 - <span data-ttu-id="8088e-108">Administrator sigurnosti</span><span class="sxs-lookup"><span data-stu-id="8088e-108">Security administrator</span></span>
 - <span data-ttu-id="8088e-109">Čitač sigurnosnih tekstova</span><span class="sxs-lookup"><span data-stu-id="8088e-109">Security reader</span></span>

<span data-ttu-id="8088e-110">**Želim vidjeti sve izvorne postavke revizije za ponovno postavljanje lozinke od vremena kada sam se isprva raspoređen**</span><span class="sxs-lookup"><span data-stu-id="8088e-110">**I want to see all password reset audit events from the time I initially deployed**</span></span>

<span data-ttu-id="8088e-111">U izvješćima o posljednjih 30 dana spremaju se i događaji za vraćanje lozinke do 120.000.</span><span class="sxs-lookup"><span data-stu-id="8088e-111">Up to 120,000 password reset/registration events are stored in the reports of the last 30 days.</span></span> <span data-ttu-id="8088e-112">Ovo se maksimalno ograničenje primjenjuje na UI prilikom preuzimanja CSV-a.</span><span class="sxs-lookup"><span data-stu-id="8088e-112">This maximum limit applies to the UI when downloading the CSV.</span></span> <span data-ttu-id="8088e-113">1.000.000 događaji dostupni su pomoću komponente PowerShell.</span><span class="sxs-lookup"><span data-stu-id="8088e-113">1 million events are available through PowerShell.</span></span>
<span data-ttu-id="8088e-114">Dodatne informacije potražite u odjeljku veze u nastavku:</span><span class="sxs-lookup"><span data-stu-id="8088e-114">For more information, see the links below:</span></span>

- [<span data-ttu-id="8088e-115">Samoposlužni događaji za vraćanje izvorne lozinke iz izvješća Azure AD i eventa</span><span class="sxs-lookup"><span data-stu-id="8088e-115">Self-service password reset events from the Azure AD Reports and Events API</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="8088e-116">Kako brzo preuzeti lozinke za upis na izvornu lozinku pomoću komponente PowerShell</span><span class="sxs-lookup"><span data-stu-id="8088e-116">How to download password reset registration events quickly with PowerShell</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)

<span data-ttu-id="8088e-117">**Želim razumjeti više o mogućnostima izvješćivanja o ponovnom postavljanju lozinki**</span><span class="sxs-lookup"><span data-stu-id="8088e-117">**I want to understand more about password reset reporting capabilities**</span></span>

<span data-ttu-id="8088e-118">Provjerite tko registrira ili ponovno postavljanje lozinki pomoću zapisnika nadzora za vraćanje izvornih postavki servisa Azure AD na portalu Azure u odjeljku **Korisnici i grupe**.</span><span class="sxs-lookup"><span data-stu-id="8088e-118">Check who is registering for or resetting passwords with Azure AD password reset audit logs in the Azure portal under **Users and groups**.</span></span>
<span data-ttu-id="8088e-119">Dodatne informacije potražite u sljedećim vezama:</span><span class="sxs-lookup"><span data-stu-id="8088e-119">For more information, see the following links:</span></span>

- [<span data-ttu-id="8088e-120">Pregled izvješća o ponovnom postavljanju lozinke</span><span class="sxs-lookup"><span data-stu-id="8088e-120">Password reset reports overview</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="8088e-121">Prikaz izvješća o ponovnom postavljanju lozinki na portalu Azure</span><span class="sxs-lookup"><span data-stu-id="8088e-121">How to view password reset reports in the Azure portal</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="8088e-122">Samoposlužni događaji za vraćanje izvorne lozinke iz izvješća Azure AD i eventa</span><span class="sxs-lookup"><span data-stu-id="8088e-122">Self-service password reset events from the Azure AD Reports and Events API</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="8088e-123">Kako brzo preuzeti lozinke za upis na izvornu lozinku pomoću komponente PowerShell</span><span class="sxs-lookup"><span data-stu-id="8088e-123">How to download password reset registration events quickly with PowerShell</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)


