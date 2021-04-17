---
title: Suvremeno slanje faktura putem e-pošte za Azure
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003801"
- "6866"
ms.openlocfilehash: 4df8c49880fe638c1659f76edc0905532d091e45
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820818"
---
# <a name="email-invoicing-in-azure"></a><span data-ttu-id="647f9-102">Slanje faktura putem e-pošte u sustavu za Azure</span><span class="sxs-lookup"><span data-stu-id="647f9-102">Email invoicing in Azure</span></span>

<span data-ttu-id="647f9-103">Morate imati ulogu vlasnika ili suradnika na profilu za naplatu ili računu za naplatu da biste ažurirali preferencu za slanje faktura putem e-pošte.</span><span class="sxs-lookup"><span data-stu-id="647f9-103">You must have an owner or a contributor role on the billing profile or its billing account to update its email invoice preference.</span></span> <span data-ttu-id="647f9-104">Nakon što se uključite, svi korisnici s ulogama vlasnika, suradnika, čitatelja i upravitelja faktura na profilu za naplatu primit će tu fakturu putem e-pošte.</span><span class="sxs-lookup"><span data-stu-id="647f9-104">Once you have opted-in, all users with an owner, contributor, readers, and invoice manager roles on a billing profile will get its invoice in email.</span></span>

1. <span data-ttu-id="647f9-105">Prijavite se na [portal platforme Microsoft Azure](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="647f9-105">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="647f9-106">Potražite **Upravljanje troškovima + naplata**.</span><span class="sxs-lookup"><span data-stu-id="647f9-106">Search for **Cost Management + Billing**.</span></span>
3. <span data-ttu-id="647f9-107">Odaberite **Fakture** na lijevoj strani zaslona i zatim odaberite **Slanje fakture putem e-pošte** na vrhu stranice.</span><span class="sxs-lookup"><span data-stu-id="647f9-107">Select **Invoices** from the left-hand side and then select **Email Invoice** from the top of the page.</span></span>
4. <span data-ttu-id="647f9-108">Ako imate više profila za naplatu, odaberite profil za naplatu i zatim odaberite **Uključivanje**.</span><span class="sxs-lookup"><span data-stu-id="647f9-108">If you have multiple billing profiles, select a billing profile and then select **Opt in**.</span></span>

5. <span data-ttu-id="647f9-109">Odaberite **Ažuriraj**.</span><span class="sxs-lookup"><span data-stu-id="647f9-109">Select **Update**.</span></span>
6. <span data-ttu-id="647f9-110">Ako imate više profila za naplatu, odaberite profil za naplatu i zatim odaberite **Uključivanje**.</span><span class="sxs-lookup"><span data-stu-id="647f9-110">If you have multiple billing profiles, select a billing profile and then select **Opt in**.</span></span>

<span data-ttu-id="647f9-111">Drugima ćete omogućiti pristup za prikaz, preuzimanje i plaćanje faktura tako što ćete im dodijeliti ulogu upravitelja faktura za profil za naplatu MCA ili MPA.</span><span class="sxs-lookup"><span data-stu-id="647f9-111">You give others access to view, download, and pay invoices by assigning them the invoice manager role for an MCA or MPA billing profile.</span></span> <span data-ttu-id="647f9-112">Ako ste se uključili za primanje fakture putem e-pošte, korisnici će također primati fakture putem e-pošte.</span><span class="sxs-lookup"><span data-stu-id="647f9-112">If you've opted in to get your invoice in email, users also get the invoices in email.</span></span>

1. <span data-ttu-id="647f9-113">Prijavite se na [portal platforme Microsoft Azure](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="647f9-113">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="647f9-114">Potražite **Upravljanje troškovima + naplata**.</span><span class="sxs-lookup"><span data-stu-id="647f9-114">Search for **Cost Management + Billing**.</span></span>
3. <span data-ttu-id="647f9-115">Odaberite **Profili za naplatu** na lijevoj strani zaslona.</span><span class="sxs-lookup"><span data-stu-id="647f9-115">Select **Billing profiles** from the left-hand side.</span></span> <span data-ttu-id="647f9-116">S popisa profila za naplatu odaberite profil za naplatu kojemu želite dodijeliti ulogu upravitelja faktura.</span><span class="sxs-lookup"><span data-stu-id="647f9-116">From the billing profiles list, select a billing profile for which you want to assign an invoice manager role.</span></span>
4. <span data-ttu-id="647f9-117">Odaberite **Kontrola pristupa (IAM)** na lijevoj strani zaslona i zatim odaberite **Dodaj** s vrha stranice.</span><span class="sxs-lookup"><span data-stu-id="647f9-117">Select **Access Control (IAM)** from the left-hand side and then select **Add** from the top of the page.</span></span>

<span data-ttu-id="647f9-118">U padajućem izborniku uloga odaberite **Upravitelj faktura**.</span><span class="sxs-lookup"><span data-stu-id="647f9-118">In the Role drop-down list, select **Invoice Manager**.</span></span> <span data-ttu-id="647f9-119">Unesite adresu e-pošte korisnika da biste mu omogućili pristup.</span><span class="sxs-lookup"><span data-stu-id="647f9-119">Enter the email address of the user to give access.</span></span> <span data-ttu-id="647f9-120">Odaberite **Spremi** da biste dodijelili ulogu.</span><span class="sxs-lookup"><span data-stu-id="647f9-120">Select **Save** to assign the role.</span></span>
