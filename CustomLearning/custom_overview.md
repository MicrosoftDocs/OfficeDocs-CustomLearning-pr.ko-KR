---
author: pkrebs
ms.author: pkrebs
title: 개요
ms.date: 02/18/2019
description: 관리자를 위한 Office 365의 사용자 지정 학습 개요
ms.openlocfilehash: 6aee3a93a5109b37e43a7118bd98ca31e8b9ac1f
ms.sourcegitcommit: 775d6807291ab263eea5ec649d9aaf1933fb41ca
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32055644"
---
# <a name="customize-the-learning-experience"></a><span data-ttu-id="c1871-103">학습 환경 사용자 지정</span><span class="sxs-lookup"><span data-stu-id="c1871-103">Customize the Learning Experience</span></span>

<span data-ttu-id="c1871-104">office 365에 대 한 사용자 지정 학습을 도입 하 여 조직 내에서 office 365의 사용 및 채택 속도를 빠르게 하도록 설계 된 Microsoft의 새로운 솔루션입니다.</span><span class="sxs-lookup"><span data-stu-id="c1871-104">Introducing Custom Learning for Office 365, a new solution from Microsoft designed to speed the usage and adoption of Office 365 within an organization.</span></span> <span data-ttu-id="c1871-105">사용자 지정 학습을 통해 다음을 수행할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c1871-105">With Custom Learning, you can:</span></span>
- <span data-ttu-id="c1871-106">사용자 환경에 맞게 Office 365 학습 및 채택 콘텐츠 조정</span><span class="sxs-lookup"><span data-stu-id="c1871-106">Tailor Office 365 learning and adoption content for your environment</span></span> 
- <span data-ttu-id="c1871-107">조직에서 지원 되는 서비스 또는 기능을 반영 하기 위해 콘텐츠를 숨기 거 나 표시</span><span class="sxs-lookup"><span data-stu-id="c1871-107">Hide or show content to reflect the services or features supported in your organization</span></span> 
- <span data-ttu-id="c1871-108">Microsoft의 최신 학습 콘텐츠 피드를 사용 하 여 콘텐츠 및 사용자를 최신 상태로 유지</span><span class="sxs-lookup"><span data-stu-id="c1871-108">Keep your content and users current with an up-to-date feed of learning content from Microsoft</span></span> 
- <span data-ttu-id="c1871-109">사용자의 요구에 맞게 만든 사용자 지정 재생 목록 및 범주 작성</span><span class="sxs-lookup"><span data-stu-id="c1871-109">Build custom playlists and categories crafted specifically for your user's needs</span></span>

![cg-introducing-.png](media/cg-introducing.png)

## <a name="how-does-custom-learning-work"></a><span data-ttu-id="c1871-111">사용자 지정 학습은 어떤 방식으로 작동 하나요?</span><span class="sxs-lookup"><span data-stu-id="c1871-111">How does Custom Learning work?</span></span>

<span data-ttu-id="c1871-112">Office 365에 대 한 사용자 지정 학습 (사용자 지정 단기 학습)은 다음과 같은 세 부분으로 구성 됩니다.</span><span class="sxs-lookup"><span data-stu-id="c1871-112">Custom Learning for Office 365 (Custom Learning for short) consists of three parts:</span></span> 
1. <span data-ttu-id="c1871-113">Microsoft online 카탈로그의 콘텐츠 라이브 피드</span><span class="sxs-lookup"><span data-stu-id="c1871-113">a live feed of content from a Microsoft online catalog</span></span>
2. <span data-ttu-id="c1871-114">SharePoint 통신 사이트</span><span class="sxs-lookup"><span data-stu-id="c1871-114">a SharePoint communication site</span></span>
3. <span data-ttu-id="c1871-115">SharePoint 웹 파트</span><span class="sxs-lookup"><span data-stu-id="c1871-115">a SharePoint web part</span></span> 

![cg-howitworks-.png](media/cg-howitworks.png)

## <a name="requirements-and-permissions"></a><span data-ttu-id="c1871-117">요구 사항 및 사용 권한</span><span class="sxs-lookup"><span data-stu-id="c1871-117">Requirements and Permissions</span></span>

<span data-ttu-id="c1871-118">이 가이드를 시작 하기 전에 SharePoint 테 넌 트 관리자가 사용자 지정 학습을 설정 했는지 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="c1871-118">Before getting started with this guide, ensure that Custom Learning has been set up by your SharePoint Tenant Administrator.</span></span> <span data-ttu-id="c1871-119">설정 되어 있는지 확인 하지 않은 경우 SharePoint 테 넌 트 관리자에 게 문의 하 여 사용자 지정 학습을 프로 비전 했는지 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="c1871-119">If you’re not sure if it's been set up, contact your SharePoint tenant administrator to verify that Custom Learning has been provisioned.</span></span> <span data-ttu-id="c1871-120">또한 사용자 지정 학습 SharePoint 사이트의 URL도 확인 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="c1871-120">Also be sure to get the URL of the Custom Learning SharePoint site.</span></span> <span data-ttu-id="c1871-121">테 넌 트 관리자이 고 사용자 지정 학습이 프로 비전 되지 않은 경우 [프로 비전 사용자 지정 학습](custom_provision.md)을 참조 하십시오.</span><span class="sxs-lookup"><span data-stu-id="c1871-121">If you are the Tenant Administrator and Custom Learning has not been provisioned, see [Provision Custom Learning](custom_provision.md).</span></span> 

### <a name="permissions-to-provision-custom-learning"></a><span data-ttu-id="c1871-122">사용자 지정 학습 프로 비전 사용 권한</span><span class="sxs-lookup"><span data-stu-id="c1871-122">Permissions to provision Custom Learning</span></span>

- <span data-ttu-id="c1871-123">테 넌 트 관리자 (Office 365 전역 관리자 라고도 함)</span><span class="sxs-lookup"><span data-stu-id="c1871-123">Tenant Administrator, also known as Office 365 Global Administrator</span></span>
- <span data-ttu-id="c1871-124">사이트에 대 한 소유자 권한이 있는 SharePoint 사이트 모음 관리자</span><span class="sxs-lookup"><span data-stu-id="c1871-124">SharePoint Site Collection Administrator with Owner permissions on the site</span></span>

### <a name="permissions-to-use-custom-learning-administration-features"></a><span data-ttu-id="c1871-125">사용자 지정 학습 관리 기능 사용 권한</span><span class="sxs-lookup"><span data-stu-id="c1871-125">Permissions to use Custom Learning Administration features</span></span>

- <span data-ttu-id="c1871-126">사이트 모음 관리자</span><span class="sxs-lookup"><span data-stu-id="c1871-126">Site Collection Administrator</span></span>
- <span data-ttu-id="c1871-127">SharePoint 소유자 또는 구성원 권한</span><span class="sxs-lookup"><span data-stu-id="c1871-127">SharePoint Owner or Member permissions</span></span>

### <a name="permissions-to-use-the-custom-learning-site-as-a-user"></a><span data-ttu-id="c1871-128">사용자로 사용자 지정 학습 사이트를 사용할 수 있는 권한</span><span class="sxs-lookup"><span data-stu-id="c1871-128">Permissions to use the Custom Learning site as a user</span></span>

- <span data-ttu-id="c1871-129">Office 365 사용자 권한/SharePoint 사이트 방문자 사용 권한 이상</span><span class="sxs-lookup"><span data-stu-id="c1871-129">Office 365 user permissions/SharePoint Site Visitor permissions or higher</span></span>

## <a name="get-started-with-customization"></a><span data-ttu-id="c1871-130">사용자 지정 시작 하기</span><span class="sxs-lookup"><span data-stu-id="c1871-130">Get started with customization</span></span>
<span data-ttu-id="c1871-131">사이트 및 웹 파트를 사용자 지정 하는 데 필요한 권한이 있는지 확인 한 후에는 사용자 지정 프로세스를 시작 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="c1871-131">Once you've ensured you have the necessary permissions to customize the site and web part, it's time to get started with the customization process.</span></span> 

- <span data-ttu-id="c1871-132">시작 하려면 [사용자 지정 학습 사이트로 이동을](custom_goto.md)참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="c1871-132">To get started, see [Go to the Custom Learning Site](custom_goto.md).</span></span>