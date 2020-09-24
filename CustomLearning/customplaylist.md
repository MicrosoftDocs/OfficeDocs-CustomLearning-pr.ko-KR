---
author: karuanag
ms.author: karuanag
title: 재생 목록 사용자 지정 및 공유
ms.date: 02/10/2019
description: 기존 콘텐츠 또는 새 SharePoint 페이지에서 사용자 지정 재생 목록 만들기
ms.service: sharepoint online
ms.openlocfilehash: 6258668b417ba496c7ac75e36ce2bc1f1dae27a5
ms.sourcegitcommit: ee4aebf60893887ae95a1294a9ad8975539ea762
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/23/2020
ms.locfileid: "48233810"
---
# <a name="customize-and-share-playlists"></a><span data-ttu-id="fe3e6-103">재생 목록 사용자 지정 및 공유</span><span class="sxs-lookup"><span data-stu-id="fe3e6-103">Customize and Share Playlists</span></span>

## <a name="create-a-playlist"></a><span data-ttu-id="fe3e6-104">재생 목록 만들기</span><span class="sxs-lookup"><span data-stu-id="fe3e6-104">Create a Playlist</span></span>

<span data-ttu-id="fe3e6-105">재생 목록은 "자산"의 compliation.</span><span class="sxs-lookup"><span data-stu-id="fe3e6-105">A playlist is a compliation of "assets".</span></span> <span data-ttu-id="fe3e6-106">"자산"은 SharePoint 페이지 또는 Microsoft 교육 콘텐츠의 기존 항목입니다.</span><span class="sxs-lookup"><span data-stu-id="fe3e6-106">An "asset" is a SharePoint page or existing item of Microsoft training content.</span></span> <span data-ttu-id="fe3e6-107">재생 목록을 만들 때 함께 이동 하는 자산을 선택 하 여 사용자에 대 한 학습 경로를 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="fe3e6-107">When you create a playlist you select assets that go together to create a learning path for your user.</span></span>  

<span data-ttu-id="fe3e6-108">SharePoint 페이지를 추가할 때의 이점은 조직에서 호스트 되는 YouTube 비디오 또는 비디오를 사용 하 여 SharePoint 페이지를 만들 수 있다는 것입니다.</span><span class="sxs-lookup"><span data-stu-id="fe3e6-108">The benefit of adding SharePoint pages is that you can create SharePoint pages with a YouTube videos or videos hosted in your organization.</span></span> <span data-ttu-id="fe3e6-109">양식 또는 기타 Office 365 콘텐츠가 포함 된 페이지를 만들 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="fe3e6-109">You can also create pages with Forms or other Office 365 content.</span></span>  

#### <a name="step-1-create-a-sharepoint-page-for-your-playlist"></a><span data-ttu-id="fe3e6-110">1 단계: 재생 목록에 대 한 SharePoint 페이지 만들기</span><span class="sxs-lookup"><span data-stu-id="fe3e6-110">Step 1: Create a SharePoint page for your playlist</span></span>
<span data-ttu-id="fe3e6-111">이 예제에서는 먼저 재생 목록에 추가할 SharePoint 페이지를 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="fe3e6-111">In this example, we’ll first create a SharePoint page to add to the playlist.</span></span> <span data-ttu-id="fe3e6-112">YouTube 비디오 웹 파트 및 텍스트 웹 파트가 포함 된 페이지를 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="fe3e6-112">We’ll create a page with a YouTube video web part and Text web part.</span></span>  <span data-ttu-id="fe3e6-113">이 지침에서는 SharePoint Online 서비스를 사용 하 고 있다고 가정 합니다.</span><span class="sxs-lookup"><span data-stu-id="fe3e6-113">These instructions assume you are using the SharePoint Online service.</span></span> 

#### <a name="create-a-new-page"></a><span data-ttu-id="fe3e6-114">새 페이지 만들기</span><span class="sxs-lookup"><span data-stu-id="fe3e6-114">Create a new page</span></span>
1.  <span data-ttu-id="fe3e6-115">사이트 콘텐츠 > 사이트 페이지 > 새 > 사이트 페이지 > 설정 메뉴를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="fe3e6-115">Select the Settings menu > Site Contents > Site Pages > New > Site Page.</span></span>
2.  <span data-ttu-id="fe3e6-116">제목 영역에 팀 명령 사용 상자를 입력 합니다.</span><span class="sxs-lookup"><span data-stu-id="fe3e6-116">In the title area, type Use the Teams command box</span></span>
3.  <span data-ttu-id="fe3e6-117">새 섹션 추가를 선택 하 고 두 개의 열을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="fe3e6-117">Select the Add a new section, and then select Two Columns.</span></span>

![2 열 추가](media/clo365addtwocolumn.png)

4.  <span data-ttu-id="fe3e6-119">왼쪽 상자에서 새 웹 파트 추가를 선택 하 고 포함을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="fe3e6-119">In the left-hand box, select Add a new web part, and then select Embed.</span></span> 
5.  <span data-ttu-id="fe3e6-120">웹 브라우저에서이 URL로 이동 하 여 https://youtu.be/wYrRCRphrp0 비디오에 대 한 embed 태그를 가져옵니다.</span><span class="sxs-lookup"><span data-stu-id="fe3e6-120">In a Web browser, go to this URL https://youtu.be/wYrRCRphrp0 and get the embed code for the video.</span></span> 
6.  <span data-ttu-id="fe3e6-121">SharePoint 웹 파트에서 Embed 태그 추가를 선택 하 여 포함 상자에 붙여 넣습니다.</span><span class="sxs-lookup"><span data-stu-id="fe3e6-121">In the SharePoint Web part, select Add Embed code and then paste it into the Embed box.</span></span> 
7.  <span data-ttu-id="fe3e6-122">오른쪽 상자에서 새 웹 파트 추가를 선택한 다음 텍스트를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="fe3e6-122">In the right-hand box, select Add a new web part, and then select Text.</span></span> 
8.  <span data-ttu-id="fe3e6-123">웹 브라우저에서 다음 URL로 이동 하 여 https://support.office.com/article/13c4e429-7324-4886-b377-5dbed539193b Try!</span><span class="sxs-lookup"><span data-stu-id="fe3e6-123">In a Web browser, go to this URL: https://support.office.com/article/13c4e429-7324-4886-b377-5dbed539193b and copy the Try it!</span></span> <span data-ttu-id="fe3e6-124">지침을 선택한 다음 텍스트 웹 파트에 붙여 넣습니다.</span><span class="sxs-lookup"><span data-stu-id="fe3e6-124">Instructions from the page and paste them into the Text Web part.</span></span> <span data-ttu-id="fe3e6-125">페이지 모양은 다음과 같습니다.</span><span class="sxs-lookup"><span data-stu-id="fe3e6-125">Your page should look like the following.</span></span> 

![페이지 포함](media/clo365teamscommandbox.png)

9.  <span data-ttu-id="fe3e6-127">**게시**를 클릭 한 다음 페이지의 URL을 복사 하 여 메모장에 붙여넣기</span><span class="sxs-lookup"><span data-stu-id="fe3e6-127">Click **Publish**, and then copy the URL of the page and paste it in Notepad</span></span>

#### <a name="step-2-create-the-playlist"></a><span data-ttu-id="fe3e6-128">2 단계: 재생 목록 만들기</span><span class="sxs-lookup"><span data-stu-id="fe3e6-128">Step 2: Create the Playlist</span></span>

1. <span data-ttu-id="fe3e6-129">사이트 환경에서 **사용자 지정 학습 관리** 페이지로 이동 합니다.</span><span class="sxs-lookup"><span data-stu-id="fe3e6-129">Navigate to the **Custom Learning Administration** page in your site experience.</span></span>
<span data-ttu-id="fe3e6-130">![custom_admin.png](media/custom_admin.png)</span><span class="sxs-lookup"><span data-stu-id="fe3e6-130">![custom_admin.png](media/custom_admin.png)</span></span>
1. <span data-ttu-id="fe3e6-131">**범주가** 선택 되어 있는지 확인</span><span class="sxs-lookup"><span data-stu-id="fe3e6-131">Make sure **Category** is selected</span></span> 
1. <span data-ttu-id="fe3e6-132">새 재생 목록을 표시할 범주를 클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="fe3e6-132">Click on the category where you'd like your new playlist to appear</span></span>
1. <span data-ttu-id="fe3e6-133">범주 이름 옆에 있는 더하기 기호를 클릭 ![custom_addplay.png](media/custom_addplay.png)</span><span class="sxs-lookup"><span data-stu-id="fe3e6-133">Next to the category name, click on the plus symbol ![custom_addplay.png](media/custom_addplay.png)</span></span>

1. <span data-ttu-id="fe3e6-134">아래 예제와 같이 값을 입력 하 고 **만들기**를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="fe3e6-134">Fill in the values as shown in the example below and select **Create**.</span></span> 
<span data-ttu-id="fe3e6-135">![custom_details.png](media/custom_details.png)</span><span class="sxs-lookup"><span data-stu-id="fe3e6-135">![custom_details.png](media/custom_details.png)</span></span>
- <span data-ttu-id="fe3e6-136">**제목** -재생 목록의 표시 이름입니다.</span><span class="sxs-lookup"><span data-stu-id="fe3e6-136">**Title** - Display name of the playlist</span></span>
- <span data-ttu-id="fe3e6-137">**Description** -배우게 되는 사항에 대 한 정보입니다.</span><span class="sxs-lookup"><span data-stu-id="fe3e6-137">**Description** - Information about what will be learned</span></span>
- <span data-ttu-id="fe3e6-138">**범주** -초기 선택을 기준으로 미리 선택 됩니다.</span><span class="sxs-lookup"><span data-stu-id="fe3e6-138">**Category** - Preselected based on your initial selection</span></span>
- <span data-ttu-id="fe3e6-139">**하위 범주** -초기 선택을 기준으로 미리 선택</span><span class="sxs-lookup"><span data-stu-id="fe3e6-139">**Sub Category** - Preselected based on your intial selection</span></span>
- <span data-ttu-id="fe3e6-140">**기술** -해당 되는 경우 선택</span><span class="sxs-lookup"><span data-stu-id="fe3e6-140">**Technology** - Select as applicable</span></span>
- <span data-ttu-id="fe3e6-141">**만추** -초급, Intermidate 또는 Advanced</span><span class="sxs-lookup"><span data-stu-id="fe3e6-141">**Level** - Beginner, Intermidate or Advanced</span></span>
- <span data-ttu-id="fe3e6-142">**대상 그룹** -Microsoft에서 제공 하는 미리 정의 된 역할 목록을 기반으로 콘텐츠를 대상으로 지정할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="fe3e6-142">**Audience** - This allows you to target content based on a pre-defined list of roles provided by Microsoft.</span></span>

6. <span data-ttu-id="fe3e6-143">**세부 정보 저장** 을 클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="fe3e6-143">Click **Save Detail**</span></span>

> [!TIP]
> <span data-ttu-id="fe3e6-144">재생 목록의 아이콘 이미지를 사용자 지정할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="fe3e6-144">You can customize the icon image for your playlist.</span></span>  <span data-ttu-id="fe3e6-145">이미지 아이콘을 클릭 하 고 이전에 업로드 한 이미지의 URL을 삽입 합니다.</span><span class="sxs-lookup"><span data-stu-id="fe3e6-145">Click the image icon and insert an URL of a previously uploaded image.</span></span>  <span data-ttu-id="fe3e6-146">이미지가 사용자 지정 학습 사이트 모음에 위치 하거나 모든 사용자가 해당 파일에 액세스할 수 있는 다른 위치에 있는지 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="fe3e6-146">Make sure the image is located within the Custom Learning site collection or in another location that all users will have access to the file.</span></span>  
<span data-ttu-id="fe3e6-147">![custom_image.png](media/custom_image.png)</span><span class="sxs-lookup"><span data-stu-id="fe3e6-147">![custom_image.png](media/custom_image.png)</span></span>

#### <a name="step-3-add-assets-to-the-playlist"></a><span data-ttu-id="fe3e6-148">3 단계: 재생 목록에 에셋 추가</span><span class="sxs-lookup"><span data-stu-id="fe3e6-148">Step 3: Add assets to the playlist</span></span>
<span data-ttu-id="fe3e6-149">이 단계에서는 Microsoft 및 만든 SharePoint 페이지의 기존 자산을 재생 목록에 추가 합니다.</span><span class="sxs-lookup"><span data-stu-id="fe3e6-149">In this step, you’ll add existing assets from Microsoft and the SharePoint page you created to the playlist.</span></span> 

1. <span data-ttu-id="fe3e6-150">재생 목록에 대 한 세부 정보를 저장 한 후에는 기존 자산 검색을 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="fe3e6-150">Once you have saved the details for your Playlist you can use the Search for Existing Assets.</span></span>
1. <span data-ttu-id="fe3e6-151">**검색 용어를 입력** 하 여 다른 재생 목록에서 사용할 수 있는 미리 정의 된 자산의 목록을 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="fe3e6-151">**Enter in any search term** to see a list of predefined assets that are available from other playlists.</span></span> <span data-ttu-id="fe3e6-152">자산 **이름을 클릭** 하 여 새 재생 목록에 포함 합니다.</span><span class="sxs-lookup"><span data-stu-id="fe3e6-152">**Click on the name** of an asset to include it in your new playlist.</span></span>
<span data-ttu-id="fe3e6-153">![custom_slist.png](media/custom_slist.png)</span><span class="sxs-lookup"><span data-stu-id="fe3e6-153">![custom_slist.png](media/custom_slist.png)</span></span>

<span data-ttu-id="fe3e6-154">이전에 만든 SharePoint 페이지를 추가 하거나 환경에서 처음부터 새로 만들 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="fe3e6-154">You can also add the SharePoint page you created earlier or create one from scratch in the experience.</span></span>

1. <span data-ttu-id="fe3e6-155">재생 목록 자산 대화 상자에서 **새 자산** 옵션을 클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="fe3e6-155">Click on the **New Asset** option in the Playlist Assets dialog</span></span>
1. <span data-ttu-id="fe3e6-156">자산에 **제목을**지정 합니다.</span><span class="sxs-lookup"><span data-stu-id="fe3e6-156">Give your asset a **Title**.</span></span> <span data-ttu-id="fe3e6-157">입력 한 추가 옵션은custom_newpage.png표시 됩니다. ![](media/custom_newpage.png)</span><span class="sxs-lookup"><span data-stu-id="fe3e6-157">Once entered, additional options will display ![custom_newpage.png](media/custom_newpage.png)</span></span>
1. <span data-ttu-id="fe3e6-158">이제 SharePoint Online에서 새 자산 페이지를 만들거나 기존 페이지의 URL을 입력 하 여 사용자 지정 재생 목록에 추가할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="fe3e6-158">You can now create a new asset page in SharePoint Online or enter in the URL of an existing page to add it to your custom playlist.</span></span> 
1. <span data-ttu-id="fe3e6-159">**범주**, **하위 범주** 및 **기술** 필드는이 재생 목록에 대 한 이전 선택 항목에 따라 미리 채워집니다.</span><span class="sxs-lookup"><span data-stu-id="fe3e6-159">**Category**, **Sub Category** and **Technology** fields will be pre-populated based on your previous selections for this playlist.</span></span>
1. <span data-ttu-id="fe3e6-160">이 개별 자산의 수준 및 대상 그룹을 적절 하 게 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="fe3e6-160">Make the appropriate selections for Level and Audience for this individual asset.</span></span>  
1. <span data-ttu-id="fe3e6-161">**자산 저장** 을 클릭 하 여 사용자 지정 재생 목록에 추가 합니다.</span><span class="sxs-lookup"><span data-stu-id="fe3e6-161">Click **Save Asset** to add it to the custom playlist</span></span>
1. <span data-ttu-id="fe3e6-162">재생 목록이 완료 될 때까지 개별 페이지를 검색 하거나 추가 하 여이 단계를 반복 합니다.</span><span class="sxs-lookup"><span data-stu-id="fe3e6-162">Repeat these steps, either searching or adding individual pages, until your playlist is complete.</span></span> 
1. <span data-ttu-id="fe3e6-163">**재생 목록 닫기** 를 클릭 하 여 저장</span><span class="sxs-lookup"><span data-stu-id="fe3e6-163">Click **Close Playlist** to save</span></span>

<span data-ttu-id="fe3e6-164">이 콘텐츠를 포함 하는 재생 목록은 사용자 지정 학습 웹 파트를 설치/포함 한 모든 위치에서 사용할 수 있게 됩니다.</span><span class="sxs-lookup"><span data-stu-id="fe3e6-164">Your playlist with this content will now be available anywhere you have installed / embedded the Custom Learning webpart.</span></span> 

> [!NOTE]
> <span data-ttu-id="fe3e6-165">재생 목록을 닫은 후 실수를 한 경우 재생 목록 이름 옆에 있는 X를 클릭 하 여 범주에서 삭제할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="fe3e6-165">If you make a mistake once you have closed the playlist, you can delete it from the category by clicking the X next to the playlist name.</span></span>  

#### <a name="things-to-think-about"></a><span data-ttu-id="fe3e6-166">고려해 야 할 사항</span><span class="sxs-lookup"><span data-stu-id="fe3e6-166">Things to Think About</span></span>

<span data-ttu-id="fe3e6-167">사용자 지정 재생 목록을 사용 하 여 최종 사용자가 다양 한 작업을 지원할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="fe3e6-167">Custom playlists can be used to assist your end users in a variety of tasks.</span></span>  <span data-ttu-id="fe3e6-168">휴가 요청 양식이 있습니까?</span><span class="sxs-lookup"><span data-stu-id="fe3e6-168">Do you have a time off request form?</span></span>  <span data-ttu-id="fe3e6-169">하드웨어 장비를 요청 하는 양식</span><span class="sxs-lookup"><span data-stu-id="fe3e6-169">A form to request hardware equipment?</span></span>  <span data-ttu-id="fe3e6-170">모든 기존 교육 자산이 환경에 프로그래밍 될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="fe3e6-170">Any existing training assets can be programmed into the experience.</span></span>  

## <a name="share-playlists"></a><span data-ttu-id="fe3e6-171">재생 목록 공유</span><span class="sxs-lookup"><span data-stu-id="fe3e6-171">Share Playlists</span></span>

1. <span data-ttu-id="fe3e6-172">웹 파트 또는 사이트 환경 내의 재생 목록으로 이동</span><span class="sxs-lookup"><span data-stu-id="fe3e6-172">Navigate to any playlist within the webpart or site experience</span></span>
1. <span data-ttu-id="fe3e6-173">왼쪽 위 모서리에 세 개의 아이콘이 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="fe3e6-173">In the upper left hand corner you will see three icons</span></span>
1. <span data-ttu-id="fe3e6-174">링크를 나타내는 아이콘을 클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="fe3e6-174">Click on the icon representing a link</span></span>
1. <span data-ttu-id="fe3e6-175">재생 목록에 URL 복사</span><span class="sxs-lookup"><span data-stu-id="fe3e6-175">Copy the URL to the playlist</span></span>

<span data-ttu-id="fe3e6-176">![share.png](media/share.png) 이제이 URL을 사이트 탐색에 삽입 하거나 다른 통신에서 사용 하 여 직원을 해당 재생 목록으로 바로 이동할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="fe3e6-176">![share.png](media/share.png) This URL can now be inserted in your site navigation or utilized in other communications to take your employees directly to that playlist.</span></span> 

### <a name="next-steps---drive-adoption"></a><span data-ttu-id="fe3e6-177">다음 단계- [드라이브 도입](driveadoption.md)</span><span class="sxs-lookup"><span data-stu-id="fe3e6-177">Next Steps - [Drive Adoption](driveadoption.md)</span></span>
