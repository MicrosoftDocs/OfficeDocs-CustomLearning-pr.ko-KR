---
author: pkrebs
ms.author: pkrebs
title: Microsoft 365 학습 경로 자산에 연결
ms.date: 02/15/2019
description: Microsoft 365 학습 경로 자산에 연결하는 방법
ms.service: sharepoint-online
ms.openlocfilehash: ae17cb531ffb66378749e4d96e72a8bb1db03dc3
ms.sourcegitcommit: 97e175e5ff5b6a9e0274d5ec9b39fdf7e18eb387
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/25/2021
ms.locfileid: "51999624"
---
# <a name="link-to-learning-pathways-content"></a><span data-ttu-id="f8f20-103">학습 경로 콘텐츠 링크</span><span class="sxs-lookup"><span data-stu-id="f8f20-103">Link to learning pathways content</span></span>

<span data-ttu-id="f8f20-104">학습 경로를 통해 콘텐츠에 연결하는 두 가지 방법이 있습니다.</span><span class="sxs-lookup"><span data-stu-id="f8f20-104">With learning pathways, there are two ways to link to content:</span></span>

- <span data-ttu-id="f8f20-105">표시할 콘텐츠에 대해 필터링된 웹 파트를 호스팅하는 페이지에 연결</span><span class="sxs-lookup"><span data-stu-id="f8f20-105">Link to the page that host the Web part filtered for the content you want to display</span></span> 
- <span data-ttu-id="f8f20-106">웹 파트의 인스턴스에 직접 연결</span><span class="sxs-lookup"><span data-stu-id="f8f20-106">Link directly to an instance of the Web part</span></span>

## <a name="link-to-a-page"></a><span data-ttu-id="f8f20-107">페이지에 연결</span><span class="sxs-lookup"><span data-stu-id="f8f20-107">Link to a page</span></span>

<span data-ttu-id="f8f20-108">Microsoft 365 학습 경로 웹 파트를 사용하여 새 페이지 및 학습 환경을 만든 경우 표시할 콘텐츠를 표시하도록 구성된 웹 파트가 있는 페이지에 연결하면 됩니다.</span><span class="sxs-lookup"><span data-stu-id="f8f20-108">If you've created new pages and learning experiences with the Microsoft 365 learning pathways web part, you can link to the page with the Web part configured to show the content you want to display.</span></span> <span data-ttu-id="f8f20-109">이전 섹션에서는 페이지에 Excel 재생 목록을 표시하는 방법을 설명했습니다.</span><span class="sxs-lookup"><span data-stu-id="f8f20-109">In the previous section, we covered how to display Excel playlists on a page.</span></span> <span data-ttu-id="f8f20-110">이제 홈 페이지를 편집하여 페이지에 연결될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="f8f20-110">You could now edit the Home page to link to the page.</span></span> 

1. <span data-ttu-id="f8f20-111">홈 페이지에서 편집을 **클릭합니다.**</span><span class="sxs-lookup"><span data-stu-id="f8f20-111">From the Home page, click **Edit**.</span></span>
2. <span data-ttu-id="f8f20-112">홈 **페이지 타일 중 하나에서** 세부 정보 편집을 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="f8f20-112">Click **Edit details** in one of the Home page tiles.</span></span> <span data-ttu-id="f8f20-113">이 예제에서는 권장 재생 **목록 타일을 편집합니다.**</span><span class="sxs-lookup"><span data-stu-id="f8f20-113">In this example, we edit the **Recommended playlists** tiles.</span></span>
3. <span data-ttu-id="f8f20-114">**링크에서** **변경을 클릭합니다.**</span><span class="sxs-lookup"><span data-stu-id="f8f20-114">Under **Link**, click **Change**.</span></span>

![cg-linktopage.png](media/cg-linktopage.png)

4. <span data-ttu-id="f8f20-116">**사이트,** 사이트 **페이지,** 연결하려는 페이지를 클릭한 다음 열기 를 **클릭합니다.**</span><span class="sxs-lookup"><span data-stu-id="f8f20-116">Click **Site**, then **Site Pages**, click the page you want to link to, and then click **Open**.</span></span> <span data-ttu-id="f8f20-117">이 예제에서는 이전 섹션에서 설명한 **Create-your-own-experience.aspx** 페이지에 연결합니다.</span><span class="sxs-lookup"><span data-stu-id="f8f20-117">In this example, we link to the **Create-your-own-experience.aspx** page covered in the previous section.</span></span>
5. <span data-ttu-id="f8f20-118">Hero 속성 창을 닫고 **게시를** 클릭한 다음 링크를 테스트합니다.</span><span class="sxs-lookup"><span data-stu-id="f8f20-118">Close the Hero properties pane, click **Publish**, and then test the link.</span></span> 

## <a name="link-to-the-microsoft-365-learning-pathways-web-part"></a><span data-ttu-id="f8f20-119">Microsoft 365 학습 경로 웹 파트에 연결</span><span class="sxs-lookup"><span data-stu-id="f8f20-119">Link to the Microsoft 365 learning pathways web part</span></span>
<span data-ttu-id="f8f20-120">학습 경로를 통해 웹 파트가 포함된 페이지와 독립적으로 웹 파트의 인스턴스에 연결하는 기능을 관리자 또는 최종 사용자에게 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="f8f20-120">Learning pathways gives you, the administrator, or an end-user, the ability to link to an instance of the Web part independent of the page that contains the Web part.</span></span> <span data-ttu-id="f8f20-121">복사한 링크를 공유하거나 다른 페이지에서 링크를 공유할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="f8f20-121">You can share the copied link or link to it from other pages.</span></span> <span data-ttu-id="f8f20-122">클릭할 때 복사된 링크는 CustomLLearningViewer.aspx 페이지에 Microsoft 365 학습 경로 웹 파트 인스턴스를 보여줍니다.</span><span class="sxs-lookup"><span data-stu-id="f8f20-122">The copied link, when clicked, shows the Microsoft 365 learning pathways web part instance in the CustomLLearningViewer.aspx page.</span></span> <span data-ttu-id="f8f20-123">예를 살펴보겠습니다.</span><span class="sxs-lookup"><span data-stu-id="f8f20-123">Let's look at an example.</span></span> 

1. <span data-ttu-id="f8f20-124">홈 페이지에서 **Microsoft365 교육 을 클릭합니다.**</span><span class="sxs-lookup"><span data-stu-id="f8f20-124">From the Home page, click **Microsoft365 training**.</span></span>
2. <span data-ttu-id="f8f20-125">**Microsoft Teams를** 클릭한 다음 **Microsoft Teams에 대한 시작을 클릭합니다.**</span><span class="sxs-lookup"><span data-stu-id="f8f20-125">Click **Microsoft Teams**, and then click **Intro to Microsoft Teams**.</span></span>
3. <span data-ttu-id="f8f20-126">복사 **아이콘을** 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="f8f20-126">Click the **Copy** icon.</span></span>

![cg-linktowebpart.png](media/cg-linktowebpart.png)

4. <span data-ttu-id="f8f20-128">Microsoft 365 학습 경로 사이트 메뉴에서 홈을 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="f8f20-128">Click Home from the Microsoft 365 learning pathways site menu.</span></span>
5. <span data-ttu-id="f8f20-129">복사한 URL을 브라우저의 주소 표시줄에 붙여넣고 Enter를 누르세요.</span><span class="sxs-lookup"><span data-stu-id="f8f20-129">Paste the copied URL in the address bar of the browser and press ENTER.</span></span> 

<span data-ttu-id="f8f20-130">다음 그림과 같이 링크는 CustomLearningViewer.aspx 페이지로 이동하여 복사된 링크의 매개 변수에 따라 콘텐츠를 나타냅니다.</span><span class="sxs-lookup"><span data-stu-id="f8f20-130">As shown in the following illustration, the link goes to the CustomLearningViewer.aspx page and displays the content based on the parameters in the copied link.</span></span> 

![cg-linktowebpartviewer.png](media/cg-linktowebpartviewer.png)

