---
title: Omogućivanje pristupa korisnicima sustava SharePoint i servisu OneDrive
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: a7e9c0b7ffa5c11a2e24ee5fda6491f049f985f1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47677199"
---
# <a name="give-users-access-to-sharepoint-and-onedrive"></a><span data-ttu-id="8b5b1-102">Omogućivanje pristupa korisnicima sustava SharePoint i servisu OneDrive</span><span class="sxs-lookup"><span data-stu-id="8b5b1-102">Give users access to SharePoint and OneDrive</span></span>

> [!NOTE]
> <span data-ttu-id="8b5b1-103">Ako web-mjesto servisa OneDrive ili SharePoint nije dostupno većem broju korisnika koji su prethodno imali pristup, možda postoji privremeni problem s servisom.</span><span class="sxs-lookup"><span data-stu-id="8b5b1-103">If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> [<span data-ttu-id="8b5b1-104">Provjerite nadzornu ploču zdravstvenog stanja servisa</span><span class="sxs-lookup"><span data-stu-id="8b5b1-104">Check the service health dashboard</span></span>](https://portal.office.com/adminportal/home#/servicehealth)
  
<span data-ttu-id="8b5b1-105">Ako želite da se osobe u tvrtki ili ustanovi mogu prijaviti i koristiti SharePoint i OneDrive, morate im dodati račune i provjeriti imaju li licencu koja im omogućuje pristup sustavu SharePoint i servisu OneDrive.</span><span class="sxs-lookup"><span data-stu-id="8b5b1-105">If you want people in your organization to be able to sign in and use SharePoint and OneDrive, you need to add accounts for them and make sure they have a license that gives them access to SharePoint and OneDrive.</span></span> <span data-ttu-id="8b5b1-106">U centru za administratore sustava Microsoft 365 najjednostavniji je način dodavanja korisnika.</span><span class="sxs-lookup"><span data-stu-id="8b5b1-106">The easiest way to add users is in the Microsoft 365 admin center.</span></span>
  
1. <span data-ttu-id="8b5b1-107">Otvorite [stranicu aktivni korisnici u centru za administratore sustava Microsoft 365](https://portal.office.com/adminportal/home#/users), a zatim kliknite **Dodaj korisnika**.</span><span class="sxs-lookup"><span data-stu-id="8b5b1-107">Go to the [Active users page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/users), and then click **Add a user**.</span></span>
    
2. <span data-ttu-id="8b5b1-108">Unesite podatke za korisnika i provjerite je li u odjeljku **licence za proizvode**dodijeljena licenca, a odabrana je **SharePoint Online** .</span><span class="sxs-lookup"><span data-stu-id="8b5b1-108">Fill in the information for the user, and make sure that under **Product licenses**, a license is assigned and **SharePoint Online** is selected.</span></span> 
    
<span data-ttu-id="8b5b1-109">Imajte na glavi da ako dopuštate vanjsko zajedničko korištenje u tvrtki ili ustanovi, korisnici mogu zajednički koristiti sadržaj sustava SharePoint i OneDrive s osobama izvan tvrtke ili ustanove.</span><span class="sxs-lookup"><span data-stu-id="8b5b1-109">Note that if you allow external sharing in your organization, users can share SharePoint and OneDrive content with people outside the organization.</span></span> <span data-ttu-id="8b5b1-110">Ne morate davati licencama tih vanjskih korisnika.</span><span class="sxs-lookup"><span data-stu-id="8b5b1-110">You don't need to give these external users licenses.</span></span> <span data-ttu-id="8b5b1-111">Ne morate ni dodavati račune za njih, osim ako zajedničko korištenje nije postavljeno na "samo postojeći vanjski korisnici".</span><span class="sxs-lookup"><span data-stu-id="8b5b1-111">You also don't need to add accounts for them, unless sharing is set to "Only existing external users."</span></span> <span data-ttu-id="8b5b1-112">U tom slučaju, ako osobe nisu u direktoriju vaše tvrtke ili ustanove, morate ih dodati kao goste u centru za administratore servisa Azure AD.</span><span class="sxs-lookup"><span data-stu-id="8b5b1-112">In that case, if the people aren't in your organization's directory, you need to add them as guest users in the Azure AD admin center.</span></span>
  

