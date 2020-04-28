---
title: Dodavanje vanjskih korisnika u grupu za raspodjelu
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: 7dbc69bced9ca800d3f95081b77dda5e49662579
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/27/2020
ms.locfileid: "43910924"
---
# <a name="add-external-users-to-a-distribution-group"></a><span data-ttu-id="6cd9a-102">Dodavanje vanjskih korisnika u grupu za raspodjelu</span><span class="sxs-lookup"><span data-stu-id="6cd9a-102">Add external users to a Distribution Group</span></span>

<span data-ttu-id="6cd9a-103">Dodavanje vanjskog kontakta u grupu za raspodjelu (DG) postupak je u dva koraka:</span><span class="sxs-lookup"><span data-stu-id="6cd9a-103">Adding an external contact to a Distribution Group (DG) is a two-step process:</span></span>
  
1. <span data-ttu-id="6cd9a-104">Stvaranje kontakta e-pošte za vanjskog korisnika:</span><span class="sxs-lookup"><span data-stu-id="6cd9a-104">Create a Mail Contact for the external user:</span></span>
    
    1. <span data-ttu-id="6cd9a-105">U centru za administratore otvorite stranicu **Kontakti** > [korisnika.](https://admin.microsoft.com/adminportal/home#/Contact)</span><span class="sxs-lookup"><span data-stu-id="6cd9a-105">In the admin center, go to the **Users** > [Contacts](https://admin.microsoft.com/adminportal/home#/Contact) page.</span></span> 
    
    2. <span data-ttu-id="6cd9a-106">Odaberite **Dodaj kontakt**.</span><span class="sxs-lookup"><span data-stu-id="6cd9a-106">Select **Add a contact**.</span></span>
    
    3. <span data-ttu-id="6cd9a-107">Upišite podatke za svoj kontakt i odaberite **Dodaj**.</span><span class="sxs-lookup"><span data-stu-id="6cd9a-107">Type the information for your contact and select **Add**.</span></span>
    
2. <span data-ttu-id="6cd9a-108">Dodajte kontakt e-pošte u dg:</span><span class="sxs-lookup"><span data-stu-id="6cd9a-108">Add the Mail Contact to your DG:</span></span>
    
    1. <span data-ttu-id="6cd9a-109">U centru za administratore idite na stranicu **Grupe grupa.** > [Groups](https://admin.microsoft.com/adminportal/home#/groups)</span><span class="sxs-lookup"><span data-stu-id="6cd9a-109">In the admin center, go to the **Groups** > [Groups](https://admin.microsoft.com/adminportal/home#/groups) page.</span></span> 
    
    2. <span data-ttu-id="6cd9a-110">Pronađite GG kojem želite dodati vanjskog korisnika i odaberite je da biste otvorili dijaloški okvir za uređivanje.</span><span class="sxs-lookup"><span data-stu-id="6cd9a-110">Find the DG you want to add the external user to, and select it to open the edit dialog.</span></span>
    
    3. <span data-ttu-id="6cd9a-111">Na kartici **Članovi** odaberite **Prikaži sve i upravljaj članovima**.</span><span class="sxs-lookup"><span data-stu-id="6cd9a-111">On the **Members** tab, select **View all and manage members**.</span></span> 
    
    4. <span data-ttu-id="6cd9a-112">Odaberite **Dodaj članove**.</span><span class="sxs-lookup"><span data-stu-id="6cd9a-112">Select **Add members**.</span></span>
    
    5. <span data-ttu-id="6cd9a-113">Odaberite kontakt pošte koji ste stvorili u prethodnom koraku, a zatim odaberite **Spremi**.</span><span class="sxs-lookup"><span data-stu-id="6cd9a-113">Select the Mail Contact you created on the previous step, and then select **Save**.</span></span>
    
<span data-ttu-id="6cd9a-114">Ako nakon ovih koraka vanjski korisnici ne mogu slati e-poštu GU-u ili ne primaju poruke e-pošte od nje, moguće je da je GU označen tako da dopušta samo e-poštu od internih korisnika.</span><span class="sxs-lookup"><span data-stu-id="6cd9a-114">If after following these steps your external users can't send emails to the DG or don't receive emails from it, it could be that the DG is marked to only allow emails from internal users.</span></span> <span data-ttu-id="6cd9a-115">Možete provjeriti ovu konfiguraciju i popraviti ga slijedeći upute [ovdje](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).</span><span class="sxs-lookup"><span data-stu-id="6cd9a-115">You can check this configuration and fix it following the directions [here](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).</span></span>
  
 <span data-ttu-id="6cd9a-116">**Napomena:** Te se upute ne primjenjuju ako je vrsta grupe "Grupa Microsoft 365" umjesto "Grupa za distribuciju".</span><span class="sxs-lookup"><span data-stu-id="6cd9a-116">**Note:** These instructions don't apply if your group's type is "Microsoft 365 group" instead of "Distribution group."</span></span> <span data-ttu-id="6cd9a-117">Ako je to slučaj, vanjski korisnik možete dodati izravno u grupu iz programa Outlook.</span><span class="sxs-lookup"><span data-stu-id="6cd9a-117">If that is the case, you can add the external user directly to the group from Outlook.</span></span> <span data-ttu-id="6cd9a-118">Detaljne informacije o gostima grupa ci35 grupa kao i upute za dodavanje vanjskih gostiju možete pronaći u [ovom članku](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span><span class="sxs-lookup"><span data-stu-id="6cd9a-118">Detailed information on Microsoft 365 Groups guests as well as instructions for adding external guests can be found in [this article](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span></span>
  