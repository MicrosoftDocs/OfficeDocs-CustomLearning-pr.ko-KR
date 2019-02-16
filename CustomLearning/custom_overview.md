---
author: pkrebs
ms.author: pkrebs
title: Overview
ms.date: 02/15/2019
description: 관리자를 위한 Office 365의 사용자 지정 학습 개요
ms.openlocfilehash: c4b9679ae5a7158306bfd53e345f8e892ab206bc
ms.sourcegitcommit: afb5502604d271f49f6d1133db9dfc499f710eec
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 02/15/2019
ms.locfileid: "30064988"
---
# <a name="overview-of-custom-learning"></a><span data-ttu-id="7f62d-103">사용자 지정 학습 개요</span><span class="sxs-lookup"><span data-stu-id="7f62d-103">Overview of Custom Learning</span></span>
<span data-ttu-id="7f62d-p101">office 365에 대 한 사용자 지정 학습을 도입 하 여 조직 내에서 office 365의 사용 및 채택 속도를 빠르게 하도록 설계 된 Microsoft의 새로운 솔루션입니다. 사용자 지정 학습을 통해 다음을 수행할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="7f62d-p101">Introducing Custom Learning for Office 365, a new solution from Microsoft designed to speed the usage and adoption of Office 365 within an organization. With Custom Learning, you can:</span></span>

- <span data-ttu-id="7f62d-p102">환경에 Office 365에 대 한 사용자 지정 학습을 조정 합니다. 브랜드 및 로고, 교육 이벤트 및 지원 정보를 사용 하 여 사이트 페이지를 수정 합니다. 조직에서 지원 되지 않는 서비스 또는 기능의 콘텐츠를 숨기 거 나 표시 합니다.</span><span class="sxs-lookup"><span data-stu-id="7f62d-p102">Tailor Custom Learning for Office 365 to your environment. Modify site pages with your brand and logo, training events, and support info. Hide and show content for services or features that are not supported in your organization.</span></span> 
- <span data-ttu-id="7f62d-109">microsoft에서 콘텐츠와 사용자를 최신 상태로 유지-사용자 지정 학습을 통해 microsoft가 최신 콘텐츠를 최신 상태로 유지 하는 교육 콘텐츠의 동적 피드를 제공 합니다.</span><span class="sxs-lookup"><span data-stu-id="7f62d-109">Let Microsoft keep your content and users up-to-date – Custom Learning provides a dynamic feed of learning content that Microsoft keeps up-to-date.</span></span> 
- <span data-ttu-id="7f62d-110">조직의 정책, 절차 및 culture를 반영 하는 범주 및 사용자 지정 재생 목록 작성-사용자가 필요에 따라 특수 하 게 만든 콘텐츠를 학습 하는 기술을 작성할 수 있도록 합니다.</span><span class="sxs-lookup"><span data-stu-id="7f62d-110">Build categories and custom playlists reflecting your organization’s policies, procedures, and culture, enabling users to build skills with learning content crafted specifically to their needs.</span></span>

![cg_introducing-.png](media/cg_introducing.png)

## <a name="how-does-custom-learning-word"></a><span data-ttu-id="7f62d-112">사용자 지정 학습 단어</span><span class="sxs-lookup"><span data-stu-id="7f62d-112">How does Custom Learning word?</span></span>
<span data-ttu-id="7f62d-113">Office 365에 대 한 사용자 지정 학습 (사용자 지정 단기 학습)은 다음과 같은 세 부분으로 구성 됩니다.</span><span class="sxs-lookup"><span data-stu-id="7f62d-113">Custom Learning for Office 365 (Custom Learning for short) consists of three parts:</span></span> 
- <span data-ttu-id="7f62d-114">SharePoint 통신 사이트</span><span class="sxs-lookup"><span data-stu-id="7f62d-114">a SharePoint communication site</span></span>
- <span data-ttu-id="7f62d-115">SharePoint 웹 파트</span><span class="sxs-lookup"><span data-stu-id="7f62d-115">a SharePoint web part</span></span>
- <span data-ttu-id="7f62d-116">Microsoft online 카탈로그의 콘텐츠 라이브 피드</span><span class="sxs-lookup"><span data-stu-id="7f62d-116">a live feed of content from a Microsoft online catalog</span></span>

![cg_howitworks-.png](media/cg_howitworks.png)

## <a name="requirements-and-permissions"></a><span data-ttu-id="7f62d-118">요구 사항 및 사용 권한</span><span class="sxs-lookup"><span data-stu-id="7f62d-118">Requirements and Permissions</span></span>
<span data-ttu-id="7f62d-p103">Office 365에 대 한 사용자 지정 학습은 조직의 테 넌 트 관리자가 설치 해야 하며, 테 넌 트 관리자 권한이 있는 사용자 여야 합니다. 이 가이드에 포함 된이 사용자 지정 절차를 시작 하기 전에 SharePoint 테 넌 트 관리자가 사용자 지정 학습을 설정 했는지 확인 합니다. 확실히 모르겠으면 SharePoint 테 넌 트 관리자에 게 문의 하 여 사용자 지정 학습을 설치 했는지 확인 합니다. 또한 사용자 지정 학습 SharePoint 사이트의 URL도 확인 해야 합니다. 테 넌 트 관리자이 고 사용자 지정 학습을 설치 하지 않은 경우에는 Office 365 용 사용자 학습 설치 가이드를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="7f62d-p103">Custom Learning for Office 365 must be installed by your organization’s tenant administrator - someone who has Tenant Administrator permission. Before getting started with this customization procedures covered in this guide, ensure that Custom Learning has been set up by a SharePoint tenant administrator. If you’re not sure, contact your SharePoint tenant administrator to verify that Custom Learning has been installed. Also be sure to get the URL of the Custom Learning SharePoint site. If you are the Tenant Administrator and Custom Learning has not been installed, see the Custom Learning for Office 365 Installation Guide.</span></span> 

### <a name="permissions-required-for-custom-learning"></a><span data-ttu-id="7f62d-124">사용자 지정 학습에 필요한 사용 권한</span><span class="sxs-lookup"><span data-stu-id="7f62d-124">Permissions required for Custom Learning</span></span> 
<span data-ttu-id="7f62d-125">다음은 사용자 지정 학습을 설치, 사용자 지정 및 사용 하는 데 필요한 사용 권한에 대 한 분석입니다.</span><span class="sxs-lookup"><span data-stu-id="7f62d-125">Here’s a breakdown of the permissions required for installing, customizing, and using Custom Learning.</span></span> 

<span data-ttu-id="7f62d-126">**사용자 지정 학습 설치 권한**</span><span class="sxs-lookup"><span data-stu-id="7f62d-126">**Permissions to install Custom Learning**</span></span>
- <span data-ttu-id="7f62d-127">Office 365 전역 관리자</span><span class="sxs-lookup"><span data-stu-id="7f62d-127">Office 365 Global Administrator</span></span>
- <span data-ttu-id="7f62d-128">SharePoint 관리자</span><span class="sxs-lookup"><span data-stu-id="7f62d-128">SharePoint Administrator</span></span>

<span data-ttu-id="7f62d-129">**사용자 지정 학습 관리 기능 사용 권한**</span><span class="sxs-lookup"><span data-stu-id="7f62d-129">**Permissions to use Custom Learning Administration features**</span></span>
- <span data-ttu-id="7f62d-130">Office 365 sharepoint 관리자/sharepoint 사이트 소유자 권한</span><span class="sxs-lookup"><span data-stu-id="7f62d-130">Office 365 SharePoint Administrator/SharePoint Site Owner Permissions</span></span>
- <span data-ttu-id="7f62d-131">sharepoint 사이트 모음 관리자/sharepoint 사이트 소유자 권한</span><span class="sxs-lookup"><span data-stu-id="7f62d-131">SharePoint Site Collection Administrator/SharePoint Site Owner Permissions</span></span>

<span data-ttu-id="7f62d-132">**사용자로 사용자 지정 학습 사이트를 사용 하려면**</span><span class="sxs-lookup"><span data-stu-id="7f62d-132">**To use the Custom Learning site as a user**</span></span>
- <span data-ttu-id="7f62d-133">Office 365 사용자 권한/SharePoint 사이트 방문자 사용 권한 이상</span><span class="sxs-lookup"><span data-stu-id="7f62d-133">Office 365 user permissions/SharePoint Site Visitor Permissions or higher</span></span>
- <span data-ttu-id="7f62d-134">필요한 사용 권한이 부여 되었는지 모르는 경우 SharePoint 테 넌 트 관리자에 게 문의 하세요.</span><span class="sxs-lookup"><span data-stu-id="7f62d-134">If you’re not sure if you’ve been granted the necessary permissions, contact your SharePoint Tenant Administrator.</span></span>

### <a name="next-steps"></a><span data-ttu-id="7f62d-135">다음 단계</span><span class="sxs-lookup"><span data-stu-id="7f62d-135">Next Steps</span></span>

- [<span data-ttu-id="7f62d-136">재생 목록 사용자 지정 및 공유</span><span class="sxs-lookup"><span data-stu-id="7f62d-136">Customize and Share Playlists</span></span>](customplaylist.md)
- [<span data-ttu-id="7f62d-137">드라이브 도입</span><span class="sxs-lookup"><span data-stu-id="7f62d-137">Drive Adoption</span></span>](driveadoption.md) 