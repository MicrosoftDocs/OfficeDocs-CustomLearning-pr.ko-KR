---
author: pkrebs
ms.author: pkrebs
title: Overview
ms.date: 02/18/2019
description: 관리자를 위한 Office 365의 사용자 지정 학습 개요
ms.openlocfilehash: 98187038b66252523c74d88dd9bfd0f217591bc5
ms.sourcegitcommit: e10085e60ca3f38029fde229fb093e6bc4a34203
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 02/25/2019
ms.locfileid: "30087537"
---
# <a name="customize-the-learning-experience"></a><span data-ttu-id="af9ec-103">학습 환경 사용자 지정</span><span class="sxs-lookup"><span data-stu-id="af9ec-103">Customize the Learning Experience</span></span>

<span data-ttu-id="af9ec-p101">office 365에 대 한 사용자 지정 학습을 도입 하 여 조직 내에서 office 365의 사용 및 채택 속도를 빠르게 하도록 설계 된 Microsoft의 새로운 솔루션입니다. 사용자 지정 학습을 통해 다음을 수행할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="af9ec-p101">Introducing Custom Learning for Office 365, a new solution from Microsoft designed to speed the usage and adoption of Office 365 within an organization. With Custom Learning, you can:</span></span>
- <span data-ttu-id="af9ec-106">사용자 환경에 맞게 Office 365 학습 및 채택 콘텐츠 조정</span><span class="sxs-lookup"><span data-stu-id="af9ec-106">Tailor Office 365 learning and adoption content for your environment</span></span> 
- <span data-ttu-id="af9ec-107">조직에서 지원 되는 서비스 또는 기능을 반영 하기 위해 콘텐츠를 숨기 거 나 표시</span><span class="sxs-lookup"><span data-stu-id="af9ec-107">Hide or show content to reflect the services or features supported in your organization</span></span> 
- <span data-ttu-id="af9ec-108">Microsoft의 최신 학습 콘텐츠 피드를 사용 하 여 콘텐츠 및 사용자를 최신 상태로 유지</span><span class="sxs-lookup"><span data-stu-id="af9ec-108">Keep your content and users current with an up-to-date feed of learning content from Microsoft</span></span> 
- <span data-ttu-id="af9ec-109">사용자의 요구에 맞게 만든 사용자 지정 재생 목록 및 범주 작성</span><span class="sxs-lookup"><span data-stu-id="af9ec-109">Build custom playlists and categories crafted specifically for your user's needs</span></span>

![cg-introducing-.png](media/cg-introducing.png)

## <a name="how-does-custom-learning-work"></a><span data-ttu-id="af9ec-111">사용자 지정 학습은 어떤 방식으로 작동 하나요?</span><span class="sxs-lookup"><span data-stu-id="af9ec-111">How does Custom Learning work?</span></span>

<span data-ttu-id="af9ec-112">Office 365에 대 한 사용자 지정 학습 (사용자 지정 단기 학습)은 다음과 같은 세 부분으로 구성 됩니다.</span><span class="sxs-lookup"><span data-stu-id="af9ec-112">Custom Learning for Office 365 (Custom Learning for short) consists of three parts:</span></span> 
1. <span data-ttu-id="af9ec-113">Microsoft online 카탈로그의 콘텐츠 라이브 피드</span><span class="sxs-lookup"><span data-stu-id="af9ec-113">a live feed of content from a Microsoft online catalog</span></span>
2. <span data-ttu-id="af9ec-114">SharePoint 통신 사이트</span><span class="sxs-lookup"><span data-stu-id="af9ec-114">a SharePoint communication site</span></span>
3. <span data-ttu-id="af9ec-115">SharePoint 웹 파트</span><span class="sxs-lookup"><span data-stu-id="af9ec-115">a SharePoint web part</span></span> 

![cg-howitworks-.png](media/cg-howitworks.png)

## <a name="requirements-and-permissions"></a><span data-ttu-id="af9ec-117">요구 사항 및 사용 권한</span><span class="sxs-lookup"><span data-stu-id="af9ec-117">Requirements and Permissions</span></span>

<span data-ttu-id="af9ec-p102">이 가이드를 시작 하기 전에 SharePoint 테 넌 트 관리자가 사용자 지정 학습을 설정 했는지 확인 합니다. 설정 되어 있는지 확인 하지 않은 경우 SharePoint 테 넌 트 관리자에 게 문의 하 여 사용자 지정 학습을 설치 했는지 확인 합니다. 또한 사용자 지정 학습 SharePoint 사이트의 URL도 확인 해야 합니다. 테 넌 트 관리자이 고 사용자 지정 학습을 설치 하지 않은 경우에는 Office 365 용 사용자 학습 설치 가이드를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="af9ec-p102">Before getting started with this guide, ensure that Custom Learning has been set up by your  SharePoint tenant administrator. If you’re not sure if it's been set up, contact your SharePoint tenant administrator to verify that Custom Learning has been installed. Also be sure to get the URL of the Custom Learning SharePoint site. If you are the Tenant Administrator and Custom Learning has not been installed, see the Custom Learning for Office 365 Installation Guide.</span></span> 

### <a name="permissions-to-install-custom-learning"></a><span data-ttu-id="af9ec-122">사용자 지정 학습 설치 권한</span><span class="sxs-lookup"><span data-stu-id="af9ec-122">Permissions to install Custom Learning</span></span>

- <span data-ttu-id="af9ec-123">Office 365 전역 관리자</span><span class="sxs-lookup"><span data-stu-id="af9ec-123">Office 365 Global Administrator</span></span>
- <span data-ttu-id="af9ec-124">SharePoint 관리자</span><span class="sxs-lookup"><span data-stu-id="af9ec-124">SharePoint Administrator</span></span>

### <a name="permissions-to-use-custom-learning-administration-features"></a><span data-ttu-id="af9ec-125">사용자 지정 학습 관리 기능 사용 권한</span><span class="sxs-lookup"><span data-stu-id="af9ec-125">Permissions to use Custom Learning Administration features</span></span>

- <span data-ttu-id="af9ec-126">Office 365 sharepoint 관리자/sharepoint 사이트 소유자 권한</span><span class="sxs-lookup"><span data-stu-id="af9ec-126">Office 365 SharePoint Administrator/SharePoint Site Owner Permissions</span></span>
- <span data-ttu-id="af9ec-127">sharepoint 사이트 모음 관리자/sharepoint 사이트 소유자 권한</span><span class="sxs-lookup"><span data-stu-id="af9ec-127">SharePoint Site Collection Administrator/SharePoint Site Owner Permissions</span></span>

### <a name="permissions-to-use-the-custom-learning-site-as-a-user"></a><span data-ttu-id="af9ec-128">사용자로 사용자 지정 학습 사이트를 사용할 수 있는 권한</span><span class="sxs-lookup"><span data-stu-id="af9ec-128">Permissions to use the Custom Learning site as a user</span></span>

- <span data-ttu-id="af9ec-129">Office 365 사용자 권한/SharePoint 사이트 방문자 사용 권한 이상</span><span class="sxs-lookup"><span data-stu-id="af9ec-129">Office 365 user permissions/SharePoint Site Visitor Permissions or higher</span></span>


