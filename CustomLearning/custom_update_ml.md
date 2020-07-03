---
author: pkrebs
ms.author: pkrebs
title: 다국어 지원에 대 한 학습 경로 업데이트
ms.date: 05/20/2019
description: 다국어 지원에 대 한 학습 경로 업데이트
ROBOTS: NOINDEX, NOFOLLOW
ms.openlocfilehash: 37a9b77ee45b8ae1ae4973f171c32de11fb530e1
ms.sourcegitcommit: 1f080ed4cf3687f922907304db3fd7a06aa9d501
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/02/2020
ms.locfileid: "45031704"
---
# <a name="update-learning-pathways-for-multilingual-support"></a><span data-ttu-id="36945-103">다국어 지원에 대 한 학습 경로 업데이트</span><span class="sxs-lookup"><span data-stu-id="36945-103">Update learning pathways for multilingual support</span></span>
<span data-ttu-id="36945-104">기존 학습 경로 사이트가 있는 경우 다국어 지원을 위해 해당 사이트를 업데이트할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="36945-104">If you have an existing Learning Pathways site, you can update it for multilingual support.</span></span> <span data-ttu-id="36945-105">다국어 4.0 버전에 대 한 학습 경로를 업데이트 하려면 웹 파트 패키지, customlearning을 SharePoint 테 넌 트 앱 카탈로그에 업로드 합니다.</span><span class="sxs-lookup"><span data-stu-id="36945-105">To update learning pathways to the multilingual 4.0 version, you upload the web part package, customlearning.sppkg, to the SharePoint tenant App Catalog.</span></span> <span data-ttu-id="36945-106">학습 경로를 업데이트할 때는 다음을 수행 합니다.</span><span class="sxs-lookup"><span data-stu-id="36945-106">When you update learning pathways:</span></span>  

- <span data-ttu-id="36945-107">이전에 만든 사용자 지정 재생 목록 및 자산은 모두 유지 관리 됩니다.</span><span class="sxs-lookup"><span data-stu-id="36945-107">Any previously created custom playlists and assets are maintained</span></span>
- <span data-ttu-id="36945-108">콘텐츠를 숨기 거 나 표시 하기 위한 설정이 유지 됩니다.</span><span class="sxs-lookup"><span data-stu-id="36945-108">Settings to hide or show content are maintained</span></span>
- <span data-ttu-id="36945-109">학습 경로 SharePoint 서식 파일이 변경 되지 않은 상태로 유지 됨</span><span class="sxs-lookup"><span data-stu-id="36945-109">The learning pathways SharePoint template is left unchanged</span></span>
- <span data-ttu-id="36945-110">학습 경로 사이트 페이지는 번역 되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="36945-110">The learning pathways site pages aren't translated.</span></span> <span data-ttu-id="36945-111">이 작업을 수동으로 수행 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="36945-111">This work must be done manually</span></span>

## <a name="read-the-learning-pathways-multilingual-overview"></a><span data-ttu-id="36945-112">학습 경로 다국어 개요를 참조 하십시오.</span><span class="sxs-lookup"><span data-stu-id="36945-112">Read the learning pathways multilingual overview</span></span>
<span data-ttu-id="36945-113">다국어 지원이 경로 학습에 작동 하는 방식에 대 한 자세한 내용은 [학습 경로 다국어 개요](custom_overview_ml.md)를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="36945-113">To learn about how multilingual support works for learning pathways, read the [Learning pathways multilingual overview](custom_overview_ml.md)).</span></span> 

## <a name="prerequisites-to-update"></a><span data-ttu-id="36945-114">업데이트할 필수 구성 요소</span><span class="sxs-lookup"><span data-stu-id="36945-114">Prerequisites to update</span></span>
<span data-ttu-id="36945-115">학습 경로를 업데이트 하기 전에 다음 필수 구성 요소를 충족 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="36945-115">Before updating learning pathways, the following prerequisite must be met:</span></span>
- <span data-ttu-id="36945-116">학습 경로를 업데이트 하는 사람은 테 넌 트 앱 카탈로그의 사이트 모음 소유자 여야 합니다.</span><span class="sxs-lookup"><span data-stu-id="36945-116">The person updating learning pathways must be a site collection owner of the tenant App Catalog.</span></span> <span data-ttu-id="36945-117">학습 경로를 프로 비전 하는 사람이 앱 카탈로그의 사이트 모음 소유자가 아닌 경우에는 [이러한 지침을 완료](addappadmin.md) 하 고 계속 진행 합니다.</span><span class="sxs-lookup"><span data-stu-id="36945-117">If the person provisioning learning pathways isn't a site collection owner of the App Catalog, [complete these instructions](addappadmin.md) and continue.</span></span> 

## <a name="set-language-settings"></a><span data-ttu-id="36945-118">언어 설정 설정</span><span class="sxs-lookup"><span data-stu-id="36945-118">Set language settings</span></span> 
<span data-ttu-id="36945-119">학습 경로를 업데이트 하기 전에 사이트 언어 설정을 설정 합니다.</span><span class="sxs-lookup"><span data-stu-id="36945-119">Before updating learning pathways, set the site language settings.</span></span> <span data-ttu-id="36945-120">학습 경로 사이트에 다국어 지원을 사용 하도록 설정 하려면 **페이지 및 뉴스를 여러 언어로 번역할 수 있도록** 설정한 다음 해당 사이트에 대해 지원할 **언어를 추가**합니다.</span><span class="sxs-lookup"><span data-stu-id="36945-120">To enable multilingual support for the learning pathways site, you can set the **Enable pages and news to be translated into multiple languages** to **On**, and then add the languages you want to support for the site.</span></span>
1.  <span data-ttu-id="36945-121">학습 경로 사이트의 오른쪽 위에서 **설정을** 선택한 다음 **사이트 정보**를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="36945-121">From the Learning Pathways site, select **Settings** from the top right, and then select **Site information**.</span></span>
2.  <span data-ttu-id="36945-122">사이트 정보 창 아래쪽에서 **모든 사이트 설정 보기**를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="36945-122">At the bottom of the site information pane, select **View all site settings**.</span></span>
3.  <span data-ttu-id="36945-123">**사이트 관리**에서 **언어 설정을**선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="36945-123">Under **Site Administration**, select **Language settings**.</span></span>
4.  <span data-ttu-id="36945-124">**페이지 및 뉴스를 여러 언어로 번역할 수 있도록**설정 아래에서 toggle 스위치를 설정 합니다.</span><span class="sxs-lookup"><span data-stu-id="36945-124">Under **Enable pages and news to be translated into multiple languages**, set the toggle switch.</span></span> 
- <span data-ttu-id="36945-125">Multiligual 사이트의 경우 켜기/끄기를 설정 **으로 슬라이드**를 연 다음 언어 추가 섹션으로 이동 합니다.</span><span class="sxs-lookup"><span data-stu-id="36945-125">For a multiligual site, slide the toggle to **On**, and then proceed to the Add Languages section.</span></span> 
- <span data-ttu-id="36945-126">영어 전용 사이트의 경우이 기능을 **해제**로 슬라이드 전환 합니다.</span><span class="sxs-lookup"><span data-stu-id="36945-126">For an English-only site, slide the toggle to **Off**.</span></span>

### <a name="add-languages"></a><span data-ttu-id="36945-127">언어 추가</span><span class="sxs-lookup"><span data-stu-id="36945-127">Add languages</span></span>
<span data-ttu-id="36945-128">학습 경로에서는 9 개의 언어를 지원 하므로 필요한 언어만 추가 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="36945-128">Learning pathways supports nine languages, you should add only the languages you need.</span></span> <span data-ttu-id="36945-129">이 설명서에 사용 된 예에서는 이탈리아어가 추가 됩니다.</span><span class="sxs-lookup"><span data-stu-id="36945-129">In the examples used in this documentation, Italian will be added.</span></span> 
- <span data-ttu-id="36945-130">**사이트 언어 추가 또는 제거**에서 언어 이름 입력을 시작 **하거나 언어를 입력**하거나 드롭다운 목록에서 언어를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="36945-130">Under **Add or remove site languages**, start typing a language name in **Select or type a language**, or choose a language from the dropdown.</span></span> <span data-ttu-id="36945-131">이 단계를 반복 하 여 여러 언어를 추가할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="36945-131">You can repeat this step to add multiple languages.</span></span> <span data-ttu-id="36945-132">언제 든 지이 페이지로 다시 이동 하 여 사이트에서 언어를 추가 하거나 제거할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="36945-132">You can add or remove languages from your site at any time by going back to this page.</span></span>
 
### <a name="assign-translators"></a><span data-ttu-id="36945-133">번역기 지정</span><span class="sxs-lookup"><span data-stu-id="36945-133">Assign translators</span></span>
<span data-ttu-id="36945-134">학습 경로의 언어 설정을 정의할 때 번역기를 할당할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="36945-134">When defining Language settings for learning pathways, you can assign translators.</span></span> <span data-ttu-id="36945-135">번역자에 게는 외국어 프로필이 설정 되어 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="36945-135">Translators should have a foreign language profile set up.</span></span> <span data-ttu-id="36945-136">외국 언어 프로필에 대 한 자세한 내용은 [다국어 통신 사이트, 페이지 및 뉴스 만들기](https://support.office.com/article/2bb7d610-5453-41c6-a0e8-6f40b3ed750c)를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="36945-136">For more information about foreign language profiles, see [Create multilingual communication sites, pages, and news](https://support.office.com/article/2bb7d610-5453-41c6-a0e8-6f40b3ed750c).</span></span>  
- <span data-ttu-id="36945-137">지원 되는 언어의 경우에는 **선택을 클릭 하거나 번역기를 입력** 한 다음 번역기를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="36945-137">For a supported language, click **Select or type a translator** and then select a translator.</span></span> 

## <a name="update-the-learning-pathways-web-part-package"></a><span data-ttu-id="36945-138">학습 경로 웹 파트 패키지 업데이트</span><span class="sxs-lookup"><span data-stu-id="36945-138">Update the learning pathways web part package</span></span>
<span data-ttu-id="36945-139">이 단계에서는 학습 경로 4.0 웹 파트를 SharePoint 앱 카탈로그에 업로드 한 다음, 학습 경로 관리 페이지로 이동 하 여 업데이트 프로세스를 시작 합니다.</span><span class="sxs-lookup"><span data-stu-id="36945-139">In this step, you upload the learning pathways 4.0 web part to the SharePoint App Catalog, and then navigate to the learning pathways Administration page to start the update process.</span></span>

### <a name="upload-the-web-part-package"></a><span data-ttu-id="36945-140">웹 파트 패키지 업로드</span><span class="sxs-lookup"><span data-stu-id="36945-140">Upload the web part package</span></span>
1.  <span data-ttu-id="36945-141">팀의 다국어 공유 위치로 이동 하 고 PC의 로컬 드라이브에 **helloworld-webpart.sppkg** 를 다운로드 합니다.</span><span class="sxs-lookup"><span data-stu-id="36945-141">Go to the multilingual share location in Teams and download **customlearning.sppkg** to a local drive on your PC.</span></span> 
2.  <span data-ttu-id="36945-142">아직 로그인 하지 않은 경우 테 넌 트 관리 또는 사이트 모음 관리자 계정을 사용 하 여 테 넌 트에 로그인 합니다.</span><span class="sxs-lookup"><span data-stu-id="36945-142">If you’re not already signed in, sign into your tenant with a Tenant Admin or Site Collection Admin account.</span></span> 
3.  <span data-ttu-id="36945-143">**관리**  >  **모든**  >  **SharePoint**  >  **추가 기능**표시를 클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="36945-143">Click **Admin** > **Show All** > **SharePoint** > **More Features**.</span></span> 
4.  <span data-ttu-id="36945-144">**앱**에서 **열기**를 클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="36945-144">Under **Apps**, click **Open**.</span></span> 
5.  <span data-ttu-id="36945-145">**앱 카탈로그**  >  **배포 앱 for SharePoint를**클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="36945-145">Click **App Catalog** > **Distribute Apps for SharePoint**.</span></span> 
6.  <span data-ttu-id="36945-146">**Upload**  >  **파일 선택을**업로드 합니다 .를 클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="36945-146">Click **Upload** > **Choose Files**.</span></span> 
7.  <span data-ttu-id="36945-147">다운로드 한 **customlearning** 파일을 선택 하 고 **확인**  >  **배포**를 클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="36945-147">Select the **customlearning.sppkg** file you downloaded, click **OK** > **Deploy**.</span></span> 

### <a name="complete-the-update"></a><span data-ttu-id="36945-148">업데이트 완료</span><span class="sxs-lookup"><span data-stu-id="36945-148">Complete the update</span></span>
1.  <span data-ttu-id="36945-149">학습 경로 사이트의 **홈** 메뉴에서 **학습 경로 관리** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="36945-149">From the Learning Pathways site, select **Learning pathways administration** from the **Home** menu.</span></span> 
2.  <span data-ttu-id="36945-150">업데이트할 것인지 묻는 메시지가 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="36945-150">You’ll see a prompt asking if you want to update.</span></span> 
<span data-ttu-id="36945-151">![custom_update_adminprompt_ml.png](media/custom_update_adminprompt_ml.png)</span><span class="sxs-lookup"><span data-stu-id="36945-151">![custom_update_adminprompt_ml.png](media/custom_update_adminprompt_ml.png)</span></span>
3.  <span data-ttu-id="36945-152">**시작**을 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="36945-152">Click **Start**.</span></span> 
4. <span data-ttu-id="36945-153">업데이트가 완료 되 면 **닫기를**클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="36945-153">When the update is complete, click **Close**.</span></span> 

### <a name="next-steps"></a><span data-ttu-id="36945-154">다음 단계</span><span class="sxs-lookup"><span data-stu-id="36945-154">Next Steps</span></span>
- <span data-ttu-id="36945-155">사이트 및 웹 파트에서 제공 되는 [기본 콘텐츠](custom_exploresite.md) 를 살펴봅니다.</span><span class="sxs-lookup"><span data-stu-id="36945-155">Explore the [default content](custom_exploresite.md) provided in the site and web part.</span></span>
- <span data-ttu-id="36945-156">사이트 페이지 번역에 대 한 자세한 내용은 [번역 사이트 페이지](custom_translate_page_ml.md)를 참조 하십시오.</span><span class="sxs-lookup"><span data-stu-id="36945-156">For more information about translating site pages, see [Translate site pages](custom_translate_page_ml.md).</span></span> 

