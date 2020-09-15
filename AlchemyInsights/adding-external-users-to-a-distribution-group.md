---
title: Dodavanje vanjskih korisnika u grupu za raspodjelu
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: 03cfd2c576cb03cbefd524a4ab6f04e2ef1eebec
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663505"
---
# <a name="add-external-users-to-a-distribution-group"></a><span data-ttu-id="e55a7-102">Dodavanje vanjskih korisnika u grupu za raspodjelu</span><span class="sxs-lookup"><span data-stu-id="e55a7-102">Add external users to a Distribution Group</span></span>

<span data-ttu-id="e55a7-103">Dodavanje vanjskog kontakta u grupu za raspodjelu (DG) postupak je u dva koraka:</span><span class="sxs-lookup"><span data-stu-id="e55a7-103">Adding an external contact to a Distribution Group (DG) is a two-step process:</span></span>
  
1. <span data-ttu-id="e55a7-104">Stvaranje kontakta e-pošte za vanjskog korisnika:</span><span class="sxs-lookup"><span data-stu-id="e55a7-104">Create a Mail Contact for the external user:</span></span>
    
    1. <span data-ttu-id="e55a7-105">U centru za administratore otvorite stranicu kontakti **korisnika**  >  [Contacts](https://admin.microsoft.com/adminportal/home#/Contact) .</span><span class="sxs-lookup"><span data-stu-id="e55a7-105">In the admin center, go to the **Users** > [Contacts](https://admin.microsoft.com/adminportal/home#/Contact) page.</span></span> 
    
    2. <span data-ttu-id="e55a7-106">Odaberite **Dodaj kontakt**.</span><span class="sxs-lookup"><span data-stu-id="e55a7-106">Select **Add a contact**.</span></span>
    
    3. <span data-ttu-id="e55a7-107">Unesite podatke za kontakt i odaberite **Dodaj**.</span><span class="sxs-lookup"><span data-stu-id="e55a7-107">Type the information for your contact and select **Add**.</span></span>
    
2. <span data-ttu-id="e55a7-108">Dodajte kontakt e-pošte u svoju DG:</span><span class="sxs-lookup"><span data-stu-id="e55a7-108">Add the Mail Contact to your DG:</span></span>
    
    1. <span data-ttu-id="e55a7-109">U centru za administratore otvorite stranicu **grupe**  >  [grupa](https://admin.microsoft.com/adminportal/home#/groups) .</span><span class="sxs-lookup"><span data-stu-id="e55a7-109">In the admin center, go to the **Groups** > [Groups](https://admin.microsoft.com/adminportal/home#/groups) page.</span></span> 
    
    2. <span data-ttu-id="e55a7-110">Pronađite DG u koju želite dodati vanjskog korisnika, a zatim ga odaberite da biste otvorili dijaloški okvir Uređivanje.</span><span class="sxs-lookup"><span data-stu-id="e55a7-110">Find the DG you want to add the external user to, and select it to open the edit dialog.</span></span>
    
    3. <span data-ttu-id="e55a7-111">Na kartici **Članovi** odaberite **Prikaz svih članova i upravljanje njima**.</span><span class="sxs-lookup"><span data-stu-id="e55a7-111">On the **Members** tab, select **View all and manage members**.</span></span> 
    
    4. <span data-ttu-id="e55a7-112">Odaberite **Dodaj članove**.</span><span class="sxs-lookup"><span data-stu-id="e55a7-112">Select **Add members**.</span></span>
    
    5. <span data-ttu-id="e55a7-113">Odaberite kontakt e-pošte koji ste stvorili u prethodnom koraku, a zatim odaberite **Spremi**.</span><span class="sxs-lookup"><span data-stu-id="e55a7-113">Select the Mail Contact you created on the previous step, and then select **Save**.</span></span>
    
<span data-ttu-id="e55a7-114">Ako nakon sljedećih koraka vaši vanjski korisnici ne mogu slati poruke e-pošte upravi ili ne primaju poruke e-pošte s nje, moguće je da je DG označena samo da dopušta poruke e-pošte od internih korisnika.</span><span class="sxs-lookup"><span data-stu-id="e55a7-114">If after following these steps your external users can't send emails to the DG or don't receive emails from it, it could be that the DG is marked to only allow emails from internal users.</span></span> <span data-ttu-id="e55a7-115">Tu konfiguraciju možete provjeriti i popraviti ga [uz upute za](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online)praćenje.</span><span class="sxs-lookup"><span data-stu-id="e55a7-115">You can check this configuration and fix it following the directions [here](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).</span></span>
  
 <span data-ttu-id="e55a7-116">**Upozorenje:** Ove se upute ne primjenjuju ako je vrsta grupe "Microsoft 365 Group" umjesto "grupa za raspodjelu".</span><span class="sxs-lookup"><span data-stu-id="e55a7-116">**Note:** These instructions don't apply if your group's type is "Microsoft 365 group" instead of "Distribution group."</span></span> <span data-ttu-id="e55a7-117">Ako je to slučaj, vanjski korisnik možete dodati izravno u grupu iz programa Outlook.</span><span class="sxs-lookup"><span data-stu-id="e55a7-117">If that is the case, you can add the external user directly to the group from Outlook.</span></span> <span data-ttu-id="e55a7-118">Detaljne informacije o tvrtki Microsoft 365 Groups, kao i upute za dodavanje vanjskih gostiju možete pronaći u [ovom članku](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span><span class="sxs-lookup"><span data-stu-id="e55a7-118">Detailed information on Microsoft 365 Groups guests as well as instructions for adding external guests can be found in [this article](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span></span>
  