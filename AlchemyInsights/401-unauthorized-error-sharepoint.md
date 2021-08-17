---
title: 401 Neovlaštena pogreška u SharePoint
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/14/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10935"
- "9001435"
ms.openlocfilehash: 04f56dfc7ebe7de91bc64a5e6d2b480b07741c6e
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58314340"
---
# <a name="401-unauthorized-error-in-sharepoint"></a>401 Neovlaštena pogreška u SharePoint

Ako primite pogrešku "(401) Neovlašteno" u programu SharePoint možda je povezana s ukidanjom TLS 1.0/1.1. Dodatne informacije potražite u sljedećim člancima:

- [Priprema za TLS 1.2 u Office 365 i Office 365 GCC](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- [Pogreške provjere autentičnosti pojavljuju se ako klijent nema podršku za TLS 1.2](https://docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

- [Ažuriranje radi omogućivanja TLS 1.1 i TLS 1.2 kao zadanih sigurnih protokola u sustavu WinHTTP u Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)

Ako su korisnici na Windows 7, provjerite jesu li provjerili [TLS Cipher Suites u Windows 7](https://docs.microsoft.com/windows/win32/secauthn/tls-cipher-suites-in-windows-7).