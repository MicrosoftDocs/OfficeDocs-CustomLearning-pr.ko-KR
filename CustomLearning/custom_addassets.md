---
author: pkrebs
ms.author: pkrebs
title: 재생 목록에 자산 추가
ms.date: 02/17/2019
description: 학습 경로 재생 목록에 새 자산 및 기존 자산 추가
ms.service: sharepoint-online
ms.openlocfilehash: abd4500faccf8d4e8008f72dc800855035d8a2c9
ms.sourcegitcommit: 97e175e5ff5b6a9e0274d5ec9b39fdf7e18eb387
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/25/2021
ms.locfileid: "51999834"
---
# <a name="add-assets-to-a-custom-playlist"></a><span data-ttu-id="692e7-103">사용자 지정 재생 목록에 자산 추가</span><span class="sxs-lookup"><span data-stu-id="692e7-103">Add Assets to a Custom Playlist</span></span>

<span data-ttu-id="692e7-104">학습 경로를 사용하여 재생 목록에 다음 자산을 추가할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="692e7-104">With learning pathways, you can add the following assets to a playlist:</span></span>

- <span data-ttu-id="692e7-105">**기존 Microsoft 365** 학습 경로 자산 - 이러한 자산은 Microsoft 온라인 카탈로그의 일부인 자산 또는 조직에서 학습 경로에 이미 추가한 자산입니다.</span><span class="sxs-lookup"><span data-stu-id="692e7-105">**Existing Microsoft 365 learning pathways assets** - these are assets that are part of the Microsoft online catalog or assets that your organization has already added to learning pathways.</span></span>
- <span data-ttu-id="692e7-106">**새 자산** - 만든 SharePoint 페이지 또는 조직의 SharePoint 사이트에서 이미 사용할 수 있는 SharePoint 자산을 사용하여 작성된 학습 경로에 추가하는 자산입니다.</span><span class="sxs-lookup"><span data-stu-id="692e7-106">**New assets** - these are assets that you add to learning pathways that are built from SharePoint pages that you create or SharePoint assets that are already available on a SharePoint site in your organization.</span></span> 

> [!TIP]
> <span data-ttu-id="692e7-107">Microsoft 재생 목록 자산이 요구 사항을 충족하지 않는 경우 새 재생 목록을 만든 다음 Microsoft 자산 및 새로 만든 자산을 재생 목록에 추가하여 원하는 환경을 구축합니다.</span><span class="sxs-lookup"><span data-stu-id="692e7-107">If a Microsoft playlist asset doesn't meet your needs, create a new playlist and then add the Microsoft assets and any newly created assets to the playlist to build the experience you want.</span></span> <span data-ttu-id="692e7-108">Microsoft에서 제공하는 학습 경로 재생 목록을 수정할 수 없지만 학습 경로 제공 자산을 사용자 지정 재생 목록에 추가할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="692e7-108">You can't modify learning pathways playlists supplied by Microsoft, but you can add learning pathways-supplied assets to a custom playlist.</span></span>   

## <a name="create-a-new-asset-for-a-playlist"></a><span data-ttu-id="692e7-109">재생 목록에 대한 새 자산 만들기</span><span class="sxs-lookup"><span data-stu-id="692e7-109">Create a new asset for a playlist</span></span>

<span data-ttu-id="692e7-110">재생 목록에 새 자산을 추가하는 두 가지 옵션이 있습니다.</span><span class="sxs-lookup"><span data-stu-id="692e7-110">There are two options for adding a new asset to a playlist.</span></span>

- <span data-ttu-id="692e7-111">**자산 페이지 만들기** - 이 옵션을 사용하면 학습 경로에서 비어 있는 새 SharePoint 페이지를 생성하고 재생 목록에 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="692e7-111">**Create Asset Page** - with this option, learning pathways will generate a new,  blank SharePoint page for you and add it to the playlist.</span></span> <span data-ttu-id="692e7-112">그런 다음 페이지에 콘텐츠를 추가하고 저장할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="692e7-112">You can then add content to the page and save it.</span></span>  
- <span data-ttu-id="692e7-113">**URL 입력** - 이 옵션을 사용하여 페이지를 미리 빌드하거나 이미 페이지를 사용할 수 있으며 재생 목록에 페이지를 추가할 URL을 지정합니다.</span><span class="sxs-lookup"><span data-stu-id="692e7-113">**Enter the URL** - with this option, you build the page in advance or you already have the page available and you specify the URL to add the page to the playlist.</span></span>

### <a name="create-asset-page"></a><span data-ttu-id="692e7-114">자산 만들기 페이지</span><span class="sxs-lookup"><span data-stu-id="692e7-114">Create Asset Page</span></span> 
<span data-ttu-id="692e7-115">자산 **페이지** 만들기 옵션을 사용하여 자산 제목을 제공한 다음 자산 만들기 페이지를 클릭하여 편집할 새 SharePoint 페이지를 만들고 여십시오.</span><span class="sxs-lookup"><span data-stu-id="692e7-115">With the **Create Asset Page** option, you provide a title for the Asset, then click Create Asset page to create and open a new SharePoint page for editing.</span></span> 

1.  <span data-ttu-id="692e7-116">재생 목록이 편집할 수 있는 아직 열려 있지 않은 경우 사용자 지정 학습 관리 **페이지에서** 편집할 재생 목록을 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="692e7-116">If the playlist isn't already open for editing, from the **Custom Learning Administration** page, click the playlist you wish to edit.</span></span> 
2. <span data-ttu-id="692e7-117">재생 목록에 새 자산을 추가하려면 새 자산 **을 클릭합니다.**</span><span class="sxs-lookup"><span data-stu-id="692e7-117">To add a new asset to a playlist, click **New Asset**.</span></span> 
3. <span data-ttu-id="692e7-118">제목을 입력합니다.</span><span class="sxs-lookup"><span data-stu-id="692e7-118">Enter a title.</span></span> <span data-ttu-id="692e7-119">이 예제에서는 "재생 목록에 자산 추가"를 입력한 다음 자산 페이지 **만들기를 클릭합니다.**</span><span class="sxs-lookup"><span data-stu-id="692e7-119">In this example enter “Add Assets to a Playlist”, and then click **Create Asset Page**.</span></span>

![cg-addassetcreatenewpage.png](media/cg-addassetcreatenewpage.png)

4. <span data-ttu-id="692e7-121">페이지 **열기 를 클릭합니다.**</span><span class="sxs-lookup"><span data-stu-id="692e7-121">Click **Open Page**.</span></span>
5. <span data-ttu-id="692e7-122">편집 **아이콘을** 클릭한 다음 제목 **영역의 웹 파트** 편집을 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="692e7-122">Click the **Edit** icon, and then click **Edit Web part** in the Title area.</span></span>
6. <span data-ttu-id="692e7-123">**레이아웃에서** 일반 을 **클릭합니다.**</span><span class="sxs-lookup"><span data-stu-id="692e7-123">Under **Layout**, click **Plain**.</span></span> 
7. <span data-ttu-id="692e7-124">한 열로 구성한 섹션을 새로 추가한 다음 페이지에 예제 텍스트를 추가하여 다음 예제와 같이 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="692e7-124">Add a new one-column section, and then add some sample text to the page so it looks like the following example.</span></span> 

![cg-addassetcreatenewpageedit.png](media/cg-addassetcreatenewpageedit.png)

7. <span data-ttu-id="692e7-126">**게시** 를 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="692e7-126">Click **Publish**.</span></span>
8. <span data-ttu-id="692e7-127">사용자 지정 **학습 관리 페이지로** 돌아오십시오.</span><span class="sxs-lookup"><span data-stu-id="692e7-127">Return to the **Custom Learning Administration** page.</span></span> 
9. <span data-ttu-id="692e7-128">자산의 나머지 속성을 작성한 다음 자산 **저장을 클릭합니다.**</span><span class="sxs-lookup"><span data-stu-id="692e7-128">Fill out the remainder of the properties for the asset, and then click **Save Asset.**</span></span>

### <a name="enter-the-url"></a><span data-ttu-id="692e7-129">URL 입력</span><span class="sxs-lookup"><span data-stu-id="692e7-129">Enter the URL</span></span>
<span data-ttu-id="692e7-130">URL **입력 옵션을** 사용하여 자산 제목을 입력한 다음 **URL** 입력을 클릭하여 재생 목록에 추가할 SharePoint 페이지를 지정합니다.</span><span class="sxs-lookup"><span data-stu-id="692e7-130">With the **Enter the URL** option, you provide a title for the Asset, then click **Enter the URL** to specify the SharePoint page you want to add to the playlist.</span></span> 

1.  <span data-ttu-id="692e7-131">편집할 재생 목록이 열려 있지 않은 경우 사용자 지정 학습 관리 **페이지에서** 편집할 재생 목록을 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="692e7-131">If the playlist isn't open for editing, from the **Custom Learning Administration** page, click the playlist you wish to edit.</span></span> 
2. <span data-ttu-id="692e7-132">재생 목록에 새 자산을 추가하려면 새 자산 **을 클릭합니다.**</span><span class="sxs-lookup"><span data-stu-id="692e7-132">To add a new asset to a playlist, click **New Asset**.</span></span> 
3. <span data-ttu-id="692e7-133">제목을 입력합니다.</span><span class="sxs-lookup"><span data-stu-id="692e7-133">Enter a title.</span></span> <span data-ttu-id="692e7-134">이 예에서는 "사용자 지정 재생 목록 소개"를 입력한 다음 **URL 입력 을 클릭합니다.**</span><span class="sxs-lookup"><span data-stu-id="692e7-134">In this example, enter “Custom Playlist Introduction”, and then click **Enter URL**.</span></span> 

![cg-newplaylistasseturl.png](media/cg-newplaylistasseturl.png)

4. <span data-ttu-id="692e7-136">이전 사용자 지정 재생 목록용 SharePoint 페이지 만들기 섹션에서 만든 [SharePoint ](custom_createnewpage.md) 페이지의 URL을 입력한 다음 다음 그림과 같이 필드의 나머지 부분을 입력합니다.</span><span class="sxs-lookup"><span data-stu-id="692e7-136">Enter the URL of the SharePoint page you created in a previous [Create SharePoint pages for custom playlists ](custom_createnewpage.md) section, and then fill out the remainder of the fields, as shown in the following illustration.</span></span>

![cg-newplaylistassetdetails.png](media/cg-newplaylistassetdetails.png)

5. <span data-ttu-id="692e7-138">자산 **저장을 클릭합니다.**</span><span class="sxs-lookup"><span data-stu-id="692e7-138">Click **Save Asset**.</span></span> 

## <a name="add-an-existing-asset-to-a-playlist"></a><span data-ttu-id="692e7-139">재생 목록에 기존 자산 추가</span><span class="sxs-lookup"><span data-stu-id="692e7-139">Add an existing asset to a playlist</span></span>

<span data-ttu-id="692e7-140">기존 자산은 조직에서 학습 경로에 이미 추가한 Microsoft 제공 학습 경로 자산 또는 자산으로 구성됩니다.</span><span class="sxs-lookup"><span data-stu-id="692e7-140">Existing assets consist of Microsoft-provided learning pathways assets or assets that have already been added to learning pathways by your organization.</span></span> 

- <span data-ttu-id="692e7-141">검색 **상자에** 검색 구를 입력한 다음 검색 결과에서 자산을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="692e7-141">In the **Search** box, enter a Search phrase, and then select an asset from the Search results.</span></span> <span data-ttu-id="692e7-142">이 예제에서는 "Excel이 무엇입니까?"를 입력합니다.</span><span class="sxs-lookup"><span data-stu-id="692e7-142">In this example, enter “What is Excel?”</span></span> <span data-ttu-id="692e7-143">을(를) 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="692e7-143">to add an Excel intro topic to the playlist.</span></span>

![cg-existplaylistassetsearch.png](media/cg-existplaylistassetsearch.png)

## <a name="edit-move-and-delete-assets"></a><span data-ttu-id="692e7-145">자산 편집, 이동 및 삭제</span><span class="sxs-lookup"><span data-stu-id="692e7-145">Edit, move, and delete assets</span></span>
<span data-ttu-id="692e7-146">만든 사용자 지정 자산을 편집할 수 있지만 Microsoft의 자산은 편집할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="692e7-146">You can edit custom assets that you create, but not assets from Microsoft.</span></span> <span data-ttu-id="692e7-147">그러나 재생 목록에서 모든 자산을 제거하고 주문 자산을 변경할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="692e7-147">However, you can remove all assets from a playlist and change the order assets.</span></span> 

![cg-playlistassetedit.png](media/cg-playlistassetedit.png)

### <a name="edit-an-asset"></a><span data-ttu-id="692e7-149">자산 편집</span><span class="sxs-lookup"><span data-stu-id="692e7-149">Edit an asset</span></span>
- <span data-ttu-id="692e7-150">자산에 대한 편집 단추를 클릭하고 자산을 수정한 다음 자산 저장을 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="692e7-150">Click the Edit button for an asset, modify the asset, and then click Save Asset.</span></span> 

### <a name="move-an-asset-in-a-playlist"></a><span data-ttu-id="692e7-151">재생 목록에서 자산 이동</span><span class="sxs-lookup"><span data-stu-id="692e7-151">Move an asset in a playlist</span></span>
- <span data-ttu-id="692e7-152">재생 목록에서 자산 순서를 이동하려면 자산 오른쪽의 위쪽 또는 아래쪽 화살표를 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="692e7-152">Click the up or down arrow to the right of the asset to move the asset order in the playlist</span></span>

### <a name="remove-an-asset-from-a-playlist"></a><span data-ttu-id="692e7-153">재생 목록에서 자산 제거</span><span class="sxs-lookup"><span data-stu-id="692e7-153">Remove an asset from a playlist</span></span>
- <span data-ttu-id="692e7-154">자산에 대한 재생 목록 X에서 제거 아이콘을 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="692e7-154">Click the Remove from Playlist X icon for the asset.</span></span> 

## <a name="view-the-playlist-in-action"></a><span data-ttu-id="692e7-155">동작에서 재생 목록 보기</span><span class="sxs-lookup"><span data-stu-id="692e7-155">View the playlist in Action</span></span>
<span data-ttu-id="692e7-156">이제 재생 목록에 자산을 추가했습니다. 이제 재생 목록을 닫고 실행 중으로 볼 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="692e7-156">Now that you've added assets to a playlist, let's close the playlist and see it in action.</span></span> 

1. <span data-ttu-id="692e7-157">재생 **목록 닫기 를 클릭합니다.**</span><span class="sxs-lookup"><span data-stu-id="692e7-157">Click **Close Playlist**.</span></span>
2. <span data-ttu-id="692e7-158">**Office 365** 교육 페이지가 있는 탭을 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="692e7-158">Click the tab with the **Office 365 training** page.</span></span>
3. <span data-ttu-id="692e7-159">페이지를 새로 고치고 시작 에서 첫 **번째 일** **을 클릭합니다.**</span><span class="sxs-lookup"><span data-stu-id="692e7-159">Refresh the page, and then click **First Days** under **Get Started**.</span></span>
4. <span data-ttu-id="692e7-160">학습 **경로 시작 키트를** 클릭하여 첫 번째 재생 목록을 볼 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="692e7-160">Click **Learning Pathways Starter Kit** to view your first playlist in action.</span></span> 

![cg-addassetcheckwork.png](media/cg-addassetcheckwork.png)