---
title: Stvarati i koristiti zajednički poštanski sandučić
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 1825cfd0a78a29734d0a5128e19acbfba9115d32
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/04/2019
ms.locfileid: "34717339"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>Poteškoća - korisnik nije pronađen u imeniku

<p>Ako korisnici primate poruku o pogrešci <strong> &ldquo; &hellip;korisnika možete&rsquo;t može pronaći u imeniku. Molimo pokušajte ponovo&hellip; </strong> gdje je vrsta problema <strong> &ldquo;korisnik nije u imenik.&rdquo;</strong>, možete dovršiti sljedeće korake za otklanjanje poteškoća.</p> <ol> <li>Provjerite račun koji je prihvatio poziv e-poštom je isti račun koji koristi se prijaviti kasnije. Provjerite je li korisnik koristi isti račun za prihvaćanje na Pozovi i prijaviti na web-mjestu. <br /><br />Za dodatne informacije pogledajte <a href="https://support.microsoft.com/en-us/help/12407/microsoft-account-how-to-manage-aliases">kako upravljati pseudonime za Microsoftov račun</a> želite upravljati prijava za Office 365. <br /><br /></li> <li>Pregledaj svakog web-mjesta u kojima korisnik prima pogrešku. <br /><br />na. Dodavanje <strong> &ldquo;/_layouts/15/people.aspx/membershipgroupid=0&rdquo; </strong> (unutar u dvostruke navodnike) na kraj URL web-mjesta. <br /><br />Primjer: https://&lt;contoso&gt;.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0 <br /><br />b. Odaberite korisnika s popisa. <br /><br />c. Kliknite <strong>Ukloni korisničke dozvole s vrpce</strong>. <br /><br />d. Dodavanje korisnika i ponovo pošaljite na poziv korisniku.</li> </ol>

