---
author: pkrebs
ms.author: pkrebs
title: Microsoft 365 학습 경로 업데이트
ms.date: 07/06/2020
description: Microsoft 365 학습 경로 업데이트
ms.service: sharepoint-online
manager: bpardi
ms.topic: article
audience: admin
ms.openlocfilehash: 324bf41df1a6eec8d4646f3affdd48bedbbe3252
ms.sourcegitcommit: 97e175e5ff5b6a9e0274d5ec9b39fdf7e18eb387
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/25/2021
ms.locfileid: "52000344"
---
# <a name="update-learning-pathways"></a><span data-ttu-id="5c4bf-103">학습 경로 업데이트</span><span class="sxs-lookup"><span data-stu-id="5c4bf-103">Update learning pathways</span></span>
<span data-ttu-id="5c4bf-104">기존 학습 경로 사이트가 있는 경우 다국어 지원을 위해 업데이트할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="5c4bf-104">If you have an existing Learning Pathways site, you can update it for multilingual support.</span></span> <span data-ttu-id="5c4bf-105">다국어 4.0 버전으로 학습 경로를 업데이트하려면 웹 파트 패키지 customlearning.sppkg를 SharePoint 테넌트 앱 카탈로그에 업로드합니다.</span><span class="sxs-lookup"><span data-stu-id="5c4bf-105">To update learning pathways to the multilingual 4.0 version, you upload the web part package, customlearning.sppkg, to the SharePoint tenant App Catalog.</span></span> <span data-ttu-id="5c4bf-106">학습 경로를 업데이트하는 경우:</span><span class="sxs-lookup"><span data-stu-id="5c4bf-106">When you update learning pathways:</span></span>  

- <span data-ttu-id="5c4bf-107">이전에 만든 모든 사용자 지정 재생 목록 및 자산은 유지 관리됩니다.</span><span class="sxs-lookup"><span data-stu-id="5c4bf-107">Any previously created custom playlists and assets are maintained</span></span>
- <span data-ttu-id="5c4bf-108">콘텐츠를 숨기거나 표시하는 설정이 유지 관리됩니다.</span><span class="sxs-lookup"><span data-stu-id="5c4bf-108">Settings to hide or show content are maintained</span></span>
- <span data-ttu-id="5c4bf-109">학습 경로 SharePoint 서식 파일은 변경되지 않은 것으로 남아 있습니다.</span><span class="sxs-lookup"><span data-stu-id="5c4bf-109">The learning pathways SharePoint template is left unchanged</span></span>
- <span data-ttu-id="5c4bf-110">학습 경로 사이트 페이지는 번역되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="5c4bf-110">The learning pathways site pages aren't translated.</span></span> <span data-ttu-id="5c4bf-111">이 작업을 수동으로 완료해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="5c4bf-111">This work must be done manually</span></span>

## <a name="read-the-learning-pathways-multilingual-overview"></a><span data-ttu-id="5c4bf-112">학습 경로 다국어 개요 읽기</span><span class="sxs-lookup"><span data-stu-id="5c4bf-112">Read the learning pathways multilingual overview</span></span>
<span data-ttu-id="5c4bf-113">학습 경로에 다국어 지원이 작동하는 방식에 대한 자세한 내용은 학습 경로 다국어 [개요 를 참조하세요.](custom_overview.md)</span><span class="sxs-lookup"><span data-stu-id="5c4bf-113">To learn about how multilingual support works for learning pathways, read the [Learning pathways multilingual overview](custom_overview.md).</span></span> 

## <a name="prerequisites-to-update"></a><span data-ttu-id="5c4bf-114">업데이트할 선행 준비</span><span class="sxs-lookup"><span data-stu-id="5c4bf-114">Prerequisites to update</span></span>
<span data-ttu-id="5c4bf-115">학습 경로를 업데이트하기 전에 다음 선행 준비를 충족해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="5c4bf-115">Before updating learning pathways, the following prerequisite must be met:</span></span>
- <span data-ttu-id="5c4bf-116">학습 경로를 업데이트하는 사람은 테넌트 앱 카탈로그의 사이트 모음 소유자가 되어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="5c4bf-116">The person updating learning pathways must be a site collection owner of the tenant App Catalog.</span></span> <span data-ttu-id="5c4bf-117">학습 경로를 프로비저닝하는 사용자가 앱 카탈로그의 사이트 모음 소유자가 아닌 경우 이러한 [지침을 완료하고](addappadmin.md) 계속합니다.</span><span class="sxs-lookup"><span data-stu-id="5c4bf-117">If the person provisioning learning pathways isn't a site collection owner of the App Catalog, [complete these instructions](addappadmin.md) and continue.</span></span> 

## <a name="set-language-settings"></a><span data-ttu-id="5c4bf-118">언어 설정 설정</span><span class="sxs-lookup"><span data-stu-id="5c4bf-118">Set language settings</span></span> 
<span data-ttu-id="5c4bf-119">학습 경로를 업데이트하기 전에 사이트 언어 설정을 설정하십시오.</span><span class="sxs-lookup"><span data-stu-id="5c4bf-119">Before updating learning pathways, set the site language settings.</span></span> <span data-ttu-id="5c4bf-120">학습 경로 사이트에 대한 다국어 지원을 사용하도록 설정하려면  페이지 및 뉴스를 여러 언어로 번역할 수 있도록 설정을 **으로** 설정한 다음 사이트에 대해 지원할 언어를 추가할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="5c4bf-120">To enable multilingual support for the learning pathways site, you can set the **Enable pages and news to be translated into multiple languages** to **On**, and then add the languages you want to support for the site.</span></span>
1.  <span data-ttu-id="5c4bf-121">학습 경로 사이트에서 오른쪽 상단의 설정을 선택한 다음 사이트 **정보를 선택합니다.** </span><span class="sxs-lookup"><span data-stu-id="5c4bf-121">From the Learning Pathways site, select **Settings** from the top right, and then select **Site information**.</span></span>
2.  <span data-ttu-id="5c4bf-122">사이트 정보 창의 아래쪽에서 모든 사이트 설정 보기 **를 선택합니다.**</span><span class="sxs-lookup"><span data-stu-id="5c4bf-122">At the bottom of the site information pane, select **View all site settings**.</span></span>
3.  <span data-ttu-id="5c4bf-123">사이트 **관리에서** 언어 **설정을 선택합니다.**</span><span class="sxs-lookup"><span data-stu-id="5c4bf-123">Under **Site Administration**, select **Language settings**.</span></span>
4.  <span data-ttu-id="5c4bf-124">페이지 **및 뉴스를 여러** 언어로 번역할 수 있도록 설정에서 토글 스위치를 설정하십시오.</span><span class="sxs-lookup"><span data-stu-id="5c4bf-124">Under **Enable pages and news to be translated into multiple languages**, set the toggle switch.</span></span> 
- <span data-ttu-id="5c4bf-125">다국어 사이트의 경우 토글을 **으로** 밀고 언어 추가 섹션으로 진행합니다.</span><span class="sxs-lookup"><span data-stu-id="5c4bf-125">For a multiligual site, slide the toggle to **On**, and then proceed to the Add Languages section.</span></span> 
- <span data-ttu-id="5c4bf-126">영어 전용 사이트의 경우 해제로 **토글합니다.**</span><span class="sxs-lookup"><span data-stu-id="5c4bf-126">For an English-only site, slide the toggle to **Off**.</span></span>

### <a name="add-languages"></a><span data-ttu-id="5c4bf-127">언어 추가</span><span class="sxs-lookup"><span data-stu-id="5c4bf-127">Add languages</span></span>
<span data-ttu-id="5c4bf-128">학습 경로는 9개 언어를 지원하고 필요한 언어만 추가해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="5c4bf-128">Learning pathways supports nine languages, you should add only the languages you need.</span></span> <span data-ttu-id="5c4bf-129">이 설명서에 사용된 예제에서 이탈리아어가 추가됩니다.</span><span class="sxs-lookup"><span data-stu-id="5c4bf-129">In the examples used in this documentation, Italian will be added.</span></span> 
- <span data-ttu-id="5c4bf-130">사이트 언어 추가 **또는 제거에서** 언어 선택 또는 입력에 언어 이름을 입력하거나 **드롭다운에서** 언어를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="5c4bf-130">Under **Add or remove site languages**, start typing a language name in **Select or type a language**, or choose a language from the dropdown.</span></span> <span data-ttu-id="5c4bf-131">이 단계를 반복하여 여러 언어를 추가할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="5c4bf-131">You can repeat this step to add multiple languages.</span></span> <span data-ttu-id="5c4bf-132">이 페이지로 돌아가서 사이트에서 언어를 추가하거나 제거할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="5c4bf-132">You can add or remove languages from your site at any time by going back to this page.</span></span>
 
### <a name="assign-translators"></a><span data-ttu-id="5c4bf-133">번역자 할당</span><span class="sxs-lookup"><span data-stu-id="5c4bf-133">Assign translators</span></span>
<span data-ttu-id="5c4bf-134">학습 경로에 대한 언어 설정을 정의할 때 번역자를 할당할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="5c4bf-134">When defining Language settings for learning pathways, you can assign translators.</span></span> <span data-ttu-id="5c4bf-135">번역자는 외래 언어 프로필을 설정해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="5c4bf-135">Translators should have a foreign language profile set up.</span></span> <span data-ttu-id="5c4bf-136">외국어 프로필에 대한 자세한 내용은 다국어 통신 사이트, 페이지 및 뉴스 만들기를 [참조하세요.](https://support.office.com/article/2bb7d610-5453-41c6-a0e8-6f40b3ed750c)</span><span class="sxs-lookup"><span data-stu-id="5c4bf-136">For more information about foreign language profiles, see [Create multilingual communication sites, pages, and news](https://support.office.com/article/2bb7d610-5453-41c6-a0e8-6f40b3ed750c).</span></span>  
- <span data-ttu-id="5c4bf-137">지원되는 언어의  경우 선택을 클릭하거나 번역을 입력한 다음 번역을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="5c4bf-137">For a supported language, click **Select or type a translator** and then select a translator.</span></span> 

## <a name="update-the-learning-pathways-web-part-package"></a><span data-ttu-id="5c4bf-138">학습 경로 웹 파트 패키지 업데이트</span><span class="sxs-lookup"><span data-stu-id="5c4bf-138">Update the learning pathways web part package</span></span>
<span data-ttu-id="5c4bf-139">이 단계에서는 학습 경로 4.0 웹 파트를 SharePoint 앱 카탈로그에 업로드한 다음 학습 경로 관리 페이지로 이동하여 업데이트 프로세스를 시작합니다.</span><span class="sxs-lookup"><span data-stu-id="5c4bf-139">In this step, you upload the learning pathways 4.0 web part to the SharePoint App Catalog, and then navigate to the learning pathways Administration page to start the update process.</span></span>

### <a name="upload-the-web-part-package"></a><span data-ttu-id="5c4bf-140">웹 파트 패키지 업로드</span><span class="sxs-lookup"><span data-stu-id="5c4bf-140">Upload the web part package</span></span>
1.  <span data-ttu-id="5c4bf-141">[GitHub](https://github.com/pnp/custom-learning-office-365/tree/master/webpart)사용자 지정 학습 리포지토리로 이동하여 **customlearning.sppkg를** 선택한 다음 PC의 로컬 드라이브에 다운로드합니다.</span><span class="sxs-lookup"><span data-stu-id="5c4bf-141">Go to the [GitHub custom learning repository](https://github.com/pnp/custom-learning-office-365/tree/master/webpart), select **customlearning.sppkg** and then download it to a local drive on your PC.</span></span>
2.  <span data-ttu-id="5c4bf-142">아직 로그인하지 않은 경우 테넌트 관리자 또는 사이트 모음 관리자 계정으로 테넌트에 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="5c4bf-142">If you’re not already signed in, sign into your tenant with a Tenant Admin or Site Collection Admin account.</span></span> 
3.  <span data-ttu-id="5c4bf-143">관리자 **모든**  >  SharePoint **추가** 기능  >  **표시**  >  **를 클릭합니다.**</span><span class="sxs-lookup"><span data-stu-id="5c4bf-143">Click **Admin** > **Show All** > **SharePoint** > **More Features**.</span></span> 
4.  <span data-ttu-id="5c4bf-144">앱에서  **열기 를 클릭합니다.**</span><span class="sxs-lookup"><span data-stu-id="5c4bf-144">Under **Apps**, click **Open**.</span></span> 
5.  <span data-ttu-id="5c4bf-145">  >  **SharePoint용 앱 카탈로그 배포를 클릭합니다.**</span><span class="sxs-lookup"><span data-stu-id="5c4bf-145">Click **App Catalog** > **Distribute Apps for SharePoint**.</span></span> 
6.  <span data-ttu-id="5c4bf-146">파일 **선택**  >  **업로드를 클릭합니다.**</span><span class="sxs-lookup"><span data-stu-id="5c4bf-146">Click **Upload** > **Choose Files**.</span></span> 
7.  <span data-ttu-id="5c4bf-147">다운로드한 **customlearning.sppkg** 파일을 선택하고 확인 **배포를**  >  **클릭합니다.**</span><span class="sxs-lookup"><span data-stu-id="5c4bf-147">Select the **customlearning.sppkg** file you downloaded, click **OK** > **Deploy**.</span></span> 

### <a name="complete-the-update"></a><span data-ttu-id="5c4bf-148">업데이트 완료</span><span class="sxs-lookup"><span data-stu-id="5c4bf-148">Complete the update</span></span>
1.  <span data-ttu-id="5c4bf-149">학습 경로 사이트에서 홈 메뉴에서 학습 **경로** 관리 **를** 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="5c4bf-149">From the Learning Pathways site, select **Learning pathways administration** from the **Home** menu.</span></span> 
2.  <span data-ttu-id="5c4bf-150">업데이트할지 묻는 메시지가 표시될 것입니다.</span><span class="sxs-lookup"><span data-stu-id="5c4bf-150">You’ll see a prompt asking if you want to update.</span></span> 
<span data-ttu-id="5c4bf-151">![업데이트를 시작하라는 메시지가 표시됩니다.](media/custom_update_adminprompt_ml.png)</span><span class="sxs-lookup"><span data-stu-id="5c4bf-151">![Message prompts you to start the update.](media/custom_update_adminprompt_ml.png)</span></span>
3.  <span data-ttu-id="5c4bf-152">**시작** 을 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="5c4bf-152">Click **Start**.</span></span> 
4. <span data-ttu-id="5c4bf-153">업데이트가 완료되면 닫기 **를 클릭합니다.**</span><span class="sxs-lookup"><span data-stu-id="5c4bf-153">When the update is complete, click **Close**.</span></span> 

### <a name="next-steps"></a><span data-ttu-id="5c4bf-154">다음 단계</span><span class="sxs-lookup"><span data-stu-id="5c4bf-154">Next Steps</span></span>
- <span data-ttu-id="5c4bf-155">사이트 [및 웹 파트에](custom_exploresite.md) 제공된 기본 콘텐츠를 살펴보겠습니다.</span><span class="sxs-lookup"><span data-stu-id="5c4bf-155">Explore the [default content](custom_exploresite.md) provided in the site and web part.</span></span>
- <span data-ttu-id="5c4bf-156">사이트 페이지 번역에 대한 자세한 내용은 사이트 페이지 [번역을 참조하세요.](custom_translate_page_ml.md)</span><span class="sxs-lookup"><span data-stu-id="5c4bf-156">For more information about translating site pages, see [Translate site pages](custom_translate_page_ml.md).</span></span> 

