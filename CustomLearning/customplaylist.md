---
author: karuanag
ms.author: karuanag
title: 재생 목록 사용자 지정 및 공유
ms.date: 02/10/2019
description: 기존 콘텐츠 또는 새 SharePoint 페이지에서 사용자 지정 재생 목록 만들기
ms.openlocfilehash: d330b6e401c9020eb68877bc8a132350811a2f31
ms.sourcegitcommit: e10085e60ca3f38029fde229fb093e6bc4a34203
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 02/25/2019
ms.locfileid: "29989729"
---
# <a name="customize-and-share-playlists"></a><span data-ttu-id="c581b-103">재생 목록 사용자 지정 및 공유</span><span class="sxs-lookup"><span data-stu-id="c581b-103">Customize and Share Playlists</span></span>

## <a name="create-a-playlist"></a><span data-ttu-id="c581b-104">재생 목록 만들기</span><span class="sxs-lookup"><span data-stu-id="c581b-104">Create a Playlist</span></span>

<span data-ttu-id="c581b-p101">재생 목록은 "자산"의 compliation. "자산"은 SharePoint 페이지 또는 Microsoft 교육 콘텐츠의 기존 항목입니다. 재생 목록을 만들 때 함께 이동 하는 자산을 선택 하 여 사용자에 대 한 학습 경로를 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="c581b-p101">A playlist is a compliation of "assets". An "asset" is a SharePoint page or existing item of Microsoft training content. When you create a playlist you select assets that go together to create a learning path for your user.</span></span>  

<span data-ttu-id="c581b-p102">sharepoint 페이지를 추가할 때의 이점은 조직에서 호스트 되는 YouTube 비디오 또는 비디오를 사용 하 여 sharepoint 페이지를 만들 수 있다는 것입니다. 양식 또는 기타 Office 365 콘텐츠가 포함 된 페이지를 만들 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c581b-p102">The benefit of adding SharePoint pages is that you can create SharePoint pages with a YouTube videos or videos hosted in your organization. You can also create pages with Forms or other Office 365 content.</span></span>  

#### <a name="step-1-create-a-sharepoint-page-for-your-playlist"></a><span data-ttu-id="c581b-110">1 단계: 재생 목록에 대 한 SharePoint 페이지 만들기</span><span class="sxs-lookup"><span data-stu-id="c581b-110">Step 1: Create a SharePoint page for your playlist</span></span>
<span data-ttu-id="c581b-p103">이 예제에서는 먼저 재생 목록에 추가할 SharePoint 페이지를 만듭니다. YouTube 비디오 웹 파트 및 텍스트 웹 파트가 포함 된 페이지를 만듭니다.  이 지침에서는 SharePoint Online 서비스를 사용 하 고 있다고 가정 합니다.</span><span class="sxs-lookup"><span data-stu-id="c581b-p103">In this example, we’ll first create a SharePoint page to add to the playlist. We’ll create a page with a YouTube video web part and Text web part.  These instructions assume you are using the SharePoint Online service.</span></span> 

#### <a name="create-a-new-page"></a><span data-ttu-id="c581b-114">새 페이지 만들기</span><span class="sxs-lookup"><span data-stu-id="c581b-114">Create a new page</span></span>
1.  <span data-ttu-id="c581b-115">설정 메뉴 > 사이트 콘텐츠 > 사이트 페이지 > 새 > Site 페이지를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="c581b-115">Select the Settings menu > Site Contents > Site Pages > New > Site Page.</span></span>
2.  <span data-ttu-id="c581b-116">제목 영역에 팀 명령 사용 상자를 입력 합니다.</span><span class="sxs-lookup"><span data-stu-id="c581b-116">In the title area, type Use the Teams command box</span></span>
3.  <span data-ttu-id="c581b-117">새 섹션 추가를 선택 하 고 두 개의 열을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="c581b-117">Select the Add a new section, and then select Two Columns.</span></span>

![2 열 추가](media/clo365addtwocolumn.png)

4.  <span data-ttu-id="c581b-119">왼쪽 상자에서 새 웹 파트 추가를 선택 하 고 포함을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="c581b-119">In the left-hand box, select Add a new web part, and then select Embed.</span></span> 
5.  <span data-ttu-id="c581b-120">웹 브라우저에서이 URL https://youtu.be/wYrRCRphrp0 로 이동 하 여 비디오에 대 한 embed 태그를 가져옵니다.</span><span class="sxs-lookup"><span data-stu-id="c581b-120">In a Web browser, go to this URL https://youtu.be/wYrRCRphrp0 and get the embed code for the video.</span></span> 
6.  <span data-ttu-id="c581b-121">SharePoint 웹 파트에서 embed 태그 추가를 선택 하 여 포함 상자에 붙여 넣습니다.</span><span class="sxs-lookup"><span data-stu-id="c581b-121">In the SharePoint Web part, select Add Embed code and then paste it into the Embed box.</span></span> 
7.  <span data-ttu-id="c581b-122">오른쪽 상자에서 새 웹 파트 추가를 선택한 다음 텍스트를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="c581b-122">In the right-hand box, select Add a new web part, and then select Text.</span></span> 
8.  <span data-ttu-id="c581b-p104">웹 브라우저에서 다음 https://support.office.com/en-us/article/13c4e429-7324-4886-b377-5dbed539193b URL로 이동 하 여 Try! 지침을 선택한 다음 텍스트 웹 파트에 붙여 넣습니다. 페이지 모양은 다음과 같습니다.</span><span class="sxs-lookup"><span data-stu-id="c581b-p104">In a Web browser, go to this URL: https://support.office.com/en-us/article/13c4e429-7324-4886-b377-5dbed539193b and copy the Try it! Instructions from the page and paste them into the Text Web part. Your page should look like the following.</span></span> 

![페이지 포함](media/clo365teamscommandbox.png)

9.  <span data-ttu-id="c581b-127">**게시**를 클릭 한 다음 페이지의 URL을 복사 하 여 메모장에 붙여넣기</span><span class="sxs-lookup"><span data-stu-id="c581b-127">Click **Publish**, and then copy the URL of the page and paste it in Notepad</span></span>

#### <a name="step-2-create-the-playlist"></a><span data-ttu-id="c581b-128">2 단계: 재생 목록 만들기</span><span class="sxs-lookup"><span data-stu-id="c581b-128">Step 2: Create the Playlist</span></span>

1. <span data-ttu-id="c581b-p105">사이트 환경에서 **사용자 지정 학습 관리** 페이지로 이동 합니다. ![custom_admin-.png](media/custom_admin.png)</span><span class="sxs-lookup"><span data-stu-id="c581b-p105">Navigate to the **Custom Learning Administration** page in your site experience. ![custom_admin.png](media/custom_admin.png)</span></span>
1. <span data-ttu-id="c581b-131">**범주가** 선택 되어 있는지 확인</span><span class="sxs-lookup"><span data-stu-id="c581b-131">Make sure **Category** is selected</span></span> 
1. <span data-ttu-id="c581b-132">새 재생 목록을 표시할 범주를 클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="c581b-132">Click on the category where you'd like your new playlist to appear</span></span>
1. <span data-ttu-id="c581b-133">범주 이름 옆에 있는 더하기 기호 ![(custom_addplay)를 클릭 합니다.](media/custom_addplay.png)</span><span class="sxs-lookup"><span data-stu-id="c581b-133">Next to the category name, click on the plus symbol ![custom_addplay.png](media/custom_addplay.png)</span></span>

1. <span data-ttu-id="c581b-p106">아래 예제와 같이 값을 입력 하 고 **만들기**를 선택 합니다. ![custom_details-.png](media/custom_details.png)</span><span class="sxs-lookup"><span data-stu-id="c581b-p106">Fill in the values as shown in the example below and select **Create**. ![custom_details.png](media/custom_details.png)</span></span>
- <span data-ttu-id="c581b-136">**제목** -재생 목록의 표시 이름입니다.</span><span class="sxs-lookup"><span data-stu-id="c581b-136">**Title** - Display name of the playlist</span></span>
- <span data-ttu-id="c581b-137">**Description** -배우게 되는 사항에 대 한 정보입니다.</span><span class="sxs-lookup"><span data-stu-id="c581b-137">**Description** - Information about what will be learned</span></span>
- <span data-ttu-id="c581b-138">**범주** -초기 선택을 기준으로 미리 선택 됩니다.</span><span class="sxs-lookup"><span data-stu-id="c581b-138">**Category** - Preselected based on your initial selection</span></span>
- <span data-ttu-id="c581b-139">**하위 범주** -초기 선택을 기준으로 미리 선택</span><span class="sxs-lookup"><span data-stu-id="c581b-139">**Sub Category** - Preselected based on your intial selection</span></span>
- <span data-ttu-id="c581b-140">**기술** -해당 되는 경우 선택</span><span class="sxs-lookup"><span data-stu-id="c581b-140">**Technology** - Select as applicable</span></span>
- <span data-ttu-id="c581b-141">**만추** -초급, intermidate 또는 Advanced</span><span class="sxs-lookup"><span data-stu-id="c581b-141">**Level** - Beginner, Intermidate or Advanced</span></span>
- <span data-ttu-id="c581b-142">**대상 그룹** -Microsoft에서 제공 하는 미리 정의 된 역할 목록을 기반으로 콘텐츠를 대상으로 지정할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c581b-142">**Audience** - This allows you to target content based on a pre-defined list of roles provided by Microsoft.</span></span>

6. <span data-ttu-id="c581b-143">**세부 정보 저장** 을 클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="c581b-143">Click **Save Detail**</span></span>

> [!TIP]
> <span data-ttu-id="c581b-p107">재생 목록의 아이콘 이미지를 사용자 지정할 수 있습니다.  이미지 아이콘을 클릭 하 고 이전에 업로드 한 이미지의 URL을 삽입 합니다.  이미지가 사용자 지정 학습 사이트 모음에 위치 하거나 모든 사용자가 해당 파일에 액세스할 수 있는 다른 위치에 있는지 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="c581b-p107">You can customize the icon image for your playlist.  Click the image icon and insert an URL of a previously uploaded image.  Make sure the image is located within the Custom Learning site collection or in another location that all users will have access to the file.</span></span>  
<span data-ttu-id="c581b-147">![custom_image-.png](media/custom_image.png)</span><span class="sxs-lookup"><span data-stu-id="c581b-147">![custom_image.png](media/custom_image.png)</span></span>

#### <a name="step-3-add-assets-to-the-playlist"></a><span data-ttu-id="c581b-148">3 단계: 재생 목록에 에셋 추가</span><span class="sxs-lookup"><span data-stu-id="c581b-148">Step 3: Add assets to the playlist</span></span>
<span data-ttu-id="c581b-149">이 단계에서는 Microsoft 및 만든 SharePoint 페이지의 기존 자산을 재생 목록에 추가 합니다.</span><span class="sxs-lookup"><span data-stu-id="c581b-149">In this step, you’ll add existing assets from Microsoft and the SharePoint page you created to the playlist.</span></span> 

1. <span data-ttu-id="c581b-150">재생 목록에 대 한 세부 정보를 저장 한 후에는 기존 자산 검색을 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c581b-150">Once you have saved the details for your Playlist you can use the Search for Existing Assets.</span></span>
1. <span data-ttu-id="c581b-p108">**검색 용어를 입력** 하 여 다른 재생 목록에서 사용할 수 있는 미리 정의 된 자산의 목록을 확인 합니다. 자산 **이름을 클릭** 하 여 새 재생 목록에 포함 합니다. ![custom_slist-.png](media/custom_slist.png)</span><span class="sxs-lookup"><span data-stu-id="c581b-p108">**Enter in any search term** to see a list of predefined assets that are available from other playlists. **Click on the name** of an asset to include it in your new playlist. ![custom_slist.png](media/custom_slist.png)</span></span>

<span data-ttu-id="c581b-154">이전에 만든 SharePoint 페이지를 추가 하거나 환경에서 처음부터 새로 만들 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c581b-154">You can also add the SharePoint page you created earlier or create one from scratch in the experience.</span></span>

1. <span data-ttu-id="c581b-155">재생 목록 자산 대화 상자에서 **새 자산** 옵션을 클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="c581b-155">Click on the **New Asset** option in the Playlist Assets dialog</span></span>
1. <span data-ttu-id="c581b-p109">자산에 **제목을**지정 합니다. 입력 된 추가 옵션에는 custom_newpage ![가 표시 됩니다.](media/custom_newpage.png)</span><span class="sxs-lookup"><span data-stu-id="c581b-p109">Give your asset a **Title**. Once entered, additional options will display ![custom_newpage.png](media/custom_newpage.png)</span></span>
1. <span data-ttu-id="c581b-158">이제 SharePoint Online에서 새 자산 페이지를 만들거나 기존 페이지의 URL을 입력 하 여 사용자 지정 재생 목록에 추가할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c581b-158">You can now create a new asset page in SharePoint Online or enter in the URL of an existing page to add it to your custom playlist.</span></span> 
1. <span data-ttu-id="c581b-159">**범주**, **하위 범주** 및 **기술** 필드는이 재생 목록에 대 한 이전 선택 항목에 따라 미리 채워집니다.</span><span class="sxs-lookup"><span data-stu-id="c581b-159">**Category**, **Sub Category** and **Technology** fields will be pre-populated based on your previous selections for this playlist.</span></span>
1. <span data-ttu-id="c581b-160">이 개별 자산의 수준 및 대상 그룹을 적절 하 게 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="c581b-160">Make the appropriate selections for Level and Audience for this individual asset.</span></span>  
1. <span data-ttu-id="c581b-161">**자산 저장** 을 클릭 하 여 사용자 지정 재생 목록에 추가 합니다.</span><span class="sxs-lookup"><span data-stu-id="c581b-161">Click **Save Asset** to add it to the custom playlist</span></span>
1. <span data-ttu-id="c581b-162">재생 목록이 완료 될 때까지 개별 페이지를 검색 하거나 추가 하 여이 단계를 반복 합니다.</span><span class="sxs-lookup"><span data-stu-id="c581b-162">Repeat these steps, either searching or adding individual pages, until your playlist is complete.</span></span> 
1. <span data-ttu-id="c581b-163">**재생 목록 닫기** 를 클릭 하 여 저장</span><span class="sxs-lookup"><span data-stu-id="c581b-163">Click **Close Playlist** to save</span></span>

<span data-ttu-id="c581b-164">이 콘텐츠를 포함 하는 재생 목록은 사용자 지정 학습 웹 파트를 설치/포함 한 모든 위치에서 사용할 수 있게 됩니다.</span><span class="sxs-lookup"><span data-stu-id="c581b-164">Your playlist with this content will now be available anywhere you have installed / embedded the Custom Learning webpart.</span></span> 

> [!NOTE]
> <span data-ttu-id="c581b-165">재생 목록을 닫은 후 실수를 한 경우 재생 목록 이름 옆에 있는 X를 클릭 하 여 범주에서 삭제할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c581b-165">If you make a mistake once you have closed the playlist, you can delete it from the category by clicking the X next to the playlist name.</span></span>  

#### <a name="things-to-think-about"></a><span data-ttu-id="c581b-166">고려해 야 할 사항</span><span class="sxs-lookup"><span data-stu-id="c581b-166">Things to Think About</span></span>

<span data-ttu-id="c581b-p110">사용자 지정 재생 목록을 사용 하 여 최종 사용자가 다양 한 작업을 지원할 수 있습니다.  휴가 요청 양식이 있습니까?  하드웨어 장비를 요청 하는 양식  모든 기존 교육 자산이 환경에 프로그래밍 될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c581b-p110">Custom playlists can be used to assist your end users in a variety of tasks.  Do you have a time off request form?  A form to request hardware equipment?  Any existing training assets can be programmed into the experience.</span></span>  

## <a name="share-playlists"></a><span data-ttu-id="c581b-171">재생 목록 공유</span><span class="sxs-lookup"><span data-stu-id="c581b-171">Share Playlists</span></span>

1. <span data-ttu-id="c581b-172">웹 파트 또는 사이트 환경 내의 재생 목록으로 이동</span><span class="sxs-lookup"><span data-stu-id="c581b-172">Navigate to any playlist within the webpart or site experience</span></span>
1. <span data-ttu-id="c581b-173">왼쪽 위 모서리에 세 개의 아이콘이 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="c581b-173">In the upper left hand corner you will see three icons</span></span>
1. <span data-ttu-id="c581b-174">링크를 나타내는 아이콘을 클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="c581b-174">Click on the icon representing a link</span></span>
1. <span data-ttu-id="c581b-175">재생 목록에 URL 복사</span><span class="sxs-lookup"><span data-stu-id="c581b-175">Copy the URL to the playlist</span></span>

<span data-ttu-id="c581b-176">![.png](media/share.png) 이 URL은 이제 사이트 탐색에 삽입 하거나 다른 통신에서 사용 하 여 직원을 해당 재생 목록으로 바로 이동할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c581b-176">![share.png](media/share.png) This URL can now be inserted in your site navigation or utilized in other communications to take your employees directly to that playlist.</span></span> 

### <a name="next-steps---drive-adoptiondriveadoptionmd"></a><span data-ttu-id="c581b-177">다음 단계- [드라이브 도입](driveadoption.md)</span><span class="sxs-lookup"><span data-stu-id="c581b-177">Next Steps - [Drive Adoption](driveadoption.md)</span></span>
