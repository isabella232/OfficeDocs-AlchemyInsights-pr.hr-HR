---
title: Nije moguće aktivirati Office
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
- "2000023"
- "3509"
ms.openlocfilehash: 9a33b7880aff6016ef6df88960d6f59ac9dd50382c7e99d72ca36bc3c9f344ea
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53928361"
---
# <a name="unable-to-activate-office"></a>Nije moguće aktivirati Office

**Napomena:** ako koristite stariju verziju programa Windows (npr. Windows 7), provjerite je li TLS 1.2 omogućen kao zadani. Dodatne informacije potražite u članku Ažuriranje radi omogućivanja [TLS 1.1 i TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)kao zadanih sigurnih protokola u aplikaciji WinHTTP u Windows .

- Provjerite je li status vaše pretplate istekao.
- Provjerite imate li pretplatu koja omogućuje klijentske licence, kao što su Office 365 Business ili Business premium, te provjerite je [li korisniku dodijeljena licenca](/microsoft-365/admin/manage/assign-licenses-to-users).
- Provjerite je li se korisnik prijavljuje u Office s pomoću istog računa na koji je dodijeljena licenca.
- Da biste saznali postoje li poznati problemi sa servisom, pogledajte članak [Stranica o stanju servisa za Office 365](/office365/enterprise/view-service-health).
- Provjerite vatrozid, antivirusni softver i postavke proxyja da biste provjerili ne blokiraju li Microsoft 365 aplikacijama pristup internetu. Pogledajte [URL-ovi i rasponi IP adresa za Office 365](/office365/enterprise/urls-and-ip-address-ranges "URL-ovi i rasponi IP adresa za Office 365").

**Savjet** Na Windows uređajima možemo dijagnosticirati i automatski riješiti nekoliko uobičajenih problema Office za prijavu. Preuzmite i pokrenite **[Microsoftovu pomoćnik za podršku i oporavak da](https://aka.ms/SaRA-OfficeSignInScenario)** biste koristili naš automatizirani alat.

Primijenite sljedeće radnje uklanjanja poteškoća:

- Otvorite aplikaciju sustava Office i [odjavite se](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) s postojećih korisničkih računa. [Uklonite](/microsoft-365/admin/manage/remove-licenses-from-users) i [ponovno dodijelite](/microsoft-365/admin/manage/assign-licenses-to-users) licencu sustava Office, a zatim se [prijavite u Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) s pomoću zahvaćenog korisničkog računa.
- Pokrenite [alat za otklanjanje poteškoća s aktivacijom](https://aka.ms/SARA-OfficeActivation-Alchemy)
- [Resetirajte stanje aktivacije sustava Office](/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "Ponovno postavljanje Office aktivacijskog stanja")
- [Provedite internetski popravak sustava Office](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA)

Dodatne rješenja za otklanjanje poteškoća potražite u sljedećim člancima:  

- [Pogreške zbog nelicenciranog proizvoda i pogreške s aktivacijom u sustavu Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380?wt.mc_id=Alchemy_ClientDIA)
- [Pogreška „Nažalost, ne možemo se povezati s vašim računom. Pokušajte ponovo kasnije” prilikom aktivacije sustava Office](/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)