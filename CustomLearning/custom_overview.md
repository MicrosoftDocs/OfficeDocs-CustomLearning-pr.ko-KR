---
author: pkrebs
ms.author: pkrebs
title: 학습 경로 사용자 지정
ms.date: 02/18/2019
description: 학습 경로 사용자 지정
ms.openlocfilehash: 15d782455204cf043937bec03041a85abc9e4ee3
ms.sourcegitcommit: 3b8896c81ad2adbcfdbda658482847af5fccb264
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 10/30/2019
ms.locfileid: "37886641"
---
# <a name="customize-learning-pathways"></a><span data-ttu-id="a86c5-103">학습 경로 사용자 지정</span><span class="sxs-lookup"><span data-stu-id="a86c5-103">Customize learning pathways</span></span>

<span data-ttu-id="a86c5-104">Microsoft 365 학습 경로는 조직의 콘텐츠를 사용자 지정할 수 있는 다양 한 방법을 제공 합니다.</span><span class="sxs-lookup"><span data-stu-id="a86c5-104">Microsoft 365 learning pathways provides a variety of ways that you can customize content for your organization.</span></span> <span data-ttu-id="a86c5-105">예를 들어, 다음을 수행할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="a86c5-105">For example, you can:</span></span>  
- <span data-ttu-id="a86c5-106">학습 경로 SharePoint 사이트 수정-사이트 이름, 로고 등을 변경 합니다.</span><span class="sxs-lookup"><span data-stu-id="a86c5-106">Modify the learning pathways SharePoint site - Change the site name, logo, and them.</span></span> <span data-ttu-id="a86c5-107">질문 하기 및 도움말 보기 페이지를 수정 하 여 자신만의 도움말 센터를 만들 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="a86c5-107">Modify the Ask Questions and Get Help page to create your own Help Center.</span></span> 
- <span data-ttu-id="a86c5-108">조직에서 지원 되는 서비스 또는 기능을 반영 하기 위해 콘텐츠를 숨기 거 나 표시</span><span class="sxs-lookup"><span data-stu-id="a86c5-108">Hide or show content to reflect the services or features supported in your organization</span></span> 
- <span data-ttu-id="a86c5-109">사용자의 요구에 맞게 특별히 제작 된 사용자 지정 재생 목록 및 하위 범주 작성</span><span class="sxs-lookup"><span data-stu-id="a86c5-109">Build custom playlists and subcategories crafted specifically for your user's needs</span></span>
- <span data-ttu-id="a86c5-110">Microsoft 팀의 채택, Outlook 모바일 또는 Microsoft 365 공동 작업을 촉진 하는 등 비즈니스 결과를 지원 하도록 필터링 된 콘텐츠를 사용 하 여 랜딩 페이지를 구성 합니다.</span><span class="sxs-lookup"><span data-stu-id="a86c5-110">Build landing pages with content filtered to support business outcomes, such as driving the adoption of Microsoft Teams, Outlook mobile, or working more collaboratively with Microsoft 365.</span></span>

![cg-introducing-.png](media/cg-introducing.png)

## <a name="requirements-and-permissions"></a><span data-ttu-id="a86c5-112">요구 사항 및 사용 권한</span><span class="sxs-lookup"><span data-stu-id="a86c5-112">Requirements and Permissions</span></span>

<span data-ttu-id="a86c5-113">학습 경로 사용자 지정 지침을 시작 하기 전에 SharePoint 테 넌 트 관리자가 학습 경로를 설정 했는지 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="a86c5-113">Before getting started with the Customize learning pathways guidance, ensure that learning pathways has been set up by your SharePoint Tenant Administrator.</span></span> <span data-ttu-id="a86c5-114">설정 되어 있는지 모르는 경우 SharePoint 테 넌 트 관리자에 게 문의 하 여 학습 경로가 프로 비전 되었는지 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="a86c5-114">If you’re not sure if it's been set up, contact your SharePoint tenant administrator to verify that learning pathways has been provisioned.</span></span> <span data-ttu-id="a86c5-115">또한 학습 경로 SharePoint 사이트의 URL도 확인 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="a86c5-115">Also be sure to get the URL of the learning pathways SharePoint site.</span></span> <span data-ttu-id="a86c5-116">테 넌 트 관리자이 고 학습 경로가 프로 비전 되지 않은 경우 [프로 비전 학습 경로](custom_provision.md)를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="a86c5-116">If you are the Tenant Administrator and learning pathways has not been provisioned, see [Provision learning pathways](custom_provision.md).</span></span> 

### <a name="permissions-to-provision-learning-pathways"></a><span data-ttu-id="a86c5-117">학습 경로를 프로 비전 하기 위한 권한</span><span class="sxs-lookup"><span data-stu-id="a86c5-117">Permissions to provision learning pathways</span></span>

- <span data-ttu-id="a86c5-118">테 넌 트 관리자 (Office 365 전역 관리자 라고도 함)</span><span class="sxs-lookup"><span data-stu-id="a86c5-118">Tenant Administrator, also known as Office 365 Global Administrator</span></span>
- <span data-ttu-id="a86c5-119">사이트에 대 한 소유자 권한이 있는 SharePoint 사이트 모음 관리자</span><span class="sxs-lookup"><span data-stu-id="a86c5-119">SharePoint Site Collection Administrator with Owner permissions on the site</span></span>

### <a name="permissions-to-use-learning-pathways-administration-features"></a><span data-ttu-id="a86c5-120">학습 경로 관리 기능을 사용 하기 위한 권한</span><span class="sxs-lookup"><span data-stu-id="a86c5-120">Permissions to use learning pathways Administration features</span></span>

- <span data-ttu-id="a86c5-121">사이트 모음 관리자</span><span class="sxs-lookup"><span data-stu-id="a86c5-121">Site Collection Administrator</span></span>
- <span data-ttu-id="a86c5-122">SharePoint 소유자 또는 구성원 권한</span><span class="sxs-lookup"><span data-stu-id="a86c5-122">SharePoint Owner or Member permissions</span></span>

### <a name="permissions-to-use-the-learning-pathways-site-as-a-user"></a><span data-ttu-id="a86c5-123">사용자로 서 학습 경로 사이트를 사용할 수 있는 권한</span><span class="sxs-lookup"><span data-stu-id="a86c5-123">Permissions to use the learning pathways site as a user</span></span>

- <span data-ttu-id="a86c5-124">Office 365 사용자 권한/SharePoint 사이트 방문자 사용 권한 이상</span><span class="sxs-lookup"><span data-stu-id="a86c5-124">Office 365 user permissions/SharePoint Site Visitor permissions or higher</span></span>

## <a name="get-started-with-customization"></a><span data-ttu-id="a86c5-125">사용자 지정 시작 하기</span><span class="sxs-lookup"><span data-stu-id="a86c5-125">Get started with customization</span></span>
<span data-ttu-id="a86c5-126">사이트 및 웹 파트를 사용자 지정 하는 데 필요한 권한이 있는지 확인 한 후에는 사용자 지정 프로세스를 시작 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="a86c5-126">Once you've ensured you have the necessary permissions to customize the site and web part, it's time to get started with the customization process.</span></span> 

- <span data-ttu-id="a86c5-127">시작 하려면 [학습 경로 사이트를](custom_goto.md)참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="a86c5-127">To get started, see [Go to the learning pathways site](custom_goto.md).</span></span>