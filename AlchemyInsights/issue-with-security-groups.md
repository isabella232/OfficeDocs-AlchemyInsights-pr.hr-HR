---
title: Problem s sigurnosnim grupama
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8252"
- "9004397"
ms.openlocfilehash: 1198b79c3301bd2752a7385a6ba6746c8f0c2b5b
ms.sourcegitcommit: 22eaf0a151ab95414476f596db8d318b6540ff31
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50177385"
---
# <a name="issue-with-security-groups"></a>Problem s sigurnosnim grupama

**Ako vam se prikazuje Mrežna pogreška AADDS104**

Nevaljana pravila grupe za mrežnu sigurnost najčešći su uzrok mrežnih pogrešaka za Azure Active Directory domene Services (AD DS). Mrežna sigurnost grupa za virtualnu mrežu mora dopustiti pristup određenim lukama i protokoli. Ako su ovi priključci blokirani, platforma Azure ne može nadzirati ni ažurirati upravljane domene. Usklañeno je i sinkronizacija između Azure i Azure AD DS-a. Pobrinite se da zadani portovi ostanu otvoreni da biste izbjegli prekid servisa.

Da biste razumjeli i riješili najčešća upozorenja o problemima s konfiguracijom mrežne sigurnosne grupe, pročitajte članak [Dodavanje i provjera sigurnosnih grupa](https://docs.microsoft.com/azure/active-directory-domain-services/alert-nsg#verify-and-edit-existing-security-rules).
