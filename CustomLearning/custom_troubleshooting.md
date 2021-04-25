---
author: pkrebs
ms.author: pkrebs
title: Microsoft 365 학습 경로 문제 해결
ms.date: 02/10/2019
description: Microsoft 365 학습 경로 문제 해결 방법 학습
ms.service: sharepoint-online
manager: bpardi
ms.topic: article
audience: admin
ms.openlocfilehash: 7190688d574042c8a1b8dfb67c8b246dfbf8c927
ms.sourcegitcommit: 97e175e5ff5b6a9e0274d5ec9b39fdf7e18eb387
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/25/2021
ms.locfileid: "52000304"
---
# <a name="troubleshoot-microsoft-365-learning-pathways"></a><span data-ttu-id="7fba8-103">Microsoft 365 학습 경로 문제 해결</span><span class="sxs-lookup"><span data-stu-id="7fba8-103">Troubleshoot Microsoft 365 learning pathways</span></span>

<span data-ttu-id="7fba8-104">다음은 Microsoft 365 학습 경로 또는 SharePoint Online 프로비전 서비스에서 발생할 수 있는 문제에 대한 문제 해결 팁입니다.</span><span class="sxs-lookup"><span data-stu-id="7fba8-104">Here are troubleshooting tips for problems that may occur with Microsoft 365 learning pathways or the SharePoint Online Provisioning Service.</span></span>

## <a name="how-to-know-if-you-have-tenant-admin-permissions"></a><span data-ttu-id="7fba8-105">테넌트 관리자 권한이 있는 경우를 아는 방법</span><span class="sxs-lookup"><span data-stu-id="7fba8-105">How to know if you have Tenant Admin permissions</span></span>

<span data-ttu-id="7fba8-106">SharePoint Online 프로비저닝 서비스에 로그인하고 사용자 지정 학습을 프로비저닝하려면 테넌트 관리자 권한이 필요합니다.</span><span class="sxs-lookup"><span data-stu-id="7fba8-106">Sign in to the SharePoint Online Provisioning Service and provisioning Custom Learning requires Tenant Admin permissions.</span></span> <span data-ttu-id="7fba8-107">SharePoint Online 프로비저닝 서비스에 로그인 문제가 발생하는 경우 전역 관리자 역할이 할당되어 있는지 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="7fba8-107">If you are experiencing sign in issues with the SharePoint Online Provisioning Service, make sure that you have been assigned the Global administrator role.</span></span> <span data-ttu-id="7fba8-108">사용자 지정 학습 솔루션에는 테넌트 관리자 권한이 필요합니다(그렇지 않으면 Office 365 전역 관리자 역할).</span><span class="sxs-lookup"><span data-stu-id="7fba8-108">The Custom Learning solution requires Tenant Admin permissions, otherwise known as Office 365 Global Administrator role.</span></span> <span data-ttu-id="7fba8-109">전역 관리자 역할이 할당되어 있는지 확인하는 방법에는 다음이 있습니다.</span><span class="sxs-lookup"><span data-stu-id="7fba8-109">Here’s how to determine if you have been assigned the Global Administrator role.</span></span>

1.  <span data-ttu-id="7fba8-110">로그인하여 Office.com.</span><span class="sxs-lookup"><span data-stu-id="7fba8-110">Sign in to Office.com.</span></span>
2.  <span data-ttu-id="7fba8-111">관리자를 **클릭합니다.**</span><span class="sxs-lookup"><span data-stu-id="7fba8-111">Click **Admin**</span></span>
3.  <span data-ttu-id="7fba8-112">사용자 **아래에서** 활성 **사용자를 선택합니다.**</span><span class="sxs-lookup"><span data-stu-id="7fba8-112">Under **Users**, select **Active Users**</span></span>
4.  <span data-ttu-id="7fba8-113">이름 검색</span><span class="sxs-lookup"><span data-stu-id="7fba8-113">Search for your name</span></span>
5.  <span data-ttu-id="7fba8-114">검색 결과에서 이름을 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="7fba8-114">Click your name in Search results.</span></span> <span data-ttu-id="7fba8-115">역할에 대한 전역 관리자가 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="7fba8-115">You should see Global administrator for your role.</span></span>
<span data-ttu-id="7fba8-116">![라이선스, 그룹 구성원 자격 및 기타 정보와 함께 역할을 나열하는 샘플 페이지입니다.](media/cg-globaladminrole.png)</span><span class="sxs-lookup"><span data-stu-id="7fba8-116">![Sample page that lists your role along with licenses, group memberships and other information.](media/cg-globaladminrole.png)</span></span>

### <a name="if-you-dont-have-the-global-administrator-role"></a><span data-ttu-id="7fba8-117">전역 관리자 역할이 없는 경우</span><span class="sxs-lookup"><span data-stu-id="7fba8-117">If you don’t have the Global administrator role</span></span>
- <span data-ttu-id="7fba8-118">조직에서 전역 관리자를 찾아 해당 사용자가 서비스에 로그인하게 하거나 사용자에게 전역 관리자 역할을 할당하게 합니다.</span><span class="sxs-lookup"><span data-stu-id="7fba8-118">Find a Global Administrator in your organization and have that person sign into the service or have them assign the Global administrator role to you.</span></span>

## <a name="tenant-app-catalog-troubleshooting"></a><span data-ttu-id="7fba8-119">테넌트 앱 카탈로그 문제 해결</span><span class="sxs-lookup"><span data-stu-id="7fba8-119">Tenant App Catalog Troubleshooting</span></span>
<span data-ttu-id="7fba8-120">사용자 지정 학습을 사용하려면 대상 테넌트에 앱 카탈로그를 프로비전해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="7fba8-120">Custom Learning requires an App Catalog to be provisioned in the target tenant.</span></span> <span data-ttu-id="7fba8-121">앱 카탈로그를 만들려면 전역 관리자 권한이 필요합니다.</span><span class="sxs-lookup"><span data-stu-id="7fba8-121">Creating an app catalog requires Global Administrator permissions.</span></span> <span data-ttu-id="7fba8-122">다음은 일반적인 앱 카탈로그 문제에 대한 문제 해결 단계입니다.</span><span class="sxs-lookup"><span data-stu-id="7fba8-122">Here’s are troubleshooting steps for common App Catalog issues:</span></span>

### <a name="how-to-know-if-you-have-a-tenant-app-catalog"></a><span data-ttu-id="7fba8-123">테넌트 앱 카탈로그가 있는지 아는 방법</span><span class="sxs-lookup"><span data-stu-id="7fba8-123">How to know if you have a Tenant app catalog</span></span> 
<span data-ttu-id="7fba8-124">먼저 전역 관리자 권한이 있는지 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="7fba8-124">For starters, ensure that you have Global administrator permissions.</span></span> <span data-ttu-id="7fba8-125">위의 테넌트 관리자 권한에 대한 단계를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="7fba8-125">See the steps for Tenant Admin permissions above.</span></span>

1. <span data-ttu-id="7fba8-126">Office 365에서 **관리자,** 확장 화살표 > 클릭하고 모든 관리 센터  >    >  **SharePoint 표시를 클릭합니다.**</span><span class="sxs-lookup"><span data-stu-id="7fba8-126">From Office 365, click **Admin**, click the expand arrow >, click **Show all** > **Admin centers** > **SharePoint**.</span></span>
2. <span data-ttu-id="7fba8-127">클래식 **관리자 SharePoint 센터 앱**  >  **앱** 카탈로그  >  **를 클릭합니다.**</span><span class="sxs-lookup"><span data-stu-id="7fba8-127">Click **Classic Admin SharePoint Center** > **apps** > **App Catalog**.</span></span>
3. <span data-ttu-id="7fba8-128">앱 **아래에** SharePoint용 앱 배포 제목의 **타일이 표시됩니다.**</span><span class="sxs-lookup"><span data-stu-id="7fba8-128">Under **Apps**, you should see a tile titled **Distribute apps for SharePoint**.</span></span> <span data-ttu-id="7fba8-129">타일이 표시되어 있는 경우 테넌트 앱 카탈로그가 있습니다.</span><span class="sxs-lookup"><span data-stu-id="7fba8-129">If you see the tile, you have a Tenant App Catalog.</span></span> <span data-ttu-id="7fba8-130">아래 **사이트 구성...** 섹션을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="7fba8-130">See the **How to ensure your are a Site Colllection...** section below.</span></span> <span data-ttu-id="7fba8-131">타일이 없는 경우 테넌트에 대한 테넌트 앱 카탈로그를 만들어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="7fba8-131">If you don’t see the tile you will need to create a tenant app catalog for your tenant.</span></span> <span data-ttu-id="7fba8-132">아래 테넌트 앱 **카탈로그를 만드는** 방법 섹션을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="7fba8-132">See the **How to create a Tenant App Catalog** section below .</span></span>

### <a name="how-to-ensure-you-are-a-site-collection-owner-on-the-tenant-app-catalog"></a><span data-ttu-id="7fba8-133">테넌트 앱 카탈로그에서 사이트 모음 소유자가 되도록 하는 방법</span><span class="sxs-lookup"><span data-stu-id="7fba8-133">How to ensure you are a Site Collection Owner on the Tenant App Catalog</span></span> 
<span data-ttu-id="7fba8-134">Microsoft 365 학습 경로를 프로비저닝하려면 테넌트 앱 카탈로그의 사이트 모음 소유자가 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="7fba8-134">To provision Microsoft 365 learning pathways, you will need to be a Site Collection Owner on the Tenant App Catalog.</span></span> <span data-ttu-id="7fba8-135">소유자인지 확인하는 방법에는 다음이 있습니다.</span><span class="sxs-lookup"><span data-stu-id="7fba8-135">Here’s how to determine if you are an Owner.</span></span>

1. <span data-ttu-id="7fba8-136">Office 365에서 **관리자,** 확장 화살표 > 클릭하고 모든 관리 센터  >    >  **SharePoint 표시를 클릭합니다.**</span><span class="sxs-lookup"><span data-stu-id="7fba8-136">From Office 365, click **Admin**, click the expand arrow >, click **Show all** > **Admin centers** > **SharePoint**.</span></span>
2. <span data-ttu-id="7fba8-137">클래식 **관리 SharePoint 센터를 클릭한** 다음 앱 카탈로그 **를 선택합니다.**</span><span class="sxs-lookup"><span data-stu-id="7fba8-137">Click **Classic Admin SharePoint Center**, and then select the **app catalog**.</span></span>
3. <span data-ttu-id="7fba8-138">소유자 **를** 선택한 다음 사이트 모음 소유자가 되도록 합니다.</span><span class="sxs-lookup"><span data-stu-id="7fba8-138">Select **Owner**, and then ensure you are a Site Collection Owner.</span></span> <span data-ttu-id="7fba8-139">모양은 다음과 같아야 합니다.</span><span class="sxs-lookup"><span data-stu-id="7fba8-139">It should look something like this.</span></span>
<span data-ttu-id="7fba8-140">![관리자 관리 페이지.](media/cg-sitecollectionowner.png)</span><span class="sxs-lookup"><span data-stu-id="7fba8-140">![Manage administrators page.](media/cg-sitecollectionowner.png)</span></span>

### <a name="how-to-create-a-tenant-app-catalog-if-one-doesnt-exists"></a><span data-ttu-id="7fba8-141">없는 경우 테넌트 앱 카탈로그를 만드는 방법</span><span class="sxs-lookup"><span data-stu-id="7fba8-141">How to create a Tenant App Catalog if one doesn’t exists</span></span> 
1. <span data-ttu-id="7fba8-142">SharePoint Online 관리자 계정으로 Office 365에 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="7fba8-142">Sign in to Office 365 with your SharePoint Online admin account.</span></span>
2. <span data-ttu-id="7fba8-143">**관리자** 를 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="7fba8-143">Click **Admin**.</span></span>
3. <span data-ttu-id="7fba8-144">관리 **센터에서** **SharePoint 를 클릭합니다.**</span><span class="sxs-lookup"><span data-stu-id="7fba8-144">Under **Admin centers**, click **SharePoint**.</span></span> 
4. <span data-ttu-id="7fba8-145">앱 **앱 카탈로그**  >  **를 클릭합니다.**</span><span class="sxs-lookup"><span data-stu-id="7fba8-145">Click **Apps** > **App Catalog**.</span></span>
5. <span data-ttu-id="7fba8-146">새 **앱 카탈로그 사이트 만들기를 클릭한** 다음 확인 을 **클릭합니다.**</span><span class="sxs-lookup"><span data-stu-id="7fba8-146">Click **Create a new app catalog site**, and then click **OK**.</span></span> 
6.  <span data-ttu-id="7fba8-147">앱 카탈로그에 대한 정보를 입력합니다.</span><span class="sxs-lookup"><span data-stu-id="7fba8-147">Enter the information for the App Catalog.</span></span> <span data-ttu-id="7fba8-148">관리자를 두 개 이상 포함할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="7fba8-148">You may want to include more than one Administrator.</span></span> <span data-ttu-id="7fba8-149">다음은 예를 보여 주는 예제입니다.</span><span class="sxs-lookup"><span data-stu-id="7fba8-149">The following shows an example.</span></span>  
![새 앱 카탈로그에 대한 정보를 입력할 양식입니다.](media/cg-appcatalogfinish.png)

7.  <span data-ttu-id="7fba8-151">그거에요.</span><span class="sxs-lookup"><span data-stu-id="7fba8-151">That’s it.</span></span> <span data-ttu-id="7fba8-152">완료한 것입니다.</span><span class="sxs-lookup"><span data-stu-id="7fba8-152">You’re done.</span></span> <span data-ttu-id="7fba8-153">그러나 프로비저닝 사용자 지정 학습으로 이동하기 전에 앱 카탈로그 만들기가 완료될 때까지 30분 이상 기다려야 합니다.</span><span class="sxs-lookup"><span data-stu-id="7fba8-153">But before you move to provisioning Custom Learning, you need to wait at least 30 minutes to make sure the App Catalog creation is complete.</span></span> 

> [!IMPORTANT]
> <span data-ttu-id="7fba8-154">사용자 지정 학습을 프로비저닝하기 전에 테넌트 앱 카탈로그를 만들고 30분 이상 기다립니다.</span><span class="sxs-lookup"><span data-stu-id="7fba8-154">Wait at least 30 minutes after creating the Tenant App Catalog before provisioning Custom Learning.</span></span> <span data-ttu-id="7fba8-155">이렇게 하면 SharePoint 내에서 앱 카탈로그 프로비저닝 프로세스가 완료됩니다.</span><span class="sxs-lookup"><span data-stu-id="7fba8-155">This ensures that the App Catalog provisioning process is complete within SharePoint.</span></span> 