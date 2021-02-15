---
title: Lozinka writeback ne funkcionira
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
- "9004595"
- "8210"
ms.openlocfilehash: d7766f908f025b5db8299aa45d01dc5389b321ec
ms.sourcegitcommit: 2f39850ac0fba9fbeba9b8b7939ae79b505d3b67
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 02/12/2021
ms.locfileid: "50243247"
---
# <a name="password-writeback-is-not-working"></a><span data-ttu-id="0a351-102">Lozinka writeback ne funkcionira</span><span class="sxs-lookup"><span data-stu-id="0a351-102">Password Writeback is not working</span></span>

<span data-ttu-id="0a351-103">**Imam problema s konfiguriranjem lozinke za nepotvrđenim**</span><span class="sxs-lookup"><span data-stu-id="0a351-103">**I'm having problems configuring password writeback**</span></span>

- <span data-ttu-id="0a351-104">Lozinka nepotvrđenim je Premium značajka.</span><span class="sxs-lookup"><span data-stu-id="0a351-104">Password writeback is a premium feature.</span></span>
- <span data-ttu-id="0a351-105">Provjerite jeste li razumjeli preduvjete za licenciranje:</span><span class="sxs-lookup"><span data-stu-id="0a351-105">Make sure that you understand the licensing requirements:</span></span>
  - <span data-ttu-id="0a351-106">U vašoj tvrtki ili ustanovi mora biti dodijeljena najmanje jedna licenca</span><span class="sxs-lookup"><span data-stu-id="0a351-106">You must have at least one license assigned in your organization</span></span>
  - <span data-ttu-id="0a351-107">**Samo oblak korisnici** -bilo koji Office 365 (O365) Paid SKU ili Azure ad Basic</span><span class="sxs-lookup"><span data-stu-id="0a351-107">**Cloud only users** - Any Office 365 (O365) paid SKU, or Azure AD Basic</span></span>
  - <span data-ttu-id="0a351-108">**Cloud i/ili lokalni korisnici** -Azure ad Premium P1 ili P2, Enterprise Mobility + Security (EMS) ili Secure produktivnost Enterprise (SPE)</span><span class="sxs-lookup"><span data-stu-id="0a351-108">**Cloud and/or on-premises users** - Azure AD Premium P1 or P2, Enterprise Mobility + Security (EMS), or Secure Productive Enterprise (SPE)</span></span>
    - <span data-ttu-id="0a351-109">Dodatne informacije o preduvjetima za licenciranje potražite u članku [Licencne preduvjete za ponovno postavljanje lozinke za Azure ad samoservisiranja](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)</span><span class="sxs-lookup"><span data-stu-id="0a351-109">To learn more about licensing requirements, see [Licensing requirements for Azure AD self-service password reset](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)</span></span>
- <span data-ttu-id="0a351-110">Imate najmanje jedan administratorski račun i jedan test korisnički račun s jednom od odgovarajućih licenci.</span><span class="sxs-lookup"><span data-stu-id="0a351-110">You have at least one administrator account and one test user account with one of the appropriate license.</span></span>
- <span data-ttu-id="0a351-111">Morate povezati Azure ad Connect s primarnom kontrolorom domene na kojoj je lozinka nepotvrđenim na posao.</span><span class="sxs-lookup"><span data-stu-id="0a351-111">You must connect Azure AD Connect to the Primary Domain Controller Emulator for password writeback to work.</span></span> <span data-ttu-id="0a351-112">Možete konfigurirati Azure AD Connect da biste koristili primarni kontroler domene tako da desnom tipkom miša kliknete **Svojstva** sinkronizacijskog konektora servisa Active Directory, a zatim odaberete **Konfiguriranje particija direktorija**.</span><span class="sxs-lookup"><span data-stu-id="0a351-112">You can configure Azure AD Connect to use a Primary Domain Controller by right clicking on the **properties** of the Active Directory synchronization connector, then selecting **configure directory partitions**.</span></span> <span data-ttu-id="0a351-113">Odatle potražite odjeljak **Postavke veze s kontrolerom domene** , a zatim potvrdite okvir **samo koristi preferirani kontroleri domena**.</span><span class="sxs-lookup"><span data-stu-id="0a351-113">From there, look for the **domain controller connection settings** section and check the box titled **only use preferred domain controllers**.</span></span>
  > [!NOTE]
  > <span data-ttu-id="0a351-114">Ako preferirani DC nije PDC emulator, Azure AD Connect i dalje će doći do PDC-a za lozinku writeback.</span><span class="sxs-lookup"><span data-stu-id="0a351-114">If the preferred DC is not a PDC emulator, Azure AD Connect will still reach out to the PDC for password writeback.</span></span>
- <span data-ttu-id="0a351-115">Ponovno postavljanje lozinke konfigurirano je i omogućeno u vašem zakupcu.</span><span class="sxs-lookup"><span data-stu-id="0a351-115">Password reset has been configured and enabled in your tenant.</span></span> <span data-ttu-id="0a351-116">Dodatne informacije potražite u članku [Omogućivanje ponovnog vraćanja lozinki za Azure ad](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started).</span><span class="sxs-lookup"><span data-stu-id="0a351-116">For more information, see [Enable users to reset their Azure AD passwords](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started).</span></span>
- <span data-ttu-id="0a351-117">Provjerite je li administratorski račun koji se koristi za omogućivanje lozinke writeback račun administratora oblaka (stvoren u servisu Azure AD nije lokalni oglas)</span><span class="sxs-lookup"><span data-stu-id="0a351-117">Make sure that the administrator account being used to enable Password Writeback is a cloud administrator account (created in Azure AD not on-premises AD)</span></span>
- <span data-ttu-id="0a351-118">Imate jednu ili više-šumsku web-lokalnu implementaciju sa sustavom Windows Server 2008 R2, Windows Server 2012 ili Windows Server 2012 R2 s instaliranim najnovijim servisnim paketima</span><span class="sxs-lookup"><span data-stu-id="0a351-118">You have a single or multi-forest AD on-premises deployment running Windows Server 2008 R2, Windows Server 2012, or Windows Server 2012 R2 with the latest service packs installed</span></span>
- <span data-ttu-id="0a351-119">Imate instaliran alat Azure AD Connect i pripremili ste svoj oglasni ambijent za sinkronizaciju u oblak.</span><span class="sxs-lookup"><span data-stu-id="0a351-119">You have the Azure AD Connect tool installed and you have prepared your AD environment for synchronization to the cloud.</span></span> <span data-ttu-id="0a351-120">Prije testiranja lozinke writeback, provjerite jeste li prvi put dovršili kompletnu uvoz i potpunu sinkronizaciju iz oglasa i Azure ad u servisu Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="0a351-120">Before testing password writeback, make sure that you first complete a full import and full sync from both AD and Azure AD in Azure AD Connect.</span></span>
- <span data-ttu-id="0a351-121">Dodatne informacije potražite u članku [potpuna sinkronizacija i puni uvoz u servisu Azure ad Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)</span><span class="sxs-lookup"><span data-stu-id="0a351-121">To learn more, see how to do a [full sync and full import in Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)</span></span>

<span data-ttu-id="0a351-122">**Imam problema s vezom za lozinku nepotvrđenim**</span><span class="sxs-lookup"><span data-stu-id="0a351-122">**I'm having a problem with password writeback connectivity**</span></span>

1. <span data-ttu-id="0a351-123">Preuzimanje i Omogućivanje najnovije verzije servisa [Azure ad Connect](https://www.microsoft.com/download/details.aspx?id=47594)</span><span class="sxs-lookup"><span data-stu-id="0a351-123">Download and enable the latest version of [Azure AD Connect](https://www.microsoft.com/download/details.aspx?id=47594)</span></span>
2. <span data-ttu-id="0a351-124">Konfiguracija vatrozida: alat za Azure AD Connect (1.1.443 i noviji) Trebat će **Izlazni https** pristup:</span><span class="sxs-lookup"><span data-stu-id="0a351-124">Firewall configuration: The Azure AD Connect tool (1.1.443 and above) will need **outbound HTTPS** access to:</span></span>
    - <span data-ttu-id="0a351-125">passwordreset.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="0a351-125">passwordreset.microsoftonline.com</span></span>
    - <span data-ttu-id="0a351-126">servicebus. Windows. Networks</span><span class="sxs-lookup"><span data-stu-id="0a351-126">servicebus.windows.networks</span></span>
3. <span data-ttu-id="0a351-127">Dopuštanje mirovanja veza koje traju najmanje 2-3 minuta</span><span class="sxs-lookup"><span data-stu-id="0a351-127">Allow idle connections to persist for at least 2-3 minutes</span></span>

<span data-ttu-id="0a351-128">**I dalje imam problema s lozinkom nepotvrđenim**</span><span class="sxs-lookup"><span data-stu-id="0a351-128">**I'm still having problems with password writeback**</span></span>

- <span data-ttu-id="0a351-129">Ako i dalje imate poteškoća, pokušajte onemogućiti i ponovno omogućiti servis za lozinku nepotvrđenim u alatu za Azure ad Connect</span><span class="sxs-lookup"><span data-stu-id="0a351-129">If you are still having difficulty, try disabling and re-enabling the password writeback service in the Azure AD Connect tool</span></span>
- <span data-ttu-id="0a351-130">Dodatne informacije potražite u članku [onemogućivanje i ponovno omogućivanje lozinke za nepotvrđenim](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)</span><span class="sxs-lookup"><span data-stu-id="0a351-130">To learn more, see how to [disable and re-enable password writeback](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)</span></span>
