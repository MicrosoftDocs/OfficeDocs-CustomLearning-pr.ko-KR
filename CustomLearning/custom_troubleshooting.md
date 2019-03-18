---
author: pkrebs
ms.author: pkrebs
title: 사용자 지정 학습 문제 해결
ms.date: 02/10/2019
description: 사용자 지정 학습 문제를 해결 하는 방법 알아보기
ms.openlocfilehash: 7cbd049d4794d14f9e8cc26fd0db5f444812d688
ms.sourcegitcommit: 64721b7763d988d3b669eeab26fdb8b677ddc486
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/17/2019
ms.locfileid: "30658225"
---
# <a name="troubleshoot-custom-learning"></a><span data-ttu-id="a95cf-103">사용자 지정 학습 문제 해결</span><span class="sxs-lookup"><span data-stu-id="a95cf-103">Troubleshoot Custom Learning</span></span>

<span data-ttu-id="a95cf-104">다음은 Office 365 또는 SharePoint Online 프로 비전 서비스에 대 한 사용자 지정 학습에서 발생할 수 있는 문제에 대 한 문제 해결 팁입니다.</span><span class="sxs-lookup"><span data-stu-id="a95cf-104">Here are troubleshooting tips for problems that may occur with Custom Learning for Office 365 or the SharePoint Online Provisioning Service.</span></span>

## <a name="how-to-know-if-you-have-tenant-admin-permissions"></a><span data-ttu-id="a95cf-105">테 넌 트 관리 권한이 있는지 확인 하는 방법</span><span class="sxs-lookup"><span data-stu-id="a95cf-105">How to know if you have Tenant Admin permissions</span></span>

<span data-ttu-id="a95cf-106">SharePoint Online 프로 비전 서비스에 로그인 하 고 사용자 지정 학습용 프로 비전에는 테 넌 트 관리자 권한이 필요 합니다.</span><span class="sxs-lookup"><span data-stu-id="a95cf-106">Sign in to the SharePoint Online Provisioning Service and provisioning Custom Learning requires Tenant Admin permissions.</span></span> <span data-ttu-id="a95cf-107">SharePoint Online 프로 비전 서비스에 로그인 하는 동안 문제가 발생 하는 경우 전역 관리자 역할이 할당 되었는지 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="a95cf-107">If you are experiencing sign in issues with the SharePoint Online Provisioning Service, make sure that you have been assigned the Global administrator role.</span></span> <span data-ttu-id="a95cf-108">사용자 지정 학습 솔루션에는 테 넌 트 관리 권한 (Office 365 전역 관리자 역할 이라고 함)이 필요 합니다.</span><span class="sxs-lookup"><span data-stu-id="a95cf-108">The Custom Learning solution requires Tenant Admin permissions, otherwise known as Office 365 Global Administrator role.</span></span> <span data-ttu-id="a95cf-109">전역 관리자 역할이 할당 되었는지 확인 하는 방법은 다음과 같습니다.</span><span class="sxs-lookup"><span data-stu-id="a95cf-109">Here’s how to determine if you have been assigned the Global Administrator role.</span></span>

1.  <span data-ttu-id="a95cf-110">Office.com에 로그인 합니다.</span><span class="sxs-lookup"><span data-stu-id="a95cf-110">Sign in to Office.com.</span></span>
2.  <span data-ttu-id="a95cf-111">**관리** 클릭</span><span class="sxs-lookup"><span data-stu-id="a95cf-111">Click **Admin**</span></span>
3.  <span data-ttu-id="a95cf-112">**사용자**에서 **활성 사용자** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="a95cf-112">Under **Users**, select **Active Users**</span></span>
4.  <span data-ttu-id="a95cf-113">사용자 이름 검색</span><span class="sxs-lookup"><span data-stu-id="a95cf-113">Search for your name</span></span>
5.  <span data-ttu-id="a95cf-114">검색 결과에서 사용자의 이름을 클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="a95cf-114">Click your name in Search results.</span></span> <span data-ttu-id="a95cf-115">전역 관리자가 역할에 대 한 것을 볼 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="a95cf-115">You should see Global administrator for your role.</span></span>

![cg-globaladminrole-.png](media/cg-globaladminrole.png)

### <a name="if-you-dont-have-the-global-administrator-role"></a><span data-ttu-id="a95cf-117">전역 관리자 역할이 없는 경우</span><span class="sxs-lookup"><span data-stu-id="a95cf-117">If you don’t have the Global administrator role</span></span>
- <span data-ttu-id="a95cf-118">조직에서 전역 관리자를 찾아서 해당 사용자가 서비스에 로그인 하거나 전역 관리자 역할을 할당 하도록 합니다.</span><span class="sxs-lookup"><span data-stu-id="a95cf-118">Find a Global Administrator in your organization and have that person sign into the service or have them assign the Global administrator role to you.</span></span>

## <a name="tenant-app-catalog-troubleshooting"></a><span data-ttu-id="a95cf-119">테 넌 트 앱 카탈로그 문제 해결</span><span class="sxs-lookup"><span data-stu-id="a95cf-119">Tenant App Catalog Troubleshooting</span></span>
<span data-ttu-id="a95cf-120">사용자 지정 학습을 수행 하려면 대상 테 넌 트에서 앱 카탈로그를 프로 비전 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="a95cf-120">Custom Learning requires an App Catalog to be provisioned in the target tenant.</span></span> <span data-ttu-id="a95cf-121">앱 카탈로그를 만들려면 전역 관리자 권한이 필요 합니다.</span><span class="sxs-lookup"><span data-stu-id="a95cf-121">Creating an app catalog requires Global Administrator permissions.</span></span> <span data-ttu-id="a95cf-122">다음은 일반적인 앱 카탈로그 문제에 대 한 문제 해결 단계입니다.</span><span class="sxs-lookup"><span data-stu-id="a95cf-122">Here’s are troubleshooting steps for common App Catalog issues:</span></span>

### <a name="how-to-know-if-you-have-a-tenant-app-catalog"></a><span data-ttu-id="a95cf-123">테 넌 트 앱 카탈로그가 있는지 여부를 확인 하는 방법</span><span class="sxs-lookup"><span data-stu-id="a95cf-123">How to know if you have a Tenant app catalog</span></span> 
<span data-ttu-id="a95cf-124">초보자에 게 전역 관리자 권한이 있는지 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="a95cf-124">For starters, ensure that you have Global administrator permissions.</span></span> <span data-ttu-id="a95cf-125">위의 테 넌 트 관리 권한 단계를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="a95cf-125">See the steps for Tenant Admin permissions above.</span></span>

1. <span data-ttu-id="a95cf-126">Office 365에서 **관리**, 확장 화살표 >를 차례로 클릭 하 고 **모든** > **관리 센터** > **SharePoint**표시를 클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="a95cf-126">From Office 365, click **Admin**, click the expand arrow >, click **Show all** > **Admin centers** > **SharePoint**.</span></span>
2. <span data-ttu-id="a95cf-127">**클래식 관리 SharePoint Center** > **apps** > **앱 카탈로그**를 클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="a95cf-127">Click **Classic Admin SharePoint Center** > **apps** > **App Catalog**.</span></span>
3. <span data-ttu-id="a95cf-128">**앱**에는 **SharePoint 용 앱 배포**라는 타일이 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="a95cf-128">Under **Apps**, you should see a tile titled **Distribute apps for SharePoint**.</span></span> <span data-ttu-id="a95cf-129">타일이 표시 되 면 테 넌 트 앱 카탈로그가 있습니다.</span><span class="sxs-lookup"><span data-stu-id="a95cf-129">If you see the tile, you have a Tenant App Catalog.</span></span> <span data-ttu-id="a95cf-130">아래에서 **사이트 Colllection를 확인 하는 방법을** 참조 하십시오.</span><span class="sxs-lookup"><span data-stu-id="a95cf-130">See the **How to ensure your are a Site Colllection...** section below.</span></span> <span data-ttu-id="a95cf-131">타일이 표시 되지 않는 경우 테 넌 트에 대 한 테 넌 트 앱 카탈로그를 만들어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="a95cf-131">If you don’t see the tile you will need to create a tenant app catalog for your tenant.</span></span> <span data-ttu-id="a95cf-132">아래에서 **테 넌 트 앱 카탈로그를 만드는 방법** 섹션을 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="a95cf-132">See the **How to create a Tenant App Catalog** section below .</span></span>

### <a name="how-to-ensure-you-are-a-site-collection-owner-on-the-tenant-app-catalog"></a><span data-ttu-id="a95cf-133">사용자가 테 넌 트 앱 카탈로그의 사이트 모음 소유자 인지 확인 하는 방법</span><span class="sxs-lookup"><span data-stu-id="a95cf-133">How to ensure you are a Site Collection Owner on the Tenant App Catalog</span></span> 
<span data-ttu-id="a95cf-134">Office 365에 대 한 사용자 지정 학습을 프로 비전 하려면 테 넌 트 앱 카탈로그의 사이트 모음 소유자 여야 합니다.</span><span class="sxs-lookup"><span data-stu-id="a95cf-134">To provision Custom Learning for Office 365, you will need to be a Site Collection Owner on the Tenant App Catalog.</span></span> <span data-ttu-id="a95cf-135">소유자 인 경우에는 다음과 같은 방법으로 determin.</span><span class="sxs-lookup"><span data-stu-id="a95cf-135">Here’s how to determin if you are an Owner.</span></span>

1. <span data-ttu-id="a95cf-136">Office 365에서 **관리**, 확장 화살표 >를 차례로 클릭 하 고 **모든** > **관리 센터** > **SharePoint**표시를 클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="a95cf-136">From Office 365, click **Admin**, click the expand arrow >, click **Show all** > **Admin centers** > **SharePoint**.</span></span>
2. <span data-ttu-id="a95cf-137">**클래식 관리 SharePoint 센터**를 클릭 하 고 **앱 카탈로그**를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="a95cf-137">Click **Classic Admin SharePoint Center**, and then select the **app catalog**.</span></span>
3. <span data-ttu-id="a95cf-138">**소유자**를 선택 하 고 사용자가 사이트 모음 소유자 인지 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="a95cf-138">Select **Owner**, and then ensure you are a Site Collection Owner.</span></span> <span data-ttu-id="a95cf-139">다음과 같이 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="a95cf-139">It should look something like this.</span></span>
 
![cg-sitecollectionowner-.png](media/cg-sitecollectionowner.png)

### <a name="how-to-create-a-tenant-app-catalog-if-one-doesnt-exists"></a><span data-ttu-id="a95cf-141">테 넌 트 앱 카탈로그가 없는 경우 만드는 방법</span><span class="sxs-lookup"><span data-stu-id="a95cf-141">How to create a Tenant App Catalog if one doesn’t exists</span></span> 
1. <span data-ttu-id="a95cf-142">SharePoint Online 관리자 계정을 사용 하 여 Office 365에 로그인 합니다.</span><span class="sxs-lookup"><span data-stu-id="a95cf-142">Sign in to Office 365 with your SharePoint Online admin account.</span></span>
2. <span data-ttu-id="a95cf-143">**관리자**를 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="a95cf-143">Click **Admin**.</span></span>
3. <span data-ttu-id="a95cf-144">**관리 센터**에서 **SharePoint**를 클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="a95cf-144">Under **Admin centers**, click **SharePoint**.</span></span> 
4. <span data-ttu-id="a95cf-145">**앱** > **앱 카탈로그**를 클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="a95cf-145">Click **Apps** > **App Catalog**.</span></span>
5. <span data-ttu-id="a95cf-146">**새 앱 카탈로그 사이트 만들기**를 클릭 한 다음 **확인**을 클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="a95cf-146">Click **Create a new app catalog site**, and then click **OK**.</span></span> 
6.  <span data-ttu-id="a95cf-147">앱 카탈로그에 대 한 정보를 입력 합니다.</span><span class="sxs-lookup"><span data-stu-id="a95cf-147">Enter the information for the App Catalog.</span></span> <span data-ttu-id="a95cf-148">관리자를 두 명 이상 포함할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="a95cf-148">You may want to include more than one Administrator.</span></span> <span data-ttu-id="a95cf-149">다음은 예제를 보여 줍니다.</span><span class="sxs-lookup"><span data-stu-id="a95cf-149">The following shows an example.</span></span>  

![cg-appcatalogfinish-.png](media/cg-appcatalogfinish.png)

7.  <span data-ttu-id="a95cf-151">그거에요.</span><span class="sxs-lookup"><span data-stu-id="a95cf-151">That’s it.</span></span> <span data-ttu-id="a95cf-152">완료 되었습니다.</span><span class="sxs-lookup"><span data-stu-id="a95cf-152">You’re done.</span></span> <span data-ttu-id="a95cf-153">하지만 사용자 지정 학습 프로 비전으로 이동 하기 전에 30 분 이상 기다려야 앱 카탈로그 만들기가 완료 되었는지 확인 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="a95cf-153">But before you move to provisioning Custom Learning, you need to wait at least 30 minutes to make sure the App Catalog creation is complete.</span></span> 

> [!IMPORTANT]
> <span data-ttu-id="a95cf-154">사용자 지정 학습을 프로 비전 하기 전에 테 넌 트 앱 카탈로그를 만든 후 30 분 이상 기다립니다.</span><span class="sxs-lookup"><span data-stu-id="a95cf-154">Wait at least 30 minutes after creating the Tenant App Catalog before provisioning Custom Learning.</span></span> <span data-ttu-id="a95cf-155">이렇게 하면 SharePoint 내에서 앱 카탈로그 프로 비전 프로세스가 완료 됩니다.</span><span class="sxs-lookup"><span data-stu-id="a95cf-155">This ensures that the App Catalog provisioning process is complete within SharePoint.</span></span> 