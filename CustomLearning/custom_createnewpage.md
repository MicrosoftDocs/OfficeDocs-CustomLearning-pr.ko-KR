---
author: pkrebs
ms.author: pkrebs
title: 재생 목록에 대 한 SharePoint 페이지 만들기
ms.date: 02/10/2019
description: 재생 목록에 대 한 SharePoint 페이지 만들기
ms.openlocfilehash: c2de66a0746260e8f6539656ad70052b209c54ba
ms.sourcegitcommit: 775d6807291ab263eea5ec649d9aaf1933fb41ca
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32055504"
---
# <a name="create-sharepoint-pages-for-custom-playlists"></a><span data-ttu-id="e0725-103">사용자 지정 재생 목록에 대 한 SharePoint 페이지 만들기</span><span class="sxs-lookup"><span data-stu-id="e0725-103">Create SharePoint pages for Custom Playlists</span></span>

<span data-ttu-id="e0725-104">사용자 지정 학습의 고유한 기능 중 하나는 Microsoft와 만든 SharePoint 자산의 자산에서 어셈블된 재생 목록을 만드는 기능입니다.</span><span class="sxs-lookup"><span data-stu-id="e0725-104">One of the unique features of Custom Learning is the ability to create playlists that are assembled from assets from Microsoft and from SharePoint assets that you create.</span></span> <span data-ttu-id="e0725-105">이 예제에서는 재생 목록을 만들기 전에 SharePoint 페이지를 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="e0725-105">In this example, we’ll create a SharePoint page in advance of creating a playlist.</span></span> <span data-ttu-id="e0725-106">SharePoint 페이지에서 재생 목록을 작성 하는 기능은 Microsoft 또는 조직에서 사용할 수 있는 웹 파트를 사용 하 여 페이지를 작성할 수 있는 다양 한 기회를 제공 합니다.</span><span class="sxs-lookup"><span data-stu-id="e0725-106">The ability to build playlists from SharePoint pages offers a variety of opportunities to build pages using the Web parts available from Microsoft or your organization.</span></span> <span data-ttu-id="e0725-107">예를 들어 재생 목록에는 YouTube의 포함 비디오가 있는 SharePoint 페이지 또는 Office 365 양식에서 작성 된 양식 또는 임베디드 Power BI 보고서가 포함 될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="e0725-107">For example, a playlist can include a SharePoint page with embedded videos from YouTube, or a form built from Office 365 Forms, or an embedded Power BI report.</span></span> <span data-ttu-id="e0725-108">이 예제에서는 Embed 웹 파트 및 텍스트 웹 파트가 포함 된 페이지를 작성 하는 방법을 보여 줍니다.</span><span class="sxs-lookup"><span data-stu-id="e0725-108">In this example, we’ll show you how to build a page with the Embed web part and the Text web part.</span></span>  

## <a name="create-a-sharepoint-page-for-a-custom-playlist"></a><span data-ttu-id="e0725-109">사용자 지정 재생 목록에 대 한 SharePoint 페이지 만들기</span><span class="sxs-lookup"><span data-stu-id="e0725-109">Create a SharePoint page for a custom playlist</span></span>

1. <span data-ttu-id="e0725-110">SharePoint **기어** 아이콘을 클릭 한 다음 **페이지 추가**를 클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="e0725-110">Click the SharePoint **Gear** icon, and then click **Add a page**.</span></span>
2. <span data-ttu-id="e0725-111">페이지 왼쪽에서 **새 섹션 (+) 추가** 를 클릭 한 다음 섹션 레이아웃에 대해 **두 개의 열** 을 클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="e0725-111">Click **Add a new section (+)** on the left-hand side of the page, and then click **Two Columns** for the section layout.</span></span>
3. <span data-ttu-id="e0725-112">왼쪽 열에서 +를 클릭 하 고 **Embed** 웹 파트를 클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="e0725-112">In the left column, click + , and then click the **Embed** web part.</span></span> 
4. <span data-ttu-id="e0725-113">오른쪽 열에서 +를 클릭 하 고 **텍스트** 웹 파트를 클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="e0725-113">In the right column, click +, and then click the **Text** web part.</span></span> <span data-ttu-id="e0725-114">페이지 모양은 다음과 같습니다.</span><span class="sxs-lookup"><span data-stu-id="e0725-114">Your page should look like this.</span></span>

![cg-pagenewstart-.png](media/cg-pagenewstart.png)

### <a name="add-a-video-and-text-from-youtube"></a><span data-ttu-id="e0725-116">YouTube에서 비디오 및 텍스트 추가</span><span class="sxs-lookup"><span data-stu-id="e0725-116">Add a video and text from YouTube</span></span>

1. <span data-ttu-id="e0725-117">브라우저에서 YouTube로 이동 합니다.</span><span class="sxs-lookup"><span data-stu-id="e0725-117">In your browser, go to YouTube.</span></span> <span data-ttu-id="e0725-118">이 예에서는 "Office 365-Microsoft의 최상의 생산성 앱"을 검색 합니다.</span><span class="sxs-lookup"><span data-stu-id="e0725-118">For this example, search for “What is Office 365 – Microsoft’s best productivity apps”.</span></span>
2. <span data-ttu-id="e0725-119">동영상을 클릭 하 여 재생 한 다음 일시 중지 하 고 마우스 오른쪽 단추로 클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="e0725-119">Click the video to play it, then pause it, then right-click on it.</span></span> 
3. <span data-ttu-id="e0725-120">**embed 태그 복사**를 클릭 하 고 SharePoint 페이지로 돌아갑니다.</span><span class="sxs-lookup"><span data-stu-id="e0725-120">Click **Copy embed code**, then return to the SharePoint page.</span></span> 
4. <span data-ttu-id="e0725-121">**embed** 웹 파트에서 **embed 태그 추가** 를 클릭 한 다음 YouTube 비디오에서 코드를 추가 합니다.</span><span class="sxs-lookup"><span data-stu-id="e0725-121">Click **Add embed code** in the **Embed** web part, and then add the code from the YouTube video.</span></span>
5. <span data-ttu-id="e0725-122">YouTube 페이지로 돌아간 후 비디오에 대 한 **설명** 텍스트를 복사 합니다.</span><span class="sxs-lookup"><span data-stu-id="e0725-122">Return to the YouTube page and copy the **Description** text for the video.</span></span> 
6. <span data-ttu-id="e0725-123">SharePoint 페이지로 돌아와서 **텍스트** 웹 파트를 선택한 다음 YouTube 비디오에서 텍스트를 복사 합니다.</span><span class="sxs-lookup"><span data-stu-id="e0725-123">Return to the SharePoint page, select the **Text** web part, then copy the text from the YouTube video.</span></span>
7. <span data-ttu-id="e0725-124">SharePoint 페이지의 제목 영역에서 **웹 파트 편집** 아이콘을 선택 하 고 페이지 이름을 "사용자 지정 재생 목록 소개"로 지정한 다음</span><span class="sxs-lookup"><span data-stu-id="e0725-124">Select the **Edit web part** icon  in the Title area of the SharePoint page, and then name the page “Custom Playlist Introduction”.</span></span> 
8. <span data-ttu-id="e0725-125">**레이아웃**에서 **일반**을 선택한 다음 **제목 영역** 속성 창을 닫습니다.</span><span class="sxs-lookup"><span data-stu-id="e0725-125">For **Layout**, select **Plain**, then close **Title Region** properties pane.</span></span> <span data-ttu-id="e0725-126">페이지의 모양은 다음과 같습니다.</span><span class="sxs-lookup"><span data-stu-id="e0725-126">The page should now look something like the following.</span></span> 

![cg-pagenewfinish-.png](media/cg-pagenewfinish.png)

### <a name="publish-the-page"></a><span data-ttu-id="e0725-128">페이지 게시</span><span class="sxs-lookup"><span data-stu-id="e0725-128">Publish the page</span></span>

- <span data-ttu-id="e0725-129">**게시** 단추를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="e0725-129">Select the **Publish** button.</span></span> <span data-ttu-id="e0725-130">이제이 SharePoint 페이지를 사용자 지정 재생 목록에 추가할 준비가 되었습니다.</span><span class="sxs-lookup"><span data-stu-id="e0725-130">Now you're ready to add this SharePoint page to your custom playlist.</span></span> 