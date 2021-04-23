---
title: Pravila zadržavanja u centru za administratore sustava Exchange ne rade
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: bb2ce7ce2405be575dfdb79d304fef690e863a4e
ms.sourcegitcommit: e9206b7bb1bf2efd2471edbf4c60c00c3607bc41
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2021
ms.locfileid: "51952220"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="6e290-102">Pravila zadržavanja u centru za administratore sustava Exchange</span><span class="sxs-lookup"><span data-stu-id="6e290-102">Retention Policies in Exchange Admin Center</span></span>

<span data-ttu-id="6e290-103">Ako želite da pokrenemo automatske provjere postavki navedenih u nastavku, odaberite gumb natrag <– pri vrhu ove stranice, a zatim unesite adresu e-pošte korisnika koji ima problema s pravilima zadržavanja.</span><span class="sxs-lookup"><span data-stu-id="6e290-103">If you want us to run automated checks for the settings mentioned below, select the back button <-- at the top of this page, and then enter the email address of the user who has problems with retention policies.</span></span>

<span data-ttu-id="6e290-104">Ako imate problema s pravilima zadržavanja u centru za administratore sustava Exchange koji se ne primjenjuju na poštanske sandučiće ili stavke koje se ne premještaju u arhivski poštanski sandučić, provjerite sljedeće:</span><span class="sxs-lookup"><span data-stu-id="6e290-104">If you have problems with retention policies in the Exchange Admin Center not applying to mailboxes or items not moving to the archive mailbox, check the following:</span></span>

<span data-ttu-id="6e290-105">**Korijenski uzroci:**</span><span class="sxs-lookup"><span data-stu-id="6e290-105">**Root Causes:**</span></span>

- <span data-ttu-id="6e290-106">**Pomoćnik za upravljane** mape nije obradio korisnikov poštanski sandučić.</span><span class="sxs-lookup"><span data-stu-id="6e290-106">**Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="6e290-107">Pomoćnik za upravljane mape pokušava obraditi svaki poštanski sandučić u tvrtki ili ustanovi u oblaku jedanput svakih sedam dana.</span><span class="sxs-lookup"><span data-stu-id="6e290-107">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span>

  <span data-ttu-id="6e290-108">**Rješenje:** Pokrenite pomoćnik za upravljane mape.</span><span class="sxs-lookup"><span data-stu-id="6e290-108">**Solution:** Run the Managed Folder Assistant.</span></span>

- <span data-ttu-id="6e290-109">**ZadržavanjeDržanje** je **omogućeno u** poštanskom sandučiću.</span><span class="sxs-lookup"><span data-stu-id="6e290-109">**RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="6e290-110">Ako je poštanski sandučić postavljen na čuvanje, pravilnik o zadržavanju u poštanskom sandučiću neće se obraditi tijekom tog razdoblja.</span><span class="sxs-lookup"><span data-stu-id="6e290-110">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span>

  <span data-ttu-id="6e290-111">**Rješenje:** Provjerite status postavke čuvanja zadržavanja i ažurirajte po potrebi.</span><span class="sxs-lookup"><span data-stu-id="6e290-111">**Solution:** Check status of Retention Hold setting and update as needed.</span></span> <span data-ttu-id="6e290-112">Detalje potražite u članku Čuvanje [zadržavanja poštanskog sandučića](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span><span class="sxs-lookup"><span data-stu-id="6e290-112">For details, see [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
 
<span data-ttu-id="6e290-113">**Napomena:** Ako je poštanski sandučić manji od 10 MB, pomoćnik za upravljane mape neće automatski obraditi poštanski sandučić.</span><span class="sxs-lookup"><span data-stu-id="6e290-113">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span>
 
<span data-ttu-id="6e290-114">Dodatne informacije o pravilima zadržavanja u centru za administratore sustava Exchange potražite u članku:</span><span class="sxs-lookup"><span data-stu-id="6e290-114">For more info on retention policies in the Exchange Admin Center, see:</span></span>

- [<span data-ttu-id="6e290-115">Oznake zadržavanja i pravilniki o zadržavanju</span><span class="sxs-lookup"><span data-stu-id="6e290-115">Retention tags and retention policies</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)

- <span data-ttu-id="6e290-116">[Primjena pravilnika o zadržavanju na poštanske sandučiće](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) [ili Dodavanje ili uklanjanje oznaka zadržavanja](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)</span><span class="sxs-lookup"><span data-stu-id="6e290-116">[Apply a retention policy to mailboxes](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) or [Add or remove retention tags](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)</span></span>

- [<span data-ttu-id="6e290-117">Kako prepoznati vrstu zadržavanja koja se nalazi na poštanskom sandučiću</span><span class="sxs-lookup"><span data-stu-id="6e290-117">How to identify the type of hold placed on a mailbox</span></span>](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
