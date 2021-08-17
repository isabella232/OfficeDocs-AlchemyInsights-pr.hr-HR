---
title: Temeljna veza zatvorena je pogreška u SharePoint
ms.author: pebaum
author: pebaum
manager: dansimp
ms.date: 04/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10802"
- "9006390"
ms.openlocfilehash: f0f82eaaa00d71992af445bb89346fb85bad3ade5d120b25ad3a6ea4f9674893
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/11/2021
ms.locfileid: "57883311"
---
# <a name="the-underlying-connection-was-closed-error-in-sharepoint"></a>Pogreška "Temeljna veza je zatvorena" u SharePoint

Ako se prikazuje pogreška "Temeljna veza je zatvorena" u programu SharePoint možda je povezana s ukidanjem TLS 1.0/1.1. Dodatne informacije potražite u člancima:

- [Priprema za TLS 1.2 u Office 365 i Office 365 GCC](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- [Pogreške provjere autentičnosti pojavljuju se ako klijent nema podršku za TLS 1.2](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

- [Ažuriranje radi omogućivanja TLS 1.1 i TLS 1.2 kao zadanih sigurnih protokola u sustavu WinHTTP u Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)

Ako su korisnici na Windows 7, provjerite jesu li provjerili [TLS Cipher Suites u Windows 7](https://docs.microsoft.com/windows/win32/secauthn/tls-cipher-suites-in-windows-7).