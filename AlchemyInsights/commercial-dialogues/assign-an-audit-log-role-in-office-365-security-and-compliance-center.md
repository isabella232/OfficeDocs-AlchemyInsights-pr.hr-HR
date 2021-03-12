---
title: Dodjela uloge zapisnika nadzora u centru za sigurnost & sigurnosti sustava Office 365
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/21/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7363"
- "9000722"
ms.openlocfilehash: 0eb470b6c17def5517db2f866ef40898b36662ed
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50743702"
---
# <a name="assign-an-audit-log-role-in-the-office-365-security--compliance-center"></a><span data-ttu-id="8c285-102">Dodjela uloge zapisnika nadzora u centru za sigurnost & sigurnosti sustava Office 365</span><span class="sxs-lookup"><span data-stu-id="8c285-102">Assign an Audit Log role in the Office 365 Security & Compliance Center</span></span>

<span data-ttu-id="8c285-103">Da biste pretražili zapisnik nadzora sustava Office 365, administratoru mora biti dodijeljena uloga **zapisnika nadzora samo za prikaz** ili ulogu **zapisnika nadzora** u sustavu Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="8c285-103">To search the Office 365 audit log, an administrator must be assigned the **View-Only Audit Logs** role or the **Audit Logs** role in Exchange Online.</span></span> <span data-ttu-id="8c285-104">Te su uloge dodijeljene grupama za upravljanje usklađivanjem i upravljanjem organizacijom prema zadanim postavkama.</span><span class="sxs-lookup"><span data-stu-id="8c285-104">These roles are assigned to the Compliance Management and Organization Management role groups by default.</span></span> <span data-ttu-id="8c285-105">Globalni administratori u sustavu Office 365 i Microsoft 365 automatski se dodaju kao članovi grupe uloga za upravljanje organizacijom.</span><span class="sxs-lookup"><span data-stu-id="8c285-105">Global administrators in Office 365 and Microsoft 365 are automatically added as members of the Organization Management role group.</span></span>

<span data-ttu-id="8c285-106">Da biste korisniku omogućili pretraživanje uz minimalnu razinu privilegija, stvorite prilagođenu grupu uloga u sustavu Exchange Online, dodajte ulogu **zapisnika nadzora** ili **zapisnika** nadzora, a zatim dodajte korisnika kao člana nove grupe uloga.</span><span class="sxs-lookup"><span data-stu-id="8c285-106">To enable a user to search with the minimum level of privileges, create a custom role group in Exchange Online, add the **View-Only Audit Logs** role or **Audit Logs** role, and then add the user as a member of the new role group.</span></span>

<span data-ttu-id="8c285-107">Dodatne informacije potražite u članku [Upravljanje grupama uloga u sustavu Exchange Online](https://docs.microsoft.com/Exchange/permissions-exo/role-groups) i [pretraživanje zapisnika nadzora u centru za sigurnost & usklađenosti](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance).</span><span class="sxs-lookup"><span data-stu-id="8c285-107">For more information, see [Manage role groups in Exchange Online](https://docs.microsoft.com/Exchange/permissions-exo/role-groups) and [Search the audit log in the Security & Compliance Center](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance).</span></span>