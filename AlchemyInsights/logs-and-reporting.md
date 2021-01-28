---
title: Zapisnici i izvješćivanje
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
- "9004331"
- "7727"
ms.openlocfilehash: 7349efb02f8d6ac5d73f6d6cd06eef6308ffe9be
ms.sourcegitcommit: 117c64e1fbcb5eec04f94eadad71423b974e7b14
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 01/27/2021
ms.locfileid: "50035862"
---
# <a name="logs-and-reporting"></a><span data-ttu-id="97025-102">Zapisnici i izvješćivanje</span><span class="sxs-lookup"><span data-stu-id="97025-102">Logs and Reporting</span></span>

<span data-ttu-id="97025-103">FAQ na servisu Azure [Active Directory javlja](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-faq) se najčešća pitanja o izvješćivanju Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="97025-103">[Azure Active Directory reporting FAQ](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-faq) answers frequently asked questions about Azure Active Directory (Azure AD) reporting.</span></span> <span data-ttu-id="97025-104">Dodatne informacije potražite u članku [izvješće o servisu Azure Active Directory](https://docs.microsoft.com/azure/active-directory/reports-monitoring/overview-reports).</span><span class="sxs-lookup"><span data-stu-id="97025-104">For more information, see [Azure Active Directory reporting](https://docs.microsoft.com/azure/active-directory/reports-monitoring/overview-reports).</span></span>

<span data-ttu-id="97025-105">**Otklanjanje poteškoća s revizijom**</span><span class="sxs-lookup"><span data-stu-id="97025-105">**Troubleshooting issues with Audit**</span></span>

1. <span data-ttu-id="97025-106">Ako imate problema s prikazanjem nekih revizijskih aktivnosti, a aktivnost koja nedostaje nalazi se na ovom [popisu](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-audit-activities), potvrdite kartu za podršku.</span><span class="sxs-lookup"><span data-stu-id="97025-106">If you are having issues seeing some audit activities and the missing Activity is in this [list](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-audit-activities), please file a support ticket.</span></span>
2. <span data-ttu-id="97025-107">Ako imate problema s prikazanjem svih zapisnika nadzora u zakupniku, pošaljite kartu za podršku.</span><span class="sxs-lookup"><span data-stu-id="97025-107">If you are having issues seeing any Audit logs in your tenant, please file a support ticket.</span></span>
3. <span data-ttu-id="97025-108">Ako se vaše Revizijske aktivnosti ne prikazuju odmah na portalu Azure, pogledajte [informacije o skrivenoj](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) u nastavku i datoteku podrške ako kašnjenje premašuje dokumentiranu latenciju.</span><span class="sxs-lookup"><span data-stu-id="97025-108">If your audit activities are not showing up immediately in the Azure Portal, check out our [latency information](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) and file a support ticket if the delay exceeds the documented latency.</span></span>
4. [<span data-ttu-id="97025-109">Zadržavanje zapisnika aktivnosti u servisu Azure AD</span><span class="sxs-lookup"><span data-stu-id="97025-109">Azure AD Activity Logs Retention</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-data-retention)
5. <span data-ttu-id="97025-110">Ako ne vidite sve revizije za odabrani datumski raspon, možete preuzeti do 250K redaka (Sortirano po najnovijim) prijava iz portala Azure.</span><span class="sxs-lookup"><span data-stu-id="97025-110">If you don't see all the audit for the date range you selected, you can download up to 250K rows (sorted by most recent) of sign-ins from Azure portal.</span></span> <span data-ttu-id="97025-111">Dodatne informacije potražite u članku [Preuzimanje nadzornih aktivnosti](https://docs.microsoft.com/azure/active-directory/reports-monitoring/quickstart-download-audit-report).</span><span class="sxs-lookup"><span data-stu-id="97025-111">For more information, see [Audit activities download](https://docs.microsoft.com/azure/active-directory/reports-monitoring/quickstart-download-audit-report).</span></span>

<span data-ttu-id="97025-112">**Otklanjanje poteškoća s prijavom**</span><span class="sxs-lookup"><span data-stu-id="97025-112">**Troubleshooting issues with Sign-ins**</span></span>

1. <span data-ttu-id="97025-113">Ako imate licencu za Azure AD Premium (P1 ili P2) za svog stanara, možete vidjeti samo zadnjih 30 dana podataka.</span><span class="sxs-lookup"><span data-stu-id="97025-113">You can only see the last 30 days of data if you have an Azure AD Premium (P1 or P2) license for your tenant.</span></span>
2. <span data-ttu-id="97025-114">Prijave dostupne su samo za stanare Azure AD Premium.</span><span class="sxs-lookup"><span data-stu-id="97025-114">Sign-ins are available only for Azure AD Premium tenants.</span></span> <span data-ttu-id="97025-115">Nije dostupan za besplatne ili osnovne licencirane zakupce.</span><span class="sxs-lookup"><span data-stu-id="97025-115">It's not available for Free or Basic licensed tenants.</span></span>
3. <span data-ttu-id="97025-116">Ako vaš zakupac ima licencu za popravak premije i ne možete vidjeti prijave, pogledajte [informacije o skrivenost](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) i datoteku podrške ako kašnjenje premašuje dokumentiranu latenciju.</span><span class="sxs-lookup"><span data-stu-id="97025-116">If your tenant has a Premium P1 license and you can't see the sign-ins, check out our [latency information](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) and file a support ticket if the delay exceeds the documented latency.</span></span>
4. <span data-ttu-id="97025-117">Ako ne vidite sve prijave za odabrani datumski raspon, imajte na čemu možete preuzeti do 250K redaka (Sortirano po najnovijim) prijava iz portala Azure.</span><span class="sxs-lookup"><span data-stu-id="97025-117">If you don't see all the sign-ins for the date range you selected, note that you can download up to 250K rows (sorted by most recent) of sign-ins from Azure portal.</span></span> <span data-ttu-id="97025-118">Dodatne informacije potražite u članku [Preuzimanje aktivnosti prijave](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-sign-ins#download-sign-in-activities).</span><span class="sxs-lookup"><span data-stu-id="97025-118">For more information, see [Sign-ins activities download](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-sign-ins#download-sign-in-activities).</span></span>

<span data-ttu-id="97025-119">**Otklanjanje poteškoća s sigurnosnim izvješćima (korisnici označeni u riziku, rizično prijavljivanje)**</span><span class="sxs-lookup"><span data-stu-id="97025-119">**Troubleshoot Security Reports (Users Flagged at Risk, Risky Sign-In)**</span></span>

1. [<span data-ttu-id="97025-120">Označeni korisnici za izvješće o sigurnosti rizika</span><span class="sxs-lookup"><span data-stu-id="97025-120">Users flagged for risk security report</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-user-at-risk)
2. [<span data-ttu-id="97025-121">Rizično izvješće o prijavi u portalu Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="97025-121">Risky sign-ins report in the Azure Active Directory portal</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-risky-sign-ins)
3. [<span data-ttu-id="97025-122">Događaji rizika za Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="97025-122">Azure Active Directory risk events</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-risk-events)
