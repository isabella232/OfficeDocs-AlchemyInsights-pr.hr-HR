---
title: Pristup pretplatama
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003799"
- "6805"
ms.openlocfilehash: 166380cff09f2a2bd9b7e8914d5db4071b6c3f12
ms.sourcegitcommit: bec3554bf061ef28a009f460fb9d0a661b4fc008
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 10/27/2020
ms.locfileid: "48807223"
---
# <a name="unable-to-sign-in-azure-due-to-browser-issues-browser-hangs-keeps-spinning-does-not-load-etc"></a><span data-ttu-id="37a00-102">Nije moguće prijaviti Azure zbog problema s preglednikom (ako se preglednik objesi, nastavlja se vrtjeti, ne učitava se, itd.)</span><span class="sxs-lookup"><span data-stu-id="37a00-102">Unable to Sign-in Azure due to browser issues (Browser hangs, keeps spinning, does not load, etc.)</span></span>

<span data-ttu-id="37a00-103">Nakon toga će vas možda utjecati Prekoračeno vrijeme.</span><span class="sxs-lookup"><span data-stu-id="37a00-103">You might be impacted by an outage.</span></span> <span data-ttu-id="37a00-104">Provjerite postoji li trenutna nevremena: [status stanja Azure](https://status.azure.com/status/history/).</span><span class="sxs-lookup"><span data-stu-id="37a00-104">Please check to see if there is an ongoing outage: [Azure Health Status](https://status.azure.com/status/history/).</span></span>

<span data-ttu-id="37a00-105">Odjavite se od svih aktivnih sesija servisa Azure.</span><span class="sxs-lookup"><span data-stu-id="37a00-105">Please log out of all the active Azure sessions.</span></span> <span data-ttu-id="37a00-106">Započnite privatni ili anonimni način web-preglednika.</span><span class="sxs-lookup"><span data-stu-id="37a00-106">Start a in-private or incognito mode of your web browser.</span></span>

<span data-ttu-id="37a00-107">Možete i pokušati osvježiti preglednik, koristiti neki drugi preglednik, izbrisati predmemorirane kolačiće ako više ne funkcionira.</span><span class="sxs-lookup"><span data-stu-id="37a00-107">You could also try to Refresh browser, use another browser, delete cache cookies if above doesn't work.</span></span>

<span data-ttu-id="37a00-108">Dodatne informacije: [Otklanjanje poteškoća s prijavom](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)</span><span class="sxs-lookup"><span data-stu-id="37a00-108">Learn more: [Troubleshoot Sign-in Issues](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)</span></span>

<span data-ttu-id="37a00-109">**Nije moguće pristupiti pretplatama**</span><span class="sxs-lookup"><span data-stu-id="37a00-109">**Unable to access subscriptions**</span></span>

<span data-ttu-id="37a00-110">Na [portalu Azure](https://portal.azure.com/)provjerite je li odabran ispravan direktorij Azure s računa u gornjem desnom kutu.</span><span class="sxs-lookup"><span data-stu-id="37a00-110">In the [Azure portal](https://portal.azure.com/), make sure that the correct Azure directory is selected from the account at the top right.</span></span>

<span data-ttu-id="37a00-111">U [centru za račun Azure](https://account.windowsazure.com/Subscriptions)provjerite je li korišten račun administrator računa.</span><span class="sxs-lookup"><span data-stu-id="37a00-111">In the [Azure Account center](https://account.windowsazure.com/Subscriptions), make sure if the account used is the account admin.</span></span>

<span data-ttu-id="37a00-112">Dodatne informacije: [Otklanjanje poteškoća koje su pronađene pretplate](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="37a00-112">Learn more: [Troubleshoot No Subscriptions found](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)</span></span>

<span data-ttu-id="37a00-113">**Nije moguće pristupiti povijesti naplate**</span><span class="sxs-lookup"><span data-stu-id="37a00-113">**Unable to access billing history**</span></span>

<span data-ttu-id="37a00-114">Administrator računa mora osigurati da korisnik koji pristupi podacima za naplatu bude dodan u servisu Azure Active Directory kao gost: [Dodajte ili izbrišite novog korisnika](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="37a00-114">The account admin needs to make sure the user accessing the billing information is added in the Azure Active directory as a guest user: [Add or delete a new user](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="37a00-115">Korisniku mora biti dodijeljena uloga globalnog administratora: [Dodjela uloge korisnicima](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="37a00-115">The user then needs to be given a Global admin role: [Assign role to users](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="37a00-116">Objavite to, korisniku se može dodijeliti pristup naplati pomoću RBAC pravilnika: [Dodijeli pristup naplati](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="37a00-116">Post this, the user can be given billing access using RBAC policies: [Grant access to billing](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="37a00-117">**Preporučeni dokumenti**</span><span class="sxs-lookup"><span data-stu-id="37a00-117">**Recommended Documents**</span></span>

-   [<span data-ttu-id="37a00-118">Ne mogu se prijaviti za upravljanje pretplatom na Azure</span><span class="sxs-lookup"><span data-stu-id="37a00-118">I can't sign in to manage my Azure subscription</span></span>](https://docs.microsoft.com/azure/billing-cannot-login-subscription?WT.mc_id=Portal-Microsoft_Azure_Support)