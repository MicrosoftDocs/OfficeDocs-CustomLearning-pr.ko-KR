---
author: pkrebs
ms.author: pkrebs
title: 학습 경로 사용자 지정
ms.date: 02/18/2019
manager: bpardi
audience: admin
ms.topic: article
description: 학습 경로 사용자 지정
ms.service: sharepoint-online
ms.openlocfilehash: a5087096ec3bd7c1194aab9dd089276fc196a736
ms.sourcegitcommit: 97e175e5ff5b6a9e0274d5ec9b39fdf7e18eb387
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/25/2021
ms.locfileid: "51999504"
---
# <a name="customize-learning-pathways"></a><span data-ttu-id="3e08f-103">학습 경로 사용자 지정</span><span class="sxs-lookup"><span data-stu-id="3e08f-103">Customize learning pathways</span></span>

<span data-ttu-id="3e08f-104">Microsoft 365 학습 경로는 조직의 콘텐츠를 사용자 지정할 수 있는 다양한 방법을 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="3e08f-104">Microsoft 365 learning pathways provides a variety of ways that you can customize content for your organization.</span></span> <span data-ttu-id="3e08f-105">예를 들어, 다음을 수행할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="3e08f-105">For example, you can:</span></span>  
- <span data-ttu-id="3e08f-106">학습 경로 SharePoint 사이트 수정 - 사이트 이름, 로고 및 변경합니다.</span><span class="sxs-lookup"><span data-stu-id="3e08f-106">Modify the learning pathways SharePoint site - Change the site name, logo, and them.</span></span> <span data-ttu-id="3e08f-107">질문하기 및 도움말 확인 페이지를 수정하여 자체 도움말 센터를 만드십시오.</span><span class="sxs-lookup"><span data-stu-id="3e08f-107">Modify the Ask Questions and Get Help page to create your own Help Center.</span></span> 
- <span data-ttu-id="3e08f-108">조직에서 지원되는 서비스 또는 기능을 반영하기 위해 콘텐츠 숨기기 또는 표시</span><span class="sxs-lookup"><span data-stu-id="3e08f-108">Hide or show content to reflect the services or features supported in your organization</span></span> 
- <span data-ttu-id="3e08f-109">사용자의 요구에 따라 특별히 만들어진 사용자 지정 재생 목록 및 하위 구성표 빌드</span><span class="sxs-lookup"><span data-stu-id="3e08f-109">Build custom playlists and subcategories crafted specifically for your user's needs</span></span>
- <span data-ttu-id="3e08f-110">Microsoft Teams, Outlook 모바일의 채택을 진행하거나 Microsoft 365와 공동 작업하는 등 비즈니스 결과를 지원하기 위해 필터링된 콘텐츠로 방문 페이지를 빌드합니다.</span><span class="sxs-lookup"><span data-stu-id="3e08f-110">Build landing pages with content filtered to support business outcomes, such as driving the adoption of Microsoft Teams, Outlook mobile, or working more collaboratively with Microsoft 365.</span></span>

![일반 Microsoft 학습 경로 사진 컬렉션입니다.](media/cg-introducing.png)

## <a name="requirements-and-permissions"></a><span data-ttu-id="3e08f-112">요구 사항 및 사용 권한</span><span class="sxs-lookup"><span data-stu-id="3e08f-112">Requirements and Permissions</span></span>

<span data-ttu-id="3e08f-113">학습 경로 사용자 지정 지침을 시작하기 전에 SharePoint 테넌트 관리자가 학습 경로를 설정해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="3e08f-113">Before getting started with the Customize learning pathways guidance, ensure that learning pathways has been set up by your SharePoint Tenant Administrator.</span></span> <span data-ttu-id="3e08f-114">설정되어 있는지 확실하지 않은 경우 SharePoint 테넌트 관리자에게 문의하여 학습 경로가 프로비전되어 있는지 확인해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="3e08f-114">If you’re not sure if it's been set up, contact your SharePoint tenant administrator to verify that learning pathways has been provisioned.</span></span> <span data-ttu-id="3e08f-115">또한 학습 경로 SharePoint 사이트의 URL을 다운로드해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="3e08f-115">Also be sure to get the URL of the learning pathways SharePoint site.</span></span> <span data-ttu-id="3e08f-116">테넌트 관리자인 경우 학습 경로가 프로비전되지 않은 경우 학습 경로 프로비전을 [참조합니다.](custom_provision.md)</span><span class="sxs-lookup"><span data-stu-id="3e08f-116">If you are the Tenant Administrator and learning pathways has not been provisioned, see [Provision learning pathways](custom_provision.md).</span></span> 

### <a name="permissions-to-provision-learning-pathways"></a><span data-ttu-id="3e08f-117">학습 경로를 프로비전하기 위한 사용 권한</span><span class="sxs-lookup"><span data-stu-id="3e08f-117">Permissions to provision learning pathways</span></span>

- <span data-ttu-id="3e08f-118">Office 365 전역 관리자라고도 하는 테넌트 관리자</span><span class="sxs-lookup"><span data-stu-id="3e08f-118">Tenant Administrator, also known as Office 365 Global Administrator</span></span>
- <span data-ttu-id="3e08f-119">사이트에 대한 소유자 권한이 있는 SharePoint 사이트 모음 관리자 </span><span class="sxs-lookup"><span data-stu-id="3e08f-119">SharePoint Site Collection Administrator with Owner permissions on the site</span></span>

### <a name="permissions-to-use-learning-pathways-administration-features"></a><span data-ttu-id="3e08f-120">학습 경로 관리 기능 사용 권한</span><span class="sxs-lookup"><span data-stu-id="3e08f-120">Permissions to use learning pathways Administration features</span></span>

- <span data-ttu-id="3e08f-121">사이트 모음 관리자</span><span class="sxs-lookup"><span data-stu-id="3e08f-121">Site Collection Administrator</span></span>
- <span data-ttu-id="3e08f-122">SharePoint 소유자 또는 구성원 권한</span><span class="sxs-lookup"><span data-stu-id="3e08f-122">SharePoint Owner or Member permissions</span></span>

### <a name="permissions-to-use-the-learning-pathways-site-as-a-user"></a><span data-ttu-id="3e08f-123">사용자로 학습 경로 사이트를 사용할 수 있는 권한</span><span class="sxs-lookup"><span data-stu-id="3e08f-123">Permissions to use the learning pathways site as a user</span></span>

- <span data-ttu-id="3e08f-124">Office 365 사용자 사용 권한/SharePoint 사이트 방문자 사용 권한 이상</span><span class="sxs-lookup"><span data-stu-id="3e08f-124">Office 365 user permissions/SharePoint Site Visitor permissions or higher</span></span>

## <a name="get-started-with-customization"></a><span data-ttu-id="3e08f-125">사용자 지정 시작</span><span class="sxs-lookup"><span data-stu-id="3e08f-125">Get started with customization</span></span>
<span data-ttu-id="3e08f-126">사이트 및 웹 파트를 사용자 지정하는 데 필요한 사용 권한을 얻었다면 이제 사용자 지정 프로세스를 시작해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="3e08f-126">Once you've ensured you have the necessary permissions to customize the site and web part, it's time to get started with the customization process.</span></span> 

- <span data-ttu-id="3e08f-127">시작을 위해 [학습 경로 사이트로 이동을 참조하세요.](custom_goto.md)</span><span class="sxs-lookup"><span data-stu-id="3e08f-127">To get started, see [Go to the learning pathways site](custom_goto.md).</span></span>