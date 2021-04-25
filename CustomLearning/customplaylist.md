---
author: karuanag
ms.author: karuanag
manager: alexb
title: 재생 목록 사용자 지정 및 공유
ms.date: 02/10/2019
description: 기존 콘텐츠 또는 새 SharePoint 페이지에서 사용자 지정 재생 목록 만들기
ms.service: sharepoint-online
audience: itpro
ms.topic: article
ms.openlocfilehash: 31a0e5524181d26f4d62ae7206636c9e553b6f8f
ms.sourcegitcommit: 97e175e5ff5b6a9e0274d5ec9b39fdf7e18eb387
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/25/2021
ms.locfileid: "52000214"
---
# <a name="customize-and-share-playlists"></a><span data-ttu-id="2d45c-103">재생 목록 사용자 지정 및 공유</span><span class="sxs-lookup"><span data-stu-id="2d45c-103">Customize and share playlists</span></span>

## <a name="create-a-playlist"></a><span data-ttu-id="2d45c-104">재생 목록 만들기</span><span class="sxs-lookup"><span data-stu-id="2d45c-104">Create a Playlist</span></span>

<span data-ttu-id="2d45c-105">재생 목록은 "자산"을 보완하는 것입니다.</span><span class="sxs-lookup"><span data-stu-id="2d45c-105">A playlist is a compliation of "assets".</span></span> <span data-ttu-id="2d45c-106">"자산"은 Microsoft 교육 콘텐츠의 SharePoint 페이지 또는 기존 항목입니다.</span><span class="sxs-lookup"><span data-stu-id="2d45c-106">An "asset" is a SharePoint page or existing item of Microsoft training content.</span></span> <span data-ttu-id="2d45c-107">재생 목록을 만들 때 함께 이동하여 사용자에 대한 학습 경로를 만드는 자산을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="2d45c-107">When you create a playlist you select assets that go together to create a learning path for your user.</span></span>  

<span data-ttu-id="2d45c-108">SharePoint 페이지를 추가하면 조직에서 호스팅되는 YouTube 비디오 또는 비디오를 사용하여 SharePoint 페이지를 만들 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="2d45c-108">The benefit of adding SharePoint pages is that you can create SharePoint pages with a YouTube videos or videos hosted in your organization.</span></span> <span data-ttu-id="2d45c-109">Forms 또는 기타 Office 365 콘텐츠를 사용하여 페이지를 만들 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="2d45c-109">You can also create pages with Forms or other Office 365 content.</span></span>  

#### <a name="step-1-create-a-sharepoint-page-for-your-playlist"></a><span data-ttu-id="2d45c-110">1단계: 재생 목록에 대한 SharePoint 페이지 만들기</span><span class="sxs-lookup"><span data-stu-id="2d45c-110">Step 1: Create a SharePoint page for your playlist</span></span>
<span data-ttu-id="2d45c-111">이 예제에서는 먼저 재생 목록에 추가할 SharePoint 페이지를 만들어 보겠습니다.</span><span class="sxs-lookup"><span data-stu-id="2d45c-111">In this example, we’ll first create a SharePoint page to add to the playlist.</span></span> <span data-ttu-id="2d45c-112">YouTube 비디오 웹 파트 및 텍스트 웹 파트가 있는 페이지를 만들 것입니다.</span><span class="sxs-lookup"><span data-stu-id="2d45c-112">We’ll create a page with a YouTube video web part and Text web part.</span></span>  <span data-ttu-id="2d45c-113">이 지침에서는 SharePoint Online 서비스를 사용 중이라 가정합니다.</span><span class="sxs-lookup"><span data-stu-id="2d45c-113">These instructions assume you are using the SharePoint Online service.</span></span> 

#### <a name="create-a-new-page"></a><span data-ttu-id="2d45c-114">새 페이지 만들기</span><span class="sxs-lookup"><span data-stu-id="2d45c-114">Create a new page</span></span>
1.  <span data-ttu-id="2d45c-115">새 사이트 페이지 > 사이트 > 콘텐츠 > > 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="2d45c-115">Select the Settings menu > Site Contents > Site Pages > New > Site Page.</span></span>
2.  <span data-ttu-id="2d45c-116">제목 영역에 Teams 명령 상자를 입력합니다.</span><span class="sxs-lookup"><span data-stu-id="2d45c-116">In the title area, type Use the Teams command box</span></span>
3.  <span data-ttu-id="2d45c-117">새 추가 섹션을 선택한 다음 두 열을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="2d45c-117">Select the Add a new section, and then select Two Columns.</span></span>

![두 열 추가](media/clo365addtwocolumn.png)

4.  <span data-ttu-id="2d45c-119">왼쪽 상자에서 새 웹 파트 추가를 선택한 다음 Embed를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="2d45c-119">In the left-hand box, select Add a new web part, and then select Embed.</span></span> 
5.  <span data-ttu-id="2d45c-120">웹 브라우저에서 이 URL로 이동하여 비디오에 대한 https://youtu.be/wYrRCRphrp0 코드를 다운로드합니다.</span><span class="sxs-lookup"><span data-stu-id="2d45c-120">In a Web browser, go to this URL https://youtu.be/wYrRCRphrp0 and get the embed code for the video.</span></span> 
6.  <span data-ttu-id="2d45c-121">SharePoint 웹 파트에서 Embed 코드 추가를 선택한 다음 임박 상자에 붙여 넣습니다.</span><span class="sxs-lookup"><span data-stu-id="2d45c-121">In the SharePoint Web part, select Add Embed code and then paste it into the Embed box.</span></span> 
7.  <span data-ttu-id="2d45c-122">오른쪽 상자에서 새 웹 파트 추가를 선택한 다음 텍스트를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="2d45c-122">In the right-hand box, select Add a new web part, and then select Text.</span></span> 
8.  <span data-ttu-id="2d45c-123">웹 브라우저에서 이 URL로 이동하여 https://support.office.com/article/13c4e429-7324-4886-b377-5dbed539193b 시도해 보세요!</span><span class="sxs-lookup"><span data-stu-id="2d45c-123">In a Web browser, go to this URL: https://support.office.com/article/13c4e429-7324-4886-b377-5dbed539193b and copy the Try it!</span></span> <span data-ttu-id="2d45c-124">페이지의 지침에 따라 텍스트 웹 파트에 붙여 넣습니다.</span><span class="sxs-lookup"><span data-stu-id="2d45c-124">Instructions from the page and paste them into the Text Web part.</span></span> <span data-ttu-id="2d45c-125">페이지는 다음과 같이 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="2d45c-125">Your page should look like the following.</span></span> 
<span data-ttu-id="2d45c-126">![Embed page](media/clo365teamscommandbox.png)</span><span class="sxs-lookup"><span data-stu-id="2d45c-126">![Embed page](media/clo365teamscommandbox.png)</span></span>
9.  <span data-ttu-id="2d45c-127">**게시를** 클릭한 다음 페이지의 URL을 복사하여 메모장에 붙여 넣습니다.</span><span class="sxs-lookup"><span data-stu-id="2d45c-127">Click **Publish**, and then copy the URL of the page and paste it in Notepad</span></span>

#### <a name="step-2-create-the-playlist"></a><span data-ttu-id="2d45c-128">2단계: 재생 목록 만들기</span><span class="sxs-lookup"><span data-stu-id="2d45c-128">Step 2: Create the Playlist</span></span>

1. <span data-ttu-id="2d45c-129">사이트 **환경의 사용자 지정 학습 관리** 페이지로 이동합니다.</span><span class="sxs-lookup"><span data-stu-id="2d45c-129">Navigate to the **Custom Learning Administration** page in your site experience.</span></span>
<span data-ttu-id="2d45c-130">![사용자 지정 학습 관리 선택 화면.](media/custom_admin.png)</span><span class="sxs-lookup"><span data-stu-id="2d45c-130">![Screen where you select Custom Learning Administration.](media/custom_admin.png)</span></span>
1. <span data-ttu-id="2d45c-131">범주가  선택되어 있는지 확인</span><span class="sxs-lookup"><span data-stu-id="2d45c-131">Make sure **Category** is selected</span></span> 
1. <span data-ttu-id="2d45c-132">새 재생 목록을 표시하려면 범주를 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="2d45c-132">Click on the category where you'd like your new playlist to appear</span></span>
1. <span data-ttu-id="2d45c-133">범주 이름 옆에 있는 더하기 기호 범주 옵션과 더하기 기호가 강조 표시된 ![ 창을 클릭합니다.](media/custom_addplay.png)</span><span class="sxs-lookup"><span data-stu-id="2d45c-133">Next to the category name, click on the plus symbol ![Window with the Category option and the Plus sign highlighted.](media/custom_addplay.png)</span></span>

1. <span data-ttu-id="2d45c-134">아래 예제와 같이 값을 입력하고 만들기를 **선택합니다.**</span><span class="sxs-lookup"><span data-stu-id="2d45c-134">Fill in the values as shown in the example below and select **Create**.</span></span> 
<span data-ttu-id="2d45c-135">![재생 목록 세부 정보를 입력하는 페이지입니다.](media/custom_details.png)</span><span class="sxs-lookup"><span data-stu-id="2d45c-135">![Page where you enter playlist details.](media/custom_details.png)</span></span>
- <span data-ttu-id="2d45c-136">**제목** - 재생 목록의 표시 이름</span><span class="sxs-lookup"><span data-stu-id="2d45c-136">**Title** - Display name of the playlist</span></span>
- <span data-ttu-id="2d45c-137">**Description** - 학습할 내용에 대한 정보</span><span class="sxs-lookup"><span data-stu-id="2d45c-137">**Description** - Information about what will be learned</span></span>
- <span data-ttu-id="2d45c-138">**범주** - 초기 선택에 따라 미리 선택</span><span class="sxs-lookup"><span data-stu-id="2d45c-138">**Category** - Preselected based on your initial selection</span></span>
- <span data-ttu-id="2d45c-139">**하위 범주** - 사용자 선택에 따라 미리 선택</span><span class="sxs-lookup"><span data-stu-id="2d45c-139">**Sub Category** - Preselected based on your intial selection</span></span>
- <span data-ttu-id="2d45c-140">**기술** - 적용 가능한 선택</span><span class="sxs-lookup"><span data-stu-id="2d45c-140">**Technology** - Select as applicable</span></span>
- <span data-ttu-id="2d45c-141">**수준** - 초보자, 상호 연결 또는 고급</span><span class="sxs-lookup"><span data-stu-id="2d45c-141">**Level** - Beginner, Intermidate or Advanced</span></span>
- <span data-ttu-id="2d45c-142">**대상** - 이를 통해 Microsoft에서 제공하는 미리 정의된 역할 목록을 기반으로 콘텐츠를 대상으로 할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="2d45c-142">**Audience** - This allows you to target content based on a pre-defined list of roles provided by Microsoft.</span></span>

6. <span data-ttu-id="2d45c-143">자세히 **저장을 클릭합니다.**</span><span class="sxs-lookup"><span data-stu-id="2d45c-143">Click **Save Detail**</span></span>

> [!TIP]
> <span data-ttu-id="2d45c-144">재생 목록의 아이콘 이미지를 사용자 지정할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="2d45c-144">You can customize the icon image for your playlist.</span></span>  <span data-ttu-id="2d45c-145">이미지 아이콘을 클릭하고 이전에 업로드한 이미지의 URL을 삽입합니다.</span><span class="sxs-lookup"><span data-stu-id="2d45c-145">Click the image icon and insert an URL of a previously uploaded image.</span></span>  <span data-ttu-id="2d45c-146">이미지가 사용자 지정 학습 사이트 모음 또는 모든 사용자가 파일에 액세스할 수 있는 다른 위치에 있는지 확인</span><span class="sxs-lookup"><span data-stu-id="2d45c-146">Make sure the image is located within the Custom Learning site collection or in another location that all users will have access to the file.</span></span>  
<span data-ttu-id="2d45c-147">![이미지 창을 선택합니다.](media/custom_image.png)</span><span class="sxs-lookup"><span data-stu-id="2d45c-147">![Choose an image window.](media/custom_image.png)</span></span>

#### <a name="step-3-add-assets-to-the-playlist"></a><span data-ttu-id="2d45c-148">3단계: 재생 목록에 자산 추가</span><span class="sxs-lookup"><span data-stu-id="2d45c-148">Step 3: Add assets to the playlist</span></span>
<span data-ttu-id="2d45c-149">이 단계에서는 Microsoft의 기존 자산과 만든 SharePoint 페이지를 재생 목록에 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="2d45c-149">In this step, you’ll add existing assets from Microsoft and the SharePoint page you created to the playlist.</span></span> 

1. <span data-ttu-id="2d45c-150">재생 목록에 대한 세부 정보를 저장한 후 기존 자산 검색을 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="2d45c-150">Once you have saved the details for your Playlist you can use the Search for Existing Assets.</span></span>
1. <span data-ttu-id="2d45c-151">**검색 용어에** 입력하여 다른 재생 목록에서 사용할 수 있는 미리 정의한 자산 목록을 볼 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="2d45c-151">**Enter in any search term** to see a list of predefined assets that are available from other playlists.</span></span> <span data-ttu-id="2d45c-152">**자산의 이름을** 클릭하여 새 재생 목록에 포함합니다.</span><span class="sxs-lookup"><span data-stu-id="2d45c-152">**Click on the name** of an asset to include it in your new playlist.</span></span><br/>
<span data-ttu-id="2d45c-153">![재생 목록 자산 페이지](media/custom_slist.png)</span><span class="sxs-lookup"><span data-stu-id="2d45c-153">![Playlist assets page](media/custom_slist.png)</span></span>

<span data-ttu-id="2d45c-154">앞에서 만든 SharePoint 페이지를 추가하거나 환경의 처음부터 만들 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="2d45c-154">You can also add the SharePoint page you created earlier or create one from scratch in the experience.</span></span>

1. <span data-ttu-id="2d45c-155">재생 목록 **자산 대화 상자에서** 새 자산 옵션을 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="2d45c-155">Click on the **New Asset** option in the Playlist Assets dialog.</span></span>
1. <span data-ttu-id="2d45c-156">자산에 제목을 **제공 합니다.**</span><span class="sxs-lookup"><span data-stu-id="2d45c-156">Give your asset a **Title**.</span></span> <span data-ttu-id="2d45c-157">입력하면 추가 옵션이 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="2d45c-157">Once entered, additional options will display.</span></span>
<span data-ttu-id="2d45c-158">![제목 및 추가 세부 정보를 입력하는 양식입니다.](media/custom_newpage.png)</span><span class="sxs-lookup"><span data-stu-id="2d45c-158">![Form where you enter your title and additional details.](media/custom_newpage.png)</span></span>
1. <span data-ttu-id="2d45c-159">이제 SharePoint Online에서 새 자산 페이지를 만들거나 기존 페이지의 URL을 입력하여 사용자 지정 재생 목록에 추가할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="2d45c-159">You can now create a new asset page in SharePoint Online or enter in the URL of an existing page to add it to your custom playlist.</span></span> 
1. <span data-ttu-id="2d45c-160">**범주,** 하위  **범주** 및 기술 필드는 이 재생 목록의 이전 선택에 따라 미리 채워지게 됩니다.</span><span class="sxs-lookup"><span data-stu-id="2d45c-160">**Category**, **Sub Category** and **Technology** fields will be pre-populated based on your previous selections for this playlist.</span></span>
1. <span data-ttu-id="2d45c-161">이 개별 자산에 대한 Level 및 Audience에 대해 적절한 선택을 합니다.</span><span class="sxs-lookup"><span data-stu-id="2d45c-161">Make the appropriate selections for Level and Audience for this individual asset.</span></span>  
1. <span data-ttu-id="2d45c-162">자산 **저장을 클릭하여** 사용자 지정 재생 목록에 추가</span><span class="sxs-lookup"><span data-stu-id="2d45c-162">Click **Save Asset** to add it to the custom playlist</span></span>
1. <span data-ttu-id="2d45c-163">재생 목록이 완료될 때까지 개별 페이지를 검색하거나 추가하는 단계를 반복합니다.</span><span class="sxs-lookup"><span data-stu-id="2d45c-163">Repeat these steps, either searching or adding individual pages, until your playlist is complete.</span></span> 
1. <span data-ttu-id="2d45c-164">재생 **목록 닫기 를 클릭하여** 저장</span><span class="sxs-lookup"><span data-stu-id="2d45c-164">Click **Close Playlist** to save</span></span>

<span data-ttu-id="2d45c-165">이 콘텐츠가 포함된 재생 목록은 이제 사용자 지정 학습 웹 사이트를 설치/포함한 모든 곳에서 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="2d45c-165">Your playlist with this content will now be available anywhere you have installed / embedded the Custom Learning webpart.</span></span> 

> [!NOTE]
> <span data-ttu-id="2d45c-166">재생 목록을 닫은 후 실수를 한 경우 재생 목록 이름 옆에 있는 X를 클릭하여 범주에서 삭제할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="2d45c-166">If you make a mistake once you have closed the playlist, you can delete it from the category by clicking the X next to the playlist name.</span></span>  

#### <a name="things-to-think-about"></a><span data-ttu-id="2d45c-167">생각할 것</span><span class="sxs-lookup"><span data-stu-id="2d45c-167">Things to Think About</span></span>

<span data-ttu-id="2d45c-168">사용자 지정 재생 목록을 사용하여 최종 사용자가 다양한 작업을 수행할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="2d45c-168">Custom playlists can be used to assist your end users in a variety of tasks.</span></span>  <span data-ttu-id="2d45c-169">시간제 요청 양식이 있나요?</span><span class="sxs-lookup"><span data-stu-id="2d45c-169">Do you have a time off request form?</span></span>  <span data-ttu-id="2d45c-170">하드웨어 장비를 요청하는 양식인가요?</span><span class="sxs-lookup"><span data-stu-id="2d45c-170">A form to request hardware equipment?</span></span>  <span data-ttu-id="2d45c-171">기존 교육 자산을 경험에 프로그래밍할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="2d45c-171">Any existing training assets can be programmed into the experience.</span></span>  

## <a name="share-playlists"></a><span data-ttu-id="2d45c-172">재생 목록 공유</span><span class="sxs-lookup"><span data-stu-id="2d45c-172">Share Playlists</span></span>

1. <span data-ttu-id="2d45c-173">웹파트 또는 사이트 환경 내의 재생 목록으로 이동</span><span class="sxs-lookup"><span data-stu-id="2d45c-173">Navigate to any playlist within the webpart or site experience</span></span>
1. <span data-ttu-id="2d45c-174">왼쪽 위 모서리에 세 개의 아이콘이 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="2d45c-174">In the upper left hand corner you will see three icons</span></span>
1. <span data-ttu-id="2d45c-175">링크를 나타내는 아이콘 클릭</span><span class="sxs-lookup"><span data-stu-id="2d45c-175">Click on the icon representing a link</span></span>
1. <span data-ttu-id="2d45c-176">URL 옆에 있는 복사를 클릭하는 재생 목록 화면에 ![ URL을 복사합니다.](media/share.png)</span><span class="sxs-lookup"><span data-stu-id="2d45c-176">Copy the URL to the playlist ![Screen where you click Copy next to the URL.](media/share.png)</span></span>
<span data-ttu-id="2d45c-177">이제 이 URL을 사이트 탐색에 삽입하거나 다른 통신에 활용하여 직원을 해당 재생 목록으로 바로 이동하는 데 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="2d45c-177">This URL can now be inserted in your site navigation or utilized in other communications to take your employees directly to that playlist.</span></span> 

### <a name="next-steps---drive-adoption"></a><span data-ttu-id="2d45c-178">다음 단계 - [채택 주도](driveadoption.md)</span><span class="sxs-lookup"><span data-stu-id="2d45c-178">Next Steps - [Drive Adoption](driveadoption.md)</span></span>
