---
title: Fakturiranje moderne Azure e-pošte
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003801"
- "6866"
ms.openlocfilehash: 65df6091a97d4937379ded384a78b5d07aa76e42
ms.sourcegitcommit: a5ba4dc8c349ed79147f67b62bde544281f7c106
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 11/03/2020
ms.locfileid: "48922001"
---
# <a name="email-invoicing-in-azure"></a><span data-ttu-id="62865-102">Fakturiranje e-pošte u servisu Azure</span><span class="sxs-lookup"><span data-stu-id="62865-102">Email invoicing in Azure</span></span>

<span data-ttu-id="62865-103">Da biste ažurirali svoju sklonost fakturi za e-poštu, morate imati vlasnika ili ulogu suradnika na profilu naplate ili račun za naplatu.</span><span class="sxs-lookup"><span data-stu-id="62865-103">You must have an owner or a contributor role on the billing profile or its billing account to update its email invoice preference.</span></span> <span data-ttu-id="62865-104">Kada se uključite, svi korisnici s ulogama vlasnik, suradnik, čitatelji i upravitelj faktura na profilu naplate dobit će svoj račun u poruci e-pošte.</span><span class="sxs-lookup"><span data-stu-id="62865-104">Once you have opted-in, all users with an owner, contributor, readers, and invoice manager roles on a billing profile will get its invoice in email.</span></span>

1. <span data-ttu-id="62865-105">Prijavite se na [portal Azure](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="62865-105">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="62865-106">Potražite **Upravljanje troškovima + naplata**.</span><span class="sxs-lookup"><span data-stu-id="62865-106">Search for **Cost Management + Billing**.</span></span>
3. <span data-ttu-id="62865-107">Na lijevoj strani odaberite **fakture** , a zatim odaberite **fakturu e-pošte** s vrha stranice.</span><span class="sxs-lookup"><span data-stu-id="62865-107">Select **Invoices** from the left-hand side and then select **Email Invoice** from the top of the page.</span></span>
4. <span data-ttu-id="62865-108">Ako imate više profila za naplatu, odaberite profil za naplatu, a zatim odaberite **Uključivanje u** nju.</span><span class="sxs-lookup"><span data-stu-id="62865-108">If you have multiple billing profiles, select a billing profile and then select **Opt in**.</span></span>

5. <span data-ttu-id="62865-109">Odaberite **Ažuriraj**.</span><span class="sxs-lookup"><span data-stu-id="62865-109">Select **Update**.</span></span>
6. <span data-ttu-id="62865-110">Ako imate više profila za naplatu, odaberite profil za naplatu, a zatim odaberite **Uključivanje u** nju.</span><span class="sxs-lookup"><span data-stu-id="62865-110">If you have multiple billing profiles, select a billing profile and then select **Opt in**.</span></span>

<span data-ttu-id="62865-111">Osobama možete dati pristup za prikaz, preuzimanje i plaćanje faktura tako da im dodijelite ulogu upravitelja faktura za profil za MCA ili MPA za naplatu.</span><span class="sxs-lookup"><span data-stu-id="62865-111">You give others access to view, download, and pay invoices by assigning them the invoice manager role for an MCA or MPA billing profile.</span></span> <span data-ttu-id="62865-112">Ako ste se uključili da biste dobili fakturu u poruci e-pošte, korisnici će dobiti i fakture u poruci e-pošte.</span><span class="sxs-lookup"><span data-stu-id="62865-112">If you've opted in to get your invoice in email, users also get the invoices in email.</span></span>

1. <span data-ttu-id="62865-113">Prijavite se na [portal Azure](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="62865-113">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="62865-114">Potražite **Upravljanje troškovima + naplata**.</span><span class="sxs-lookup"><span data-stu-id="62865-114">Search for **Cost Management + Billing**.</span></span>
3. <span data-ttu-id="62865-115">Na lijevoj strani odaberite **profile za naplatu** .</span><span class="sxs-lookup"><span data-stu-id="62865-115">Select **Billing profiles** from the left-hand side.</span></span> <span data-ttu-id="62865-116">Na popisu Profili za naplatu odaberite profil za naplatu kojem želite dodijeliti ulogu upravitelja faktura.</span><span class="sxs-lookup"><span data-stu-id="62865-116">From the billing profiles list, select a billing profile for which you want to assign an invoice manager role.</span></span>
4. <span data-ttu-id="62865-117">Na lijevoj strani odaberite **Control Access (IAM)** , a zatim odaberite **Dodaj** s vrha stranice.</span><span class="sxs-lookup"><span data-stu-id="62865-117">Select **Access Control (IAM)** from the left-hand side and then select **Add** from the top of the page.</span></span>

<span data-ttu-id="62865-118">Na padajućem popisu uloga odaberite **Upravitelj faktura**.</span><span class="sxs-lookup"><span data-stu-id="62865-118">In the Role drop-down list, select **Invoice Manager**.</span></span> <span data-ttu-id="62865-119">Unesite adresu e-pošte korisnika da biste dali pristup.</span><span class="sxs-lookup"><span data-stu-id="62865-119">Enter the email address of the user to give access.</span></span> <span data-ttu-id="62865-120">Odaberite **Spremi** da biste dodijelili ulogu.</span><span class="sxs-lookup"><span data-stu-id="62865-120">Select **Save** to assign the role.</span></span>
