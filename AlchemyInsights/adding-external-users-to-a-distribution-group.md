---
title: Dodavanje vanjskog korisnika grupe raspodjele
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: e84a5b04d6fc805deaa47cb10c91081f37411e5b
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36737865"
---
# <a name="add-external-users-to-a-distribution-group"></a><span data-ttu-id="96c7d-102">Dodavanje vanjski korisnici grupe raspodjele</span><span class="sxs-lookup"><span data-stu-id="96c7d-102">Add external users to a Distribution Group</span></span>

<span data-ttu-id="96c7d-103">Dodavanje vanjskog kontakta za na raspodjele grupe (DG) je postupak u dva koraka:</span><span class="sxs-lookup"><span data-stu-id="96c7d-103">Adding an external contact to a Distribution Group (DG) is a two-step process:</span></span>
  
1. <span data-ttu-id="96c7d-104">Stvaranje pošte kontaktu za vanjske korisnika:</span><span class="sxs-lookup"><span data-stu-id="96c7d-104">Create a Mail Contact for the external user:</span></span>
    
    1. <span data-ttu-id="96c7d-105">U centru za administraciju Idi **korisnici** > stranica[kontakata](https://admin.microsoft.com/adminportal/home#/Contact) .</span><span class="sxs-lookup"><span data-stu-id="96c7d-105">In the admin center, go to the **Users** > [Contacts](https://admin.microsoft.com/adminportal/home#/Contact) page.</span></span> 
    
    2. <span data-ttu-id="96c7d-106">Odaberite **Dodaj kontakt**.</span><span class="sxs-lookup"><span data-stu-id="96c7d-106">Select **Add a contact**.</span></span>
    
    3. <span data-ttu-id="96c7d-107">Unesite informacije za vaš kontakt i odaberite **Dodaj**.</span><span class="sxs-lookup"><span data-stu-id="96c7d-107">Type the information for your contact and select **Add**.</span></span>
    
2. <span data-ttu-id="96c7d-108">Dodavanje kontakta pošte vaše DG:</span><span class="sxs-lookup"><span data-stu-id="96c7d-108">Add the Mail Contact to your DG:</span></span>
    
    1. <span data-ttu-id="96c7d-109">U centru za administraciju Idi **grupe** > [grupe](https://admin.microsoft.com/adminportal/home#/groups) stranica.</span><span class="sxs-lookup"><span data-stu-id="96c7d-109">In the admin center, go to the **Groups** > [Groups](https://admin.microsoft.com/adminportal/home#/groups) page.</span></span> 
    
    2. <span data-ttu-id="96c7d-110">Traži DG želite dodati vanjskog korisnika i odaberite ga da biste otvorili dijaloški okvir Uređivanje.</span><span class="sxs-lookup"><span data-stu-id="96c7d-110">Find the DG you want to add the external user to, and select it to open the edit dialog.</span></span>
    
    3. <span data-ttu-id="96c7d-111">Na kartici **Članovi** odaberite **Prikaz svih i upravljanje članovima**.</span><span class="sxs-lookup"><span data-stu-id="96c7d-111">On the **Members** tab, select **View all and manage members**.</span></span> 
    
    4. <span data-ttu-id="96c7d-112">Odaberite **Dodaj članove**.</span><span class="sxs-lookup"><span data-stu-id="96c7d-112">Select **Add members**.</span></span>
    
    5. <span data-ttu-id="96c7d-113">Odaberite kontakt pošte stvorena na prethodni korak i odaberite **Spremi**.</span><span class="sxs-lookup"><span data-stu-id="96c7d-113">Select the Mail Contact you created on the previous step, and then select **Save**.</span></span>
    
<span data-ttu-id="96c7d-114">Ako nakon ovih koraka vanjski korisnici pošta nije moguće poslati na DG ili ne primate pošta iz nje, to može biti u DG označen samo iz internim korisnicima dopustiti pošta.</span><span class="sxs-lookup"><span data-stu-id="96c7d-114">If after following these steps your external users can't send emails to the DG or don't receive emails from it, it could be that the DG is marked to only allow emails from internal users.</span></span> <span data-ttu-id="96c7d-115">Provjerite konfiguraciju i popravite slijedeći upute [ovdje](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).</span><span class="sxs-lookup"><span data-stu-id="96c7d-115">You can check this configuration and fix it following the directions [here](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).</span></span>
  
 <span data-ttu-id="96c7d-116">**Napomena:** Te se upute ne primijenite ako je vaša grupa Vrsta "Office 365 grupa" umjesto "Grupu raspodjele."</span><span class="sxs-lookup"><span data-stu-id="96c7d-116">**Note:** These instructions don't apply if your group's type is "Office 365 group" instead of "Distribution group."</span></span> <span data-ttu-id="96c7d-117">Ako je to slučaj, možete dodati vanjskog korisnika izravno na grupe iz programa Outlook.</span><span class="sxs-lookup"><span data-stu-id="96c7d-117">If that is the case, you can add the external user directly to the group from Outlook.</span></span> <span data-ttu-id="96c7d-118">Detaljne informacije o Office 365 grupe Gosti i upute za dodavanje vanjskog Gosti mogu pronaći u [ovom članku](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span><span class="sxs-lookup"><span data-stu-id="96c7d-118">Detailed information on Office 365 groups guests as well as instructions for adding external guests can be found in [this article](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span></span>
  