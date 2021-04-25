---
author: pkrebs
ms.author: pkrebs
title: 재생 목록용 SharePoint 페이지 만들기
ms.date: 02/10/2019
description: 재생 목록용 SharePoint 페이지 만들기
ms.service: sharepoint-online
ms.openlocfilehash: 40c249fbd5b0fdaefd555f23bf20ac23240ea954
ms.sourcegitcommit: 97e175e5ff5b6a9e0274d5ec9b39fdf7e18eb387
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/25/2021
ms.locfileid: "51999094"
---
# <a name="create-sharepoint-pages-for-custom-playlists"></a><span data-ttu-id="ba5eb-103">사용자 지정 재생 목록용 SharePoint 페이지 만들기</span><span class="sxs-lookup"><span data-stu-id="ba5eb-103">Create SharePoint pages for Custom Playlists</span></span>

<span data-ttu-id="ba5eb-104">학습 경로의 고유한 기능 중 하나는 Microsoft의 자산 및 만든 SharePoint 자산에서 어셈블된 재생 목록을 만드는 기능입니다.</span><span class="sxs-lookup"><span data-stu-id="ba5eb-104">One of the unique features of learning pathways is the ability to create playlists that are assembled from assets from Microsoft and from SharePoint assets that you create.</span></span> <span data-ttu-id="ba5eb-105">이 예제에서는 재생 목록을 만들기에 앞서 SharePoint 페이지를 만들어 보겠습니다.</span><span class="sxs-lookup"><span data-stu-id="ba5eb-105">In this example, we’ll create a SharePoint page in advance of creating a playlist.</span></span> <span data-ttu-id="ba5eb-106">SharePoint 페이지에서 재생 목록을 작성하는 기능을 통해 Microsoft 또는 조직에서 사용할 수 있는 웹 파트를 사용하여 페이지를 빌드할 수 있는 다양한 기회를 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="ba5eb-106">The ability to build playlists from SharePoint pages offers a variety of opportunities to build pages using the Web parts available from Microsoft or your organization.</span></span> <span data-ttu-id="ba5eb-107">예를 들어 재생 목록에는 YouTube의 비디오가 포함된 SharePoint 페이지 또는 Office 365 Forms에서 작성된 양식 또는 포함된 Power BI 보고서가 포함됩니다.</span><span class="sxs-lookup"><span data-stu-id="ba5eb-107">For example, a playlist can include a SharePoint page with embedded videos from YouTube, or a form built from Office 365 Forms, or an embedded Power BI report.</span></span> <span data-ttu-id="ba5eb-108">이 예제에서는 Embed 웹 파트 및 텍스트 웹 파트를 사용하여 페이지를 작성하는 방법을 보여 주겠습니다.</span><span class="sxs-lookup"><span data-stu-id="ba5eb-108">In this example, we’ll show you how to build a page with the Embed web part and the Text web part.</span></span>  

## <a name="create-a-sharepoint-page-for-a-custom-playlist"></a><span data-ttu-id="ba5eb-109">사용자 지정 재생 목록에 대한 SharePoint 페이지 만들기</span><span class="sxs-lookup"><span data-stu-id="ba5eb-109">Create a SharePoint page for a custom playlist</span></span>

1. <span data-ttu-id="ba5eb-110">SharePoint **기어** 아이콘을 클릭한 다음 페이지 **추가 를 클릭합니다.**</span><span class="sxs-lookup"><span data-stu-id="ba5eb-110">Click the SharePoint **Gear** icon, and then click **Add a page**.</span></span>
2. <span data-ttu-id="ba5eb-111">페이지 **왼쪽에** 있는 새 섹션 추가(+)를 클릭한 다음 섹션 레이아웃에 대해 두 **개의 열을** 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="ba5eb-111">Click **Add a new section (+)** on the left-hand side of the page, and then click **Two Columns** for the section layout.</span></span>
3. <span data-ttu-id="ba5eb-112">왼쪽 열에서 + 를 클릭한 다음 **Embed** 웹 파트를 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="ba5eb-112">In the left column, click + , and then click the **Embed** web part.</span></span> 
4. <span data-ttu-id="ba5eb-113">오른쪽 열에서 +를 클릭한 다음 텍스트 웹 **파트를** 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="ba5eb-113">In the right column, click +, and then click the **Text** web part.</span></span> <span data-ttu-id="ba5eb-114">페이지는 다음과 같이 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="ba5eb-114">Your page should look like this.</span></span>

![cg-pagenewstart.png](media/cg-pagenewstart.png)

### <a name="add-a-video-and-text-from-youtube"></a><span data-ttu-id="ba5eb-116">YouTube에서 비디오 및 텍스트 추가</span><span class="sxs-lookup"><span data-stu-id="ba5eb-116">Add a video and text from YouTube</span></span>

1. <span data-ttu-id="ba5eb-117">브라우저에서 YouTube로 이동하세요.</span><span class="sxs-lookup"><span data-stu-id="ba5eb-117">In your browser, go to YouTube.</span></span> <span data-ttu-id="ba5eb-118">이 예제에서는 "Office 365 - Microsoft 최고의 생산성 앱"을 검색합니다.</span><span class="sxs-lookup"><span data-stu-id="ba5eb-118">For this example, search for “What is Office 365 – Microsoft’s best productivity apps”.</span></span>
2. <span data-ttu-id="ba5eb-119">비디오를 클릭하여 재생한 다음 일시 중지한 다음 마우스 오른쪽 단추로 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="ba5eb-119">Click the video to play it, then pause it, then right-click on it.</span></span> 
3. <span data-ttu-id="ba5eb-120">임의 **코드 복사를 클릭한** 다음 SharePoint 페이지로 돌아오십시오.</span><span class="sxs-lookup"><span data-stu-id="ba5eb-120">Click **Copy embed code**, then return to the SharePoint page.</span></span> 
4. <span data-ttu-id="ba5eb-121">**Embed** 웹 파트에  코드 추가를 클릭한 다음 YouTube 비디오에서 코드를 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="ba5eb-121">Click **Add embed code** in the **Embed** web part, and then add the code from the YouTube video.</span></span>
5. <span data-ttu-id="ba5eb-122">YouTube 페이지로 돌아가서 비디오의 **설명** 텍스트를 복사합니다.</span><span class="sxs-lookup"><span data-stu-id="ba5eb-122">Return to the YouTube page and copy the **Description** text for the video.</span></span> 
6. <span data-ttu-id="ba5eb-123">SharePoint 페이지로 돌아가서  텍스트 웹 파트를 선택한 다음 YouTube 비디오에서 텍스트를 복사합니다.</span><span class="sxs-lookup"><span data-stu-id="ba5eb-123">Return to the SharePoint page, select the **Text** web part, then copy the text from the YouTube video.</span></span>
7. <span data-ttu-id="ba5eb-124">SharePoint **페이지의** 제목 영역에 있는 웹 파트 편집 아이콘을 선택한 다음 페이지의 이름을 "사용자 지정 재생 목록 소개"로 지정합니다.</span><span class="sxs-lookup"><span data-stu-id="ba5eb-124">Select the **Edit web part** icon  in the Title area of the SharePoint page, and then name the page “Custom Playlist Introduction”.</span></span> 
8. <span data-ttu-id="ba5eb-125">레이아웃의 경우 **일반을** 선택한 다음 제목 **영역 속성** 창을 닫습니다. </span><span class="sxs-lookup"><span data-stu-id="ba5eb-125">For **Layout**, select **Plain**, then close **Title Region** properties pane.</span></span> <span data-ttu-id="ba5eb-126">이제 페이지는 다음과 같이 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="ba5eb-126">The page should now look something like the following.</span></span> 

![cg-pagenewfinish.png](media/cg-pagenewfinish.png)

### <a name="publish-the-page"></a><span data-ttu-id="ba5eb-128">페이지 게시</span><span class="sxs-lookup"><span data-stu-id="ba5eb-128">Publish the page</span></span>

- <span data-ttu-id="ba5eb-129">게시 **단추를** 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="ba5eb-129">Select the **Publish** button.</span></span> <span data-ttu-id="ba5eb-130">이제 사용자 지정 재생 목록에 이 SharePoint 페이지를 추가할 준비가 완료되었습니다.</span><span class="sxs-lookup"><span data-stu-id="ba5eb-130">Now you're ready to add this SharePoint page to your custom playlist.</span></span> 