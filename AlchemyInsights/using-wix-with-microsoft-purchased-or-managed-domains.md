---
title: Korištenje Wix web-mjesta s Microsoftovim kupljenim ili upravljanim domenama
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/05/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5855"
- "9003096"
ms.openlocfilehash: f6845c56f05e9cef11362ce601a974b73a154c9a
ms.sourcegitcommit: 28a319e482e6a8644e87726e1b0e599819df52d0
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2020
ms.locfileid: "46629388"
---
# <a name="using-a-wix-website-with-microsoft-purchased-or-managed-domains"></a><span data-ttu-id="9bbaa-102">Korištenje Wix web-mjesta s Microsoftovim kupljenim ili upravljanim domenama</span><span class="sxs-lookup"><span data-stu-id="9bbaa-102">Using a Wix website with Microsoft purchased or managed domains</span></span>

<span data-ttu-id="9bbaa-103">Informacije o tome kako koristiti Wix web-mjesto s Microsoftovom kupljenom ili upravljanom domenom potražite [u članku Ažuriranje DNS zapisa radi zadržavanja web-mjesta s trenutnim davatelja usluga hostiranja](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider).</span><span class="sxs-lookup"><span data-stu-id="9bbaa-103">For information about how to use a Wix website with a Microsoft purchased or managed domain, see [Update DNS records to keep your website with your current hosting provider](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider).</span></span>

<span data-ttu-id="9bbaa-104">Pojedinosti potražite u članku:</span><span class="sxs-lookup"><span data-stu-id="9bbaa-104">For details, see:</span></span> 

- <span data-ttu-id="9bbaa-105">Članak Wix, "povezivanje domene sa sustavom Wix pomoću metode pokazujući", preporučuje se dodavanjem DNS zapisa kao što je navedeno u nastavku, a ne promjenom poslužitelja naziva kada koristite Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="9bbaa-105">The Wix article, "Connecting a Domain to Wix Using the Pointing Method," recommends adding DNS records as outlined in the link above rather than changing names servers when you're using Microsoft 365.</span></span>

- <span data-ttu-id="9bbaa-106">Ako odaberete promjenu poslužitelja naziva u Wix, morate stvoriti DNS zapise u programu Wix za Microsoft.</span><span class="sxs-lookup"><span data-stu-id="9bbaa-106">If you choose to change name servers to Wix, you must create DNS records at Wix for Microsoft.</span></span> <span data-ttu-id="9bbaa-107">Dodatne informacije potražite u članku [Stvaranje DNS zapisa u programu Wix za Microsoft](https://docs.microsoft.com/microsoft-365/admin/dns/create-dns-records-at-wix).</span><span class="sxs-lookup"><span data-stu-id="9bbaa-107">For more info, see [Create DNS records at Wix for Microsoft](https://docs.microsoft.com/microsoft-365/admin/dns/create-dns-records-at-wix).</span></span>

- <span data-ttu-id="9bbaa-108">Ako je vaša domena kupljena od Microsofta, poslužitelji naziva ne mogu se promijeniti.</span><span class="sxs-lookup"><span data-stu-id="9bbaa-108">If your domain was purchased from Microsoft the name servers can't be changed.</span></span> <span data-ttu-id="9bbaa-109">Ako morate promijeniti poslužitelje naziva, Microsoftova kupljena domena mora se prenijeti na drugog davatelja usluge hostiranja nakon 60 dana.</span><span class="sxs-lookup"><span data-stu-id="9bbaa-109">If you must change names servers, the Microsoft purchased domain must be transferred to another hosting provider after 60 days.</span></span> <span data-ttu-id="9bbaa-110">Dodatne informacije potražite u članku [Najčešća pitanja o domenama](https://docs.microsoft.com/microsoft-365/admin/setup/domains-faq#can-i-transfer-a-domain-i-purchased-from-microsoft-to-another-provider).</span><span class="sxs-lookup"><span data-stu-id="9bbaa-110">For more info, see the [Domains FAQ](https://docs.microsoft.com/microsoft-365/admin/setup/domains-faq#can-i-transfer-a-domain-i-purchased-from-microsoft-to-another-provider).</span></span>