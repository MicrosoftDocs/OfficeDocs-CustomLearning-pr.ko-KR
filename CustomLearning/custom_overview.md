---
author: pkrebs
ms.author: pkrebs
title: 개요
ms.date: 02/18/2019
description: Microsoft 365 학습 경로 개요
ms.openlocfilehash: 74fac090177ad8009155e21a977b05ee2b742b3b
ms.sourcegitcommit: f5a7079d56598c14aef2f4b886c025a59ba89276
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 10/21/2019
ms.locfileid: "34247857"
---
# <a name="customize-the-learning-experience"></a><span data-ttu-id="ddd69-103">학습 환경 사용자 지정</span><span class="sxs-lookup"><span data-stu-id="ddd69-103">Customize the learning experience</span></span>

<span data-ttu-id="ddd69-104">Microsoft 365 학습 경로 소개 Microsoft에서 제공 하는 새로운 솔루션은 조직 내에서 Office 365의 사용 및 채택 속도를 높일 수 있도록 설계 되었습니다.</span><span class="sxs-lookup"><span data-stu-id="ddd69-104">Introducing Microsoft 365 learning pathways, a new solution from Microsoft designed to speed the usage and adoption of Office 365 within an organization.</span></span> <span data-ttu-id="ddd69-105">학습 pathwyas을 사용 하 여 다음을 수행할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ddd69-105">With learning pathwyas, you can:</span></span>
- <span data-ttu-id="ddd69-106">사용자 환경에 맞게 Microsoft 365 학습 및 채택 콘텐츠를 조정 합니다.</span><span class="sxs-lookup"><span data-stu-id="ddd69-106">Tailor Microsoft 365 learning and adoption content for your environment</span></span> 
- <span data-ttu-id="ddd69-107">조직에서 지원 되는 서비스 또는 기능을 반영 하기 위해 콘텐츠를 숨기 거 나 표시</span><span class="sxs-lookup"><span data-stu-id="ddd69-107">Hide or show content to reflect the services or features supported in your organization</span></span> 
- <span data-ttu-id="ddd69-108">Microsoft의 최신 학습 콘텐츠 피드를 사용 하 여 콘텐츠 및 사용자를 최신 상태로 유지</span><span class="sxs-lookup"><span data-stu-id="ddd69-108">Keep your content and users current with an up-to-date feed of learning content from Microsoft</span></span> 
- <span data-ttu-id="ddd69-109">사용자의 요구에 맞게 만든 사용자 지정 재생 목록 및 범주 작성</span><span class="sxs-lookup"><span data-stu-id="ddd69-109">Build custom playlists and categories crafted specifically for your user's needs</span></span>

![cg-introducing-.png](media/cg-introducing.png)

## <a name="how-does-learning-pathways-work"></a><span data-ttu-id="ddd69-111">학습용 경로는 어떻게 작동 하나요?</span><span class="sxs-lookup"><span data-stu-id="ddd69-111">How does learning pathways work?</span></span>

<span data-ttu-id="ddd69-112">Office 365 (간단한 학습 경로)에 대 한 학습 경로는 다음과 같은 세 부분으로 구성 됩니다.</span><span class="sxs-lookup"><span data-stu-id="ddd69-112">learning pathways for Office 365 (learning pathways for short) consists of three parts:</span></span> 
1. <span data-ttu-id="ddd69-113">Microsoft online 카탈로그의 콘텐츠 라이브 피드</span><span class="sxs-lookup"><span data-stu-id="ddd69-113">a live feed of content from a Microsoft online catalog</span></span>
2. <span data-ttu-id="ddd69-114">SharePoint 통신 사이트</span><span class="sxs-lookup"><span data-stu-id="ddd69-114">a SharePoint communication site</span></span>
3. <span data-ttu-id="ddd69-115">SharePoint 웹 파트</span><span class="sxs-lookup"><span data-stu-id="ddd69-115">a SharePoint web part</span></span> 

![cg-howitworks-.png](media/cg-howitworks.png)

## <a name="requirements-and-permissions"></a><span data-ttu-id="ddd69-117">요구 사항 및 사용 권한</span><span class="sxs-lookup"><span data-stu-id="ddd69-117">Requirements and Permissions</span></span>

<span data-ttu-id="ddd69-118">이 가이드를 시작 하기 전에 SharePoint 테 넌 트 관리자가 학습 경로를 설정 했는지 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="ddd69-118">Before getting started with this guide, ensure that learning pathways has been set up by your SharePoint Tenant Administrator.</span></span> <span data-ttu-id="ddd69-119">설정 되어 있는지 모르는 경우 SharePoint 테 넌 트 관리자에 게 문의 하 여 학습 경로가 프로 비전 되었는지 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="ddd69-119">If you’re not sure if it's been set up, contact your SharePoint tenant administrator to verify that learning pathways has been provisioned.</span></span> <span data-ttu-id="ddd69-120">또한 학습 경로 SharePoint 사이트의 URL도 확인 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="ddd69-120">Also be sure to get the URL of the learning pathways SharePoint site.</span></span> <span data-ttu-id="ddd69-121">테 넌 트 관리자이 고 학습 경로가 프로 비전 되지 않은 경우 [프로 비전 학습 경로](custom_provision.md)를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="ddd69-121">If you are the Tenant Administrator and learning pathways has not been provisioned, see [Provision learning pathways](custom_provision.md).</span></span> 

### <a name="permissions-to-provision-learning-pathways"></a><span data-ttu-id="ddd69-122">학습 경로를 프로 비전 하기 위한 권한</span><span class="sxs-lookup"><span data-stu-id="ddd69-122">Permissions to provision learning pathways</span></span>

- <span data-ttu-id="ddd69-123">테 넌 트 관리자 (Office 365 전역 관리자 라고도 함)</span><span class="sxs-lookup"><span data-stu-id="ddd69-123">Tenant Administrator, also known as Office 365 Global Administrator</span></span>
- <span data-ttu-id="ddd69-124">사이트에 대 한 소유자 권한이 있는 SharePoint 사이트 모음 관리자</span><span class="sxs-lookup"><span data-stu-id="ddd69-124">SharePoint Site Collection Administrator with Owner permissions on the site</span></span>

### <a name="permissions-to-use-learning-pathways-administration-features"></a><span data-ttu-id="ddd69-125">학습 경로 관리 기능을 사용 하기 위한 권한</span><span class="sxs-lookup"><span data-stu-id="ddd69-125">Permissions to use learning pathways Administration features</span></span>

- <span data-ttu-id="ddd69-126">사이트 모음 관리자</span><span class="sxs-lookup"><span data-stu-id="ddd69-126">Site Collection Administrator</span></span>
- <span data-ttu-id="ddd69-127">SharePoint 소유자 또는 구성원 권한</span><span class="sxs-lookup"><span data-stu-id="ddd69-127">SharePoint Owner or Member permissions</span></span>

### <a name="permissions-to-use-the-learning-pathways-site-as-a-user"></a><span data-ttu-id="ddd69-128">사용자로 서 학습 경로 사이트를 사용할 수 있는 권한</span><span class="sxs-lookup"><span data-stu-id="ddd69-128">Permissions to use the learning pathways site as a user</span></span>

- <span data-ttu-id="ddd69-129">Office 365 사용자 권한/SharePoint 사이트 방문자 사용 권한 이상</span><span class="sxs-lookup"><span data-stu-id="ddd69-129">Office 365 user permissions/SharePoint Site Visitor permissions or higher</span></span>

## <a name="get-started-with-customization"></a><span data-ttu-id="ddd69-130">사용자 지정 시작 하기</span><span class="sxs-lookup"><span data-stu-id="ddd69-130">Get started with customization</span></span>
<span data-ttu-id="ddd69-131">사이트 및 웹 파트를 사용자 지정 하는 데 필요한 권한이 있는지 확인 한 후에는 사용자 지정 프로세스를 시작 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="ddd69-131">Once you've ensured you have the necessary permissions to customize the site and web part, it's time to get started with the customization process.</span></span> 

- <span data-ttu-id="ddd69-132">시작 하려면 [학습 경로 사이트를](custom_goto.md)참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="ddd69-132">To get started, see [Go to the learning pathways site](custom_goto.md).</span></span>